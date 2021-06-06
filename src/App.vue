<template>
  <div id="app">
    <Header />
    <intro />
    <Video />
    <Case />
    <Task />
  </div>
</template>

<script>

import Header from "@/components/Header/Header";
import Intro from "@/components/Intro/Intro";
import Video from "@/components/Video/Video";
import Case from "@/components/Case/Case";
import Task from "@/components/Task/Task";
export default {
  name: 'App',
  components: {Task, Case, Video, Intro, Header},
}
</script>

<style>

</style>
