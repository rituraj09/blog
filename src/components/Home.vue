<template>
  <div>
    <h1>Hello from Home Component</h1>
    <h2 v-if="show">{{ data }}</h2>
    <div v-else>
        <table border="1px">
            <tr>
                <td>
                    ID
                </td>
                <td>
                    Name
                </td>
                <td>
                    Email
                </td>
            </tr>
             <tr v-for="user in users" :key="user.id">
                <td>
                    {{user.id}}
                </td>
                <td>
                    {{user.name}}
                </td>
                <td>
                    {{user.email}}
                </td>
            </tr>
        </table>
    </div>
    <button v-on:click="hello('Data is added')">Clcik Me!</button><br><br>
    <button v-on:click="display()">Toggle!</button>
  </div>
</template>
<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String,
  },
  data(){
        return {
            show:true,
            users:[
                {id:1001, name: 'Ritz', email: 'ritz@gmail.com'},
                {id:1002, name: 'Kiranmoyee', email: 'kiran@gmail.com'},
                {id:1003, name: 'Dulumoni', email: 'dulu@gmail.com'},
                {id:1004, name: 'Sania', email: 'sania@gmail.com'},
            ]

        }

  },
  methods: {
    hello(d) {
        alert("Hello Console "+d);
    },
    display(){
        this.show=!this.show;
    }
  },
};
</script>