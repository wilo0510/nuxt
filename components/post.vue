<template>
    <nuxt-link :to="'/posts/'+id">
        <div class="post">
        <p>{{id}}.{{name}}</p>
       
        </div> 
    </nuxt-link>
    
</template>
<script>
export default {
    name:'Post',
    props:['id','name']
}
</script>
<style scoped>
    .post{
        padding: 1rem;
        border: 1px solid whitesmoke;
        margin: 1rem 0rem;
    }
    .post:hover{
        background: #2d3436;
        border: 1px solid #6c5ce7;
        cursor: pointer;
    }
    a{
        color:whitesmoke;
        text-decoration: none;
    }
    a:hover{
        color:#6c5ce7;
        text-decoration: none;
    }
</style>