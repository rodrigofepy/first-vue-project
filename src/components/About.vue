<template>
  <div class="about">
    <h1>Hello {{their_name}} This is an about page</h1>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugit, quaerat? Dolorem expedita illo neque quasi aspernatur tenetur suscipit, quod excepturi eaque assumenda, cum eius corporis unde delectus? Illum, distinctio ad.</p>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      their_name: this.$route.params.name
    }
  }
}
</script>
