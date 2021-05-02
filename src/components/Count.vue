<template>
    <div>
        <p><slot></slot></p>
        <p v-if="cntr>0">Counting {{cntr}} {{theMesg}}</p>
        <button @click="addMe">Add One to Button</button>
    </div>
</template>


<script>

export default{
    name: 'Count',
    props: ['msg'],
    data()
    {   
        return {
            theMesg : this.msg,
            cntr: 0
        }
    },
    methods:
    {
        addMe()
        {
            this.theMesg = this.msg + " One more added";
            this.cntr++
        }
    }
   
}
</script>

<style scoped>
    div {background: linear-gradient(to left, #1f4037, #99f2c8);
        padding: 5px; 
        border-bottom: 2px black dotted
    }

</style>
