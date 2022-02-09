<template>
  <article>
    <h3> {{post.title}}</h3>
    <div class="date">{{post.created_at}}</div>
    <p class="text">{{post.content}}</p>
  </article>
</template>

<script>
export default {
  name:'PostItem',
  props:{
    'post': Object
  }
}
</script>

<style lang="scss" scoped>

  article{
    margin-bottom: 20px;
    .date{
      font-size: 12px;
      font-style: italic;
    }
    .text{
      padding: 10px 0;
    }
  }

</style>