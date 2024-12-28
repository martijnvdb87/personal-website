<script setup lang="ts">
import Label from '@/components/Label.vue';

const props = withDefaults(defineProps<{
  showAll?: boolean,
  labels?: string[]
}>(), {
  labels: () => []
});

const labels = [
  'PHP',
  'Laravel',
  'Javascript',
  'Typescript',
  'React',
  'Vue',
  'Svelte',
  'Web Components',
  'SQL',
  'PostgreSQL',
  'MySQL',
  'MongoDB',
  'Redis',
  'Memcached',
  'C# .NET',
  'HTML',
  'CSS',
  'SEO',
  'UI/UX',
  'Git',
  'REST API',
  'SOAP',
  'OpenID Connect',
  'SAML',
  'OAuth',
  'Wordpress',
  'Moodle',
  'Docker',
  'CI/CD',
  'FHIR',
];

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
