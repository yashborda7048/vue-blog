<!-- There is two part of new component one is template and second is script -->
<template>
    <!-- in template there is only one route component -->
    <div>
        <h1>Data coming from Home</h1>
        <p>{{ data }}</p>
        <p>{{ msg }}</p>
        <button v-on:click="myFun()">Call Me</button>
        <!-- if else condition -->
        <h2 v-if="show">Show this line on vue</h2>
        <h2 v-else>Hide this line for vue</h2>
        <button v-on:click="toggle()">Toggle</button>
    </div>
</template>

<script>
    export default{
        name:'Home',
        // It is compulsory to define data type of property when we are using interpolation as below
        props:{
            data:String,
            msg:String
        },
        // For event Element we have to use of method
        methods:{
            myFun(){
                alert("Hello chanmol, what's going with vue ?")
            },
            // To make toggle for if else condition
            toggle(){
                if(this.show==true)
                this.show=false
                else{
                    this.show=true
                }
                // this.show=!this.show         //This is known as negation which work short of if else condition
            }
        },
        // For making toggle we have to make data() likewise
        data(){
            return {show:true}
        }
    }
</script>