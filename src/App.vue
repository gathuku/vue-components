<template>
 <div>
   <div class="container">
      <button @click="selectedComponent='appQuote'">Quote</button>
          <button @click="selectedComponent='appAuthor'">Author</button>
          <button @click="selectedComponent='appNew'">New</button>
          <p>{{selectedComponent}}</p>
        <app-quote>

         

          <h1 slot="title">{{quoteTitle}}</h1>
          <p slot="content">A wonderful Quote</p>
        </app-quote>

        
   </div>
 </div>
</template>

<script>
import Quote from './components/Quote.vue'
import Author from './components/Author.vue'
import New from './components/New.vue'

export default {
 components:{
  appQuote:Quote,
  appAuthor:Author,
  appNew:New
 },

 data: function(){
     return {
       quoteTitle:'The Quote',
       selectedComponent: 'Quote'
       
     }
 }
}
</script>

<style>

</style>
