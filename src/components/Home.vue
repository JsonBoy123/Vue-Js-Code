<template>
<h1>First Home Component {{10+20}}</h1>
<h1>Email {{email}}</h1>
<h1>Name {{getName()}}</h1>
<h1>Name {{setName()}}</h1>
<h1>All Data {{getData().email}}</h1>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            email: 'abc@test.com',
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
        }
    }
}
</script>

<style scoped>
h1 {
    color: #fa0000;
    font-style: italic;
}
</style>
