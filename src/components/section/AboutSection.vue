<script setup>
import BaseImage from '../Elements/BaseImage.vue';
import BaseParagraph from '../Elements/BaseParagraph.vue';
import BaseTitle from '../Elements/BaseTitle.vue';
import ListItem from '../Elements/ListItem.vue';


</script>

<template>
  <section class="about bg-primary">
    <div class="container medium-2 gap-2 align-center">
              <!-- about us content  -->
      <div>
       <BaseTitle class="text-secondary">About Me</BaseTitle>
        <BaseParagraph>
          I'm <span class="highlight">MD AL HASAN NIROB</span>, a passionate front-end developer with expertise in
          <strong>React.js</strong>, <strong>Vue.js</strong>, and modern web tools. I build beautiful, responsive, and fast websites that solve real-world problems.
        </BaseParagraph>
        <ul class="highlights">
          <ListItem>Creative problem solver</ListItem>
          <ListItem>Focused on performance & UX</ListItem>
          <ListItem>Skilled in Firebase, Git, and APIs</ListItem>
          <ListItem>Always learning & improving</ListItem>
        </ul>
      </div>
      <!-- img container  -->
      <div class="about-image">
        <BaseImage image="https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?auto=format&fit=crop&w=1650&q=80" alt="image" />
      </div>


    </div>
  </section>
</template>

<style scoped>
.about {
  padding: 3.75rem 0;
  color: var(--alternative-color);
}
.about-image {
  height: 100%;
  width: 100%;
}
.about-image img {
  height: auto;
  width: 100%;
  object-fit: cover;
}
.about ul {
    list-style: none;
    padding: 0;
}
.about ul li {
  position: relative;
  padding-left: 1rem;
  margin-bottom: .25rem;
}
.about ul li::before {
  content: "✓";
  position: absolute;
  left: 0;
  color: var(--secondary-color);
}
.about .highlight {
    color: var(--secondary-color);
    font-weight: bold;
}
</style>