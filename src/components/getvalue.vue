<template>
<h1>Get Input Field value</h1>
<input type="text" placeholder="enter email" v-model="email"/>
<br />
<br />
<input type="password" placeholder="enter password"  v-model="password"/>
<br />
<br />
<button v-on:click="getData()" type="button">Get Values</button>
<h2>Get Radio Button And Checkbox value</h2>
<h3>Technology</h3>
<label for="java">Java</label>
<input type="checkbox" value="Java" id="java" v-model="technology"/>

<label for="php">PHP</label>
<input type="checkbox" value="php" id="php" v-model="technology"/>

<label for="node">Node</label>
<input type="checkbox" value="node" id="node" v-model="technology"/>

<h4>I am a developer of : {{technology}}</h4>

<h3>Vehical</h3>
<label for="car">Car</label>
<input type="radio" value="car" name="vehical" id="car" v-model="vehical"/>

<label for="bike">Bike</label>
<input type="radio" value="bike" name="vehical" id="bike" v-model="vehical"/>

<h4>I am purchashing a new : {{vehical}}</h4>
</template>

<script>
export default {
    name: 'getvalue',
    data() {
        return{
            email:null,
            password:null,
            technology:[],
            vehical: [],
        }
    },
    methods:{
        getData() {
            console.log("Values :",this.email,this.password)
        }
    },
};
</script>
