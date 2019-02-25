<template>
    <div>
      
     <h1>New Quote</h1>
     <button @click="counter++">Increase</button>
     {{counter}}
    </div>
</template>

<script>
export default {
    data: function (){
        return{
           counter:0
        }
    },
    destroyed(){
       console.log('destroyed');
    },
    activated(){
        console.log('activated')
    },
    deactivated(){
        console.log('deactivated');
    }
}
</script>

<style>

</style>


