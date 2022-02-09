<template>
<h1 v-on:mousemove="getConsole()">First Home Component {{10+20}}</h1>
<h1>Email {{email}}</h1>
<h1>Name {{getName()}}</h1>
<h1>Name {{setName()}}</h1>
<h1>All Data {{getData().email}}</h1>
<button v-on:click="setData()">Click Me</button>
<button v-on:dblclick="setData('Button double clicked')">Click Me</button>
<h2>{{count}}</h2>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            email: 'abc@test.com',
            count:0,
            getName: function () {
                return "ABC"
            }
        }
    },
    methods: {
        setName() {
            return "DBF_POS"
        },
        getData() {
            return {
                name: "sam",
                email: this.email
            }
        },
        setData() {
            this.count=this.count+1
        },
        getConsole() {
            console.warn("same")
        }
    },
}
</script>

<style scoped>
h1 {
    color: #fa0000;
    font-style: italic;
}
</style>
