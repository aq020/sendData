<template>
   <div>
       <Child :msg1= "msg" @getMessage= "getmsg" />
       Home:{{msgv1}}      
   </div>
</template>

<script>
import Child from "../../components/Child"
export default {
    name:"Home",
    components:{
        Child
    },
    data(){
        return{
            msg: "父组件先传数据给子组件" ,
            msgv1 : " "

        }
    },
    methods:{
        getmsg(data){
           this.msgv1 = data;
            console.log(data)
        }
    }
}
</script>

<style>

</style>