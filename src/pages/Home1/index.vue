<template>
    <div>
        V1、V2组件经过父组件（中介）传数据
        <V1 @sendMSG= "getMSG" />
        <V2 :v2msg= "msg" />
    </div>
</template>

<script>
import V1 from "../../components/V1"
import V2 from "../../components/V2"
export default {
    name: "Home1",
    components:{
        V1,
        V2
    },
    data(){
        return{
            msg: ""
        }
    },
    methods:{
        getMSG(data){
            this.msg = data,
            console.log(data)
        }
    }

}
</script>
<style scoped>

</style>