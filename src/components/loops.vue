<template>
<h1>Loops</h1>
<h2>Technology Name</h2>
<ul>
    <li v-for="item in technology" :key="item">
        {{item}}
    </li>
</ul>

<h2>Users Name And Email</h2>
<ul>
    <li v-for="item in user" :key="item.email">
        Name is : {{item.name}} And Email is : {{item.email}}
    </li>
</ul>
</template>

<script>
export default {
    name: 'loops',
    data() {
        return {
            technology: ['java', 'react', 'node', 'javascript'],
            user: [{
                    name: 'Sam',
                    email: 'sam@gmail.com'
                },
                {
                    name: 'Ram',
                    email: 'ram@gmail.com'
                },
                {
                    name: 'Aman',
                    email: 'aman@gmail.com'
                }
            ]
        }
    }
};
</script>
