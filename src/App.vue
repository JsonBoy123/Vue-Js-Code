<template>
<img alt="Vue logo" src="./assets/logo.png" />
<HelloWorld msg="Welcome to Your New Vue.js App" />
<Home />
<test />
<getvalue />
<conditions />
<loops />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Home from "./components/Home.vue";
import test from "./components/test.vue";
import getvalue from "./components/getvalue.vue";
import conditions from "./components/conditions.vue";
import loops from "./components/loops.vue";

export default {
    name: "App",
    components: {
        HelloWorld,
        Home,
        test,
        getvalue,
        conditions,
        loops,
    },
};
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
