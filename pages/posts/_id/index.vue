<template>
    <div>
        <h1>{{post.body}}</h1>
    </div>
   
</template>
<script>
import axios from 'axios'
export default {
    data(){
        return{
            post:{}
        }
    },
    async created(){
        
        const res= await axios.get('https://jsonplaceholder.typicode.com/posts/'+this.$route.params.id)
        this.post=res.data
    }
}
</script>