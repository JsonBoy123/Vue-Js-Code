<template>
<h1>If Else conditions</h1>
<h2 v-if="show">If condition</h2>
<h3 v-else>Else condition</h3>
<button v-on:click="show=!show">Toggle</button>
</template>

<script>
export default {
    name: 'conditions',
    data() {
        return {
            show:true
        }
    }
};
</script>