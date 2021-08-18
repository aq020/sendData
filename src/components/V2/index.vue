<template>
    <div>
        V2:{{v2msg}}
    </div>
</template>

<script>
export default {
    name: "V2",
    props:{
        v2msg:{
            type: String,
            default: ""
        }
    }

}
</script>
<style scoped>

</style>