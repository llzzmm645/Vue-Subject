<template>
    <from @submit.prevent="postdata">
        名字:<input type="text" v-model="name" id="name">
        <br>
        年龄:<input type="text" v-model="age" id="age">
        <br>
        幸运数字:<input type="text" v-model="lucknumber" id="lucknumber">
        <br>
        <input type="submit" value="提交">
    </from>
</template>
<script>
export default {
    data(){
        return {
            name:"Liuzimo",
            age:11,
            lucknumber:5
        }
    },
    methods:{
        postdata(){
            alert(this.name+" - "+this.$data.age.toString()+" - "+this.lucknumber.toString())
        }
    }
}
</script>