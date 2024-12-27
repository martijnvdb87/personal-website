<script setup lang="ts">
import Segment from '@/components/Segment.vue';
import Link from '@/components/Link.vue';
</script>

<template>
  <div class="introduction">
    <Segment title="Introduction" icon="user">
      <p>
        I'm a <strong>self-taught senior full-stack developer</strong> from the Netherlands.
        I have been developing websites and webapps for <strong>more than 25 years</strong>.
        When I was 12 years old I became interested in programming and I turned it into my profession.
        I dedicate my free time to my personal projects.
        Currently I'm working on a drag-and-drop graphics design tool.
      </p>
    </Segment>
  </div>
</template>

<style scoped lang="scss">
  strong {
    font-weight: 575;
  }
</style>
