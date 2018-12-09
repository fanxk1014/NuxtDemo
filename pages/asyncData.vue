<template>
    <div>
        {{name}}
        <h1>name:{{info.name}}</h1>
        <h2>age:{{info.age}}</h2>
        <h3>interest:{{info.interest}}</h3>
    </div>
</template>

<script>
    import axios from 'axios'
    export default{
        data(){
            return {
                name:'hello nuxt'
            }
        },
        // asyncData(){
        //     return axios.get('https://api.myjson.com/bins/14qge6');
        //     .then((res)=>{
        //         console.log(res);
        //         return {
        //             info:res.data
        //         }
        //     })
        // },
        async asyncData(){
            let {data} = await axios.get('https://api.myjson.com/bins/14qge6');
            console.log({data},data);
            return {info:data}
        }
    }
</script>