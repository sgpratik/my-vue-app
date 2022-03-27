<template>
    <div @load="getQuotes()" class="quote"><i>"The quote will be displayed here."</i> </div>
</template>

<script>

export default {
    components:{
        name: 'Quote'
    },

}
</script>

<style scoped>

.quote {
  max-width: 400px;
  margin: 10px auto;
  overflow: auto;
  min-height: 50px;
  border: 1px solid rgb(29, 167, 221);
  padding: 30px;
  border-radius: 50px;
}

</style>
