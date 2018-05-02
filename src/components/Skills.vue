<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data,index) in skills" :key='index'>{{ index }}. {{ data.skill }}</li>
      </ul>

      <div v-bind:style="{ backgroundColor: bgColor, width: bgWidth, height: bgHeight }"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      skills: [
        { "skill": "Vue.js" },
        { "skill": "Frontend Developer" }
      ],
      bgColor: 'yellow',
      bgWidth: '100%',
      bgHeight: '30px'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .alert {
    width: 100%;
    height: 30px;

    background-color: yellow;
  }
</style>
