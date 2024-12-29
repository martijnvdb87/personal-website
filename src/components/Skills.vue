<script setup lang="ts">
import Label from '@/components/Label.vue';
import { Skill } from '@/enums/skill';

const props = withDefaults(defineProps<{
  showAll?: boolean,
  labels?: Skill[]
}>(), {
  labels: () => []
});

const labels = Object.values(Skill);

const validLabel = (label: string): boolean => {
  return props.labels.map(label => label.toLowerCase()).includes(label.toLowerCase());
}
</script>

<template>
  <div class="skills">
    <template v-for="label in labels">
      <Label v-if="validLabel(label) || props.showAll">{{label}}</Label>
    </template>
  </div>
</template>

<style scoped lang="scss">
.skills {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
  padding-top: 0.5rem;

  &::after {
    content: '';
    display: block;
    flex: 1 0 0;
  }
}
</style>
