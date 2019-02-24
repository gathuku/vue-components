<template>
    <div>
      
        <div class="title">
            <slot name="title"></slot>
            <slot name="content"></slot>
        </div>
       <hr>
        <div>
            <slot name="title"></slot>
            <slot name="content"></slot>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
div{
    padding: 30px;
    
    margin: 20px auto;
    font-weight: 700;
    text-align: center;
}

h1 {
    color: blue;
}
.title {
    font-style: italic;
}
</style>


