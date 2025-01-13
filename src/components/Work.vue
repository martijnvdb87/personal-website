<script setup lang="ts">
import Segment from '@/components/Segment.vue';
import Link from '@/components/Link.vue';
import SegmentLead from './SegmentLead.vue';
import { Skill } from '@/enums/skill';
</script>

<template>
  <div class="work">
    <div class="container">
      <section class="columns">
        <div class="columns__column">
          <Segment title="Senior full-stack developer" content="Ksyos" subtitle="October 2022 - Present" href="https://www.ksyos.nl/" target="_blank">
            <ul>
              <li><SegmentLead>Authorization system</SegmentLead> Added a new authorization system to give more fine-grained access control for healthcare professionals and Ksyos employees throughout whole the medical platform</li>
              <li><SegmentLead>Patient privacy</SegmentLead> Made the medical platform comform to the <Link href="https://www.nen.nl/nen-7513-2024-nl-329182" target="_blank">NEN 7513</Link> patient privacy standard, to ensure patients get full insight into whom is accessing their medical data by implementing developer friendly and scaleable access logging throughout the platform</li>
              <li><SegmentLead>SAML SSO</SegmentLead> Set up multiple SAML SSO's to give healthcare professionals seemless access to partner platforms</li>
              <li><SegmentLead>Medical services</SegmentLead> Succesfully developed and maintained medical services with tight deadlines</li>
              <li><SegmentLead>Testing</SegmentLead> Added a testing utility function to create dummy users with specific permissions to simplify writing unit and integration tests</li>
            </ul>
            <Skills :labels="[Skill.Javascript, Skill.Typescript, Skill.Sql, Skill.PostgreSQL, Skill.Html, Skill.Css, Skill.React, Skill.RestApi, Skill.Saml, Skill.Git, Skill.Fhir]" />
          </Segment>
          <Segment title="Lead full-stack developer" content="SkillsTown" subtitle="March 2019 - September 2022" href="https://skillstown.com/" target="_blank">
            <ul>
              <li><SegmentLead>Interoperability</SegmentLead> Implemented <Link href="https://en.wikipedia.org/wiki/Learning_Tools_Interoperability" target="_blank">LTI 1.3</Link> which allowed us to contract the biggest customer in the history of the company</li>
              <li><SegmentLead>SAML SSO</SegmentLead> Automated the <Link href="https://en.wikipedia.org/wiki/Security_Assertion_Markup_Language" target="_blank">SAML SSO</Link> process which reduced the development time from 8 hours to 10 minutes</li>
              <li><SegmentLead>OpenID Connect SSO</SegmentLead> Added <Link href="https://en.wikipedia.org/wiki/OpenID#OpenID_Connect_(OIDC)" target="_blank">OpenID Connect</Link> capability to the platform</li>
              <li><SegmentLead>Frontend</SegmentLead> Rewrote an unstable <Link href="https://svelte.dev/" target="_blank">Svelte</Link> application to a stable <Link href="https://reactjs.org/" target="_blank">React</Link> one</li>
              <li><SegmentLead>Security</SegmentLead> Located and fixed mulitple <Link href="https://en.wikipedia.org/wiki/Cross-site_scripting" target="_blank">XSS vulnerabilities</Link></li>
              <li><SegmentLead>Upgrade</SegmentLead> Upgraded the legacy platform from PHP 5 to 7</li>
              <li><SegmentLead>LRS</SegmentLead> Implemented full <Link href="https://en.wikipedia.org/wiki/Learning_Record_Store" target="_blank">LRS</Link> capability in two existing platforms (PHP & C# .NET)</li>
              <li><SegmentLead>WooCommerce</SegmentLead> Automated the ordering process between the learning platform and the <Link href="https://woocommerce.com/" target="_blank">WooCommerce</Link> webshop</li>
            </ul>
            <Skills :labels="[Skill.Php, Skill.Javascript, Skill.Typescript, Skill.CSharpDorNet, Skill.Sql, Skill.MySQL, Skill.MongoDB, Skill.Html, Skill.Css, Skill.Laravel, Skill.React, Skill.Vue, Skill.Svelte, Skill.RestApi, Skill.Git, Skill.OpenIdConnect, Skill.Saml, Skill.OAuth, Skill.Wordpress, Skill.Moodle]" />
          </Segment>
          <Segment title="Owner & full-stack developer" content="Monversa Web Development" subtitle="July 2013 - February 2019" href="https://web.archive.org/web/20180831062310/https://monversa.nl/" target="_blank">
            <ul>
              <li><SegmentLead>CMS</SegmentLead> Designed and developed my own Content Management System</li>
              <li><SegmentLead>Servers</SegmentLead> Setting up and maintaining Centos/Ubuntu, Apache/Nginx, PHP and MySQL servers</li>
              <li><SegmentLead>Wordpress</SegmentLead> Built multiple Wordpress sites for small local businesses</li>
              <li><SegmentLead>Plugins</SegmentLead> Created several custom Wordpress webshop plugins</li>
            </ul>
            <Skills :labels="[Skill.Php, Skill.Javascript, Skill.Sql, Skill.MySQL, Skill.Html, Skill.Css, Skill.UiUx, Skill.RestApi, Skill.Git, Skill.Wordpress]" />
          </Segment>
          <Segment title="Full-stack developer" content="Innowijs" subtitle="June 2018 - December 2018 (part-time)" href="https://innowijs.nl/" target="_blank">
            <ul>
              <li><SegmentLead>Interactive tablet tour </SegmentLead> Developed an interactive tablet tour for children visting a museum located in The Hague</li>
              <li><SegmentLead>Online courses </SegmentLead> Added custom interactivity to <Link href="https://articulate.com/360/storyline" target="_blank">Articulate Storline</Link> online courses</li>
              <li><SegmentLead>Moodle</SegmentLead> Designed and developed a modern <Link href="https://moodle.org/" target="_blank">Moodle</Link> theme</li>
              <li><SegmentLead>Library plugin</SegmentLead> Created a custom online libary Wordpress plugin</li>
              <li><SegmentLead>Charity site</SegmentLead> Built a Wordpress site for a charity organisation</li>
            </ul>
            <Skills :labels="[Skill.Php, Skill.Javascript, Skill.Sql, Skill.MySQL, Skill.Html, Skill.Css, Skill.UiUx, Skill.RestApi, Skill.Wordpress, Skill.Moodle]" />
          </Segment>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped lang="scss">
.work {
  .container {
    padding: 1.5rem;
  }

  .columns__column {
    ul {
      font-size: 0.9375rem;
      margin: 0;

      li {
        margin-bottom: 0.25rem;

        &::marker {
          color: var(--blue-400);
        }
      }
    }
    
    p,
    ul {
      margin-bottom: 1rem;
    }
  }
}
</style>
