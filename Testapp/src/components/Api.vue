<template>
    <div class="container">
       <h1 style="{color: '#000';}">{{ title  }}</h1>
        <hr>
        <table>
            <tr>
                <th>
                    POST ID
                </th>
                <th>
                Post Title 
                </th>
                <th>
                    POST BODY
                </th>
            </tr>
            <tr v-for="item in retrive" v-bind:key="item.id">
                <td>
                    {{ item.id }}
                </td>

                <td>
                    {{ item.title }}
                </td>
                <td>
                    {{ item.body }}
                </td>
            </tr>
        </table>
    </div>
</template>


<script>
// import Vue from 'vue'
// import axios from 'axios';
// import VueAxios from 'axios'
import data from './Data.json'
export default {
    api: 'Api',
    props: {
        title: String,
    }, data() {
        return {
            retrive: null
        }
    }, methods: {

        deleteacc(id) {
            alert(`this is tartget id ${id}`)
        },
        edit(id) {
            const listitem = data.filter((item) => {
                return item.id === id ? item : null;
            });

        },

    },
    mounted() {
        fetch("https://jsonplaceholder.typicode.com/posts")
            .then(response => response.json())
            .then(json => {
                this.retrive = json;
            })
    }
}
</script>


<style>
* {
    text-transform: capitalize;
}

table tr{
  padding: 1px  solid red;
}

table tr th {
      border: 1px solid orange;
}
table tr td {
   border: 2px solid gray;   
}

.container {
    margin-top: 30px;
}

.card {
    margin-top: 50px;
    padding: 10px;
    width: 400px;
    min-height: 300px;
    background-color: rgb(239, 243, 231);
    box-shadow: 2px 2px 10px rgb(91, 88, 88);
    border-radius: 10px;
}

.btn {
    padding: 2px 10px;
    margin: 0px 5px;
}

.btn:nth-child(1) {
    background-color: rgb(175, 94, 12);
    color: #fff;
    border: none;
    cursor: pointer;
}

.btn:nth-child(2) {
    background-color: rgb(187, 8, 8);
    color: #fff;
    border: none;
    cursor: pointer;
}

.account {
    width: 300px;
    display: flex;
    align-items: center;
    justify-content: space-around;
}
</style>
