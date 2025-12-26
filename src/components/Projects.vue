<script setup lang="ts">
import Segment from '@/components/Segment.vue';
import Link from '@/components/Link.vue';
import Skills from '@/components/Skills.vue';
import { Skill } from '@/enums/skill';
</script>

<template>
  <div class="projects">
    <div class="container">
      <section class="columns">
        <div class="columns__column">
          <Segment title="Type Vault" href="https://github.com/martijnvdb87/type-vault" target="_blank">
            <p>Type Vault is a TypeScript utility package that provides robust and validated types for common structured values like UUIDs, URLs, ISO date-times, hex colors, and more. It helps enforce correctness at runtime while maintaining strong typing at compile time. It is originally written in <Link href="https://github.com/martijnvdb87/type-vault" target="_blank">TypeScript</Link>, but it also has a <Link href="https://github.com/martijnvdb87/type-vault-php" target="_blank">PHP</Link> equivalent.</p>
            <Skills :labels="[Skill.Typescript, Skill.Php, Skill.Git]" />
          </Segment>
    
          <Segment title="OhMyBrush">
            <p>OhMyBrush is a Hungarian beauty blog which won the Cosmopolitan beauty blog of the year award in 2016. The Wordpress website used multiple themes over the years all desiged and developed by me. In 2014 it got nominated as best designed blog by Cosmopolitan.</p>
            <Skills :labels="[Skill.Php, Skill.Javascript, Skill.Html, Skill.Css, Skill.Git, Skill.Wordpress]" />
          </Segment>
    
          <Segment title="PHP CLI" href="https://github.com/martijnvdb87/php-cli" target="_blank">
            <p>The <Link href="https://github.com/martijnvdb87/php-cli" target="_blank">PHP CLI library</Link> helps you to create CLI applications quicky. The library can also be installed via <Link href="https://packagist.org/packages/martijnvdb/php-cli" target="_blank">Composer</Link>.</p>
            <Skills :labels="[Skill.Php, Skill.Git]" />
          </Segment>
    
          <Segment title="PHP Image Resize" href="https://github.com/martijnvdb87/php-image-resize" target="_blank">
            <p>This <Link href="https://github.com/martijnvdb87/php-image-resize" target="_blank">PHP Image Resize library</Link> allows you to resize and convert images to a different file format. The supported file types are JPG, PNG, GIF and WebP. The library can also be installed via <Link href="https://packagist.org/packages/martijnvdb/php-image-resize" target="_blank">Composer</Link></p>
            <Skills :labels="[Skill.Php, Skill.Git]" />
          </Segment>
          
          <Segment title="Wordpress Plugin Payhip Products" href="https://github.com/martijnvdb87/wordpress-plugin-payhip-products" target="_blank">
            <p>The <Link href="https://github.com/martijnvdb87/wordpress-plugin-payhip-products" target="_blank">Wordpress Payhip Products plugin</Link> will display a list of your Payhip products on your Wordpress website. It allows your visitors to buy your Payhip products directly from a Wordpress website.</p>
            <Skills :labels="[Skill.Php, Skill.Html, Skill.Javascript, Skill.Css, Skill.Git, Skill.Wordpress]" />
          </Segment>
    
          <Segment title="Wordpress Plugin Tools" href="https://github.com/martijnvdb87/wordpress-plugin-tools" target="_blank">
            <p>The <Link href="https://github.com/martijnvdb87/wordpress-plugin-tools" target="_blank">Wordpress Plugin Tools library</Link> was made to simplify the proces of creating custom post types and settings pages in Wordpress. The library can also be installed via <Link href="https://packagist.org/packages/martijnvdb/wordpress-plugin-tools" target="_blank">Composer</Link></p>
            <Skills :labels="[Skill.Php, Skill.Html, Skill.Javascript, Skill.Css, Skill.Git, Skill.Wordpress]" />
          </Segment>
    
          <Segment title="mRouter" href="https://github.com/martijnvdb87/mrouter" target="_blank">
            <p>A <Link href="https://github.com/martijnvdb87/mrouter" target="_blank">simple routing class</Link> for small projects build with PHP.</p>
            <Skills :labels="[Skill.Php, Skill.Git]" />
          </Segment>
    
          <Segment title="WYSIWYG Editor" href="https://github.com/martijnvdb87/wysiwyg-editor" target="_blank">
            <p>A simple jQuery <Link href="https://github.com/martijnvdb87/wysiwyg-editor" target="_blank">WYSIWYG editor</Link> based on the Medium.com editor.</p>
            <Skills :labels="[Skill.Javascript, Skill.JQuery, Skill.Html, Skill.Css, Skill.Git]" />
          </Segment>
    
          <Segment title="MagyarBlogok" href="https://web.archive.org/web/20181129093940/http://www.magyarblogok.hu/" target="_blank">
            <p>One of the biggest curated Hungarian blogging feed. <Link href="https://web.archive.org/web/20181129093940/http://www.magyarblogok.hu/" target="_blank">MagyarBlogok</Link> scapped over a hundred blogs and YouTube channels multiple times a day to get titles, URL's, thumbnails and descriptions of new posts and videos. The blogs were scrapped based on historical post activity frequency, so more active blogs would be scrapped more frequently.</p>
            <Skills :labels="[Skill.Php, Skill.Javascript, Skill.Sql, Skill.Html, Skill.Css, Skill.RestApi]" />
          </Segment>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped lang="scss">
.projects {
  .container {
    padding: 1.5rem;
  }
    
  .columns__column {
    p,
    ul {
      margin-bottom: 1rem;
    }
  }
  @media only screen and (min-width: 80rem) {
    .columns__column {
      display: flex;
      flex-wrap: wrap;
      gap: 0 3rem;

      > section {
        flex: 0 0 calc(50% - 1.5rem);
      }
    }
  }
}
</style>
