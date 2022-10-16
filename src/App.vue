<template>
  <DIV>
    <div>
      <button v-on:click="addLike">Like</button>
      <button v-on:click="addDislike">Dislike</button>
    </div>
    <div>
      Likes count <strong>{{ likes }}</strong>
      Dislikes count <strong>{{ dislikes }}</strong>
    </div>
  </DIV>
</template>

<script>
  export default {
    data() {
      return {
        likes: 0,
        dislikes: 5,
      }
    },
    methods: {
      addLike() {
        this.likes += 1;
      },
      addDislike() {
        this.dislikes += 1;
      }
    }
  }
</script>

<style>

</style>
