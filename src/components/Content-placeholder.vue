<!--Content placeholders for the search grid created by @Mahelaa -->
<template>

    <div class="content-placeholder-container">
    <figure class="content-placeholder_item">
    <img ref="img" :class="{'content-placeholder-image': true}"
      :image="Placeholder" src="../assets/SVGSearch.svg">
       </figure>
    </div>

</template>

<script>

export default {
  name: 'Placeholder',
  props: ['Skeleton'],
  data() {
    return {
      windowHeight: 0,
      Placeholder: '',
    };
  },

};

</script>

<!--Todo l8r- calculate size with the help of the screensize calculator, animate, fragment-->
<style lang="scss" scoped>
.content-placeholder-container{
  margin: 10px;
}

.content-placeholder-image{
    margin: auto;
    display: block;
  }

.content-placeholder_item {
    width: 30%;
    padding: 1%;
    position: relative;
    display: block;
    float: left;
    flex: 0 0 auto;
    flex-grow: 1;
    cursor: pointer;
  }


</style>
