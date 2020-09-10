<template>
    <div>
        <h1>POSTS</h1>
        <Post
            v-for=" post of arregloPublicaciones"
            :key="post.id" 
            :name="post.title" 
            :id="post.id"
            
        />
    </div>
    
</template>
<script>
import axios from 'axios'
import Post from '../../components/post'
export default {
    components:{
        Post:Post
    },
    data(){
        return{
            arregloPublicaciones:[]
        }
    },
    async created(){
        try{
            const res=await axios.get('https://jsonplaceholder.typicode.com/posts')
            this.arregloPublicaciones=res.data
        }catch(error){
            console.log(error)
        }
                
    }
}
</script>
<style>
    
</style>