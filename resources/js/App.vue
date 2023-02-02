<template>
    <h1>Componente Vue</h1>
</template>

<script>
import { assertExpressionStatement, throwStatement } from '@babel/types';
import { response } from 'express';

    export default{
        name: 'App',
        data() {
            return {
                arrPosts: [],
            };
        },

        created() {
            axios.get('/api/post')
                then(response => this.arrPosts = responde.data.results)
        }
    }
</script>


