<template>
  <div class="skills">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key='index'>{{index}}. {{data.skill}}</li>
      </ul>

      <p v-if="skills.length >= 1">You have more than 1 skill</p>
      <p v-else>You have less than or equal to 1 skill</p>
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
      ]
    }
  },
  }
</script>

<style scoped>
  body {  
      background-color: #eeeeee;
    }
</style>
