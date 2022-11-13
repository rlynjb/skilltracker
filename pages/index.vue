<template>
<div class="index-page">
  <header class="intro">
    Skill Tracker
  </header>

  <div class="dsa">
    <div class="dsa-card">
      <b>Data Structures and Algorithms (Coding)</b>
      <ul>
        <li>Sorting</li>
        <li>Recursion</li>
        <li>Trees</li>
        <li>Graphs</li>
        <li>Dynamin Programming</li>
      </ul>
    </div>
    <dsa-card />
  </div>

  <div class="latest">
    <div class="latest-card">
      <b>Front-end Domain</b>
      <ul>
        <li>JavaScript Language and Libraries</li>
        <li>UI and DOM</li>
        <li>Front-end System Design</li>
        <li>Patterns, Tools, and Technique</li>
      </ul>
    </div>
    <latest-card />
  </div>

  <div class="projects">
    <div class="project-card">
      <b>System Design</b>
      <ul>
        <li>Online Processing Systems</li>
        <li>Batch Processing Systems</li>
        <li>Stream Processing Systems</li>
      </ul>
    </div>
    <project-card />
    <project-card />
  </div>
</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  data() {
    return {
      dsa: [],
      latest: [],
      projects: [],
    }
  },
})
</script>

<style scoped lang="postcss">
.index-page {
  @apply grid grid-cols-12 p-12 gap-4;
}
.intro,
.projects,
.latest,
.dsa {
  @apply col-span-12 grid grid-cols-12 gap-4;
  min-height: 10em;
}
.intro {

}
.dsa-card {
  @apply col-span-12;
}
.latest-card {
  @apply col-span-12;
}
.project-card {
  @apply col-span-12;
}
</style>