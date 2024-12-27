<script setup lang="ts">
import Segment from '@/components/Segment.vue';
</script>

<template>
  <div class="education">
    <div class="container">
      <section class="columns">
        <div class="columns__column">
          <Segment title="Microsoft Certificate | Programming in C# (MOC20483)" subtitle="September 2021 – December 2021 | Utrecht, The Netherlands (Hybrid)">
            <ul>
              <li>C# Fundamentals</li>
              <li>C# Object Programming</li>
              <li>C# .NET Developer</li>
            </ul>
          </Segment>
          <Segment title="LOI | HBO Communication & Multimediadesign" subtitle="2006 – 2012 | Leiderdorp, The Netherlands (Remote) | Did not finish">
          </Segment>
          <Segment title="Avans University of Applied Sciences | HBO Informatica" subtitle="2005 – 2006 | ’s-Hertogenbosch, The Netherlands | Did not finish"></Segment>
          <Segment title="Elde College | HAVO Nature & Technic (+ Informatica)" subtitle="2000 – 2005 | Schijndel, The Netherlands"></Segment>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped lang="scss">
.education {
  .container {
    padding: 1.5rem;
  }

  .columns__column {
    ul {
      font-size: 0.9375rem;
      margin: 0;
  
      li {
        margin-bottom: 0.25rem;
  
        strong {
          color: var(--blue-400);
          font-weight: 500;
        }
  
        &::marker {
          color: var(--blue-400);
        }
      }
    }
    
    p,
    ul {
      margin-bottom: 2rem;
    }
  }
}
</style>
