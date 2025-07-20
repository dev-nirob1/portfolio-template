<script setup>
import BaseParagraph from '../Elements/BaseParagraph.vue';
import HeroTitle from './../Elements/HeroTitle.vue'
</script>
<template>
  <section class="hero">
    <div class="overlay">
      <div class="content">
        <HeroTitle>Hi, I'm <span class="highlight">MD AL HASAN NIROB</span></HeroTitle>
        <BaseParagraph>Front-End Developer specializing in React & Vue</BaseParagraph>
        <div class="flex justify-center gap-1 flex-wrap mt-2">
          <a href="#contact" class="btn">Contact Me</a>
          <a href="#" class="btn outline" download>Download CV</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  background: url('https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?auto=format&fit=crop&w=1650&q=80') center/cover no-repeat fixed;
  min-height: 100vh;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  color: var(--alternative-color);
  padding: 5rem 0;
}

.hero .overlay {
  background: rgb(from var(--primary-color) r g b / 85%);
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.hero .content {
  max-width: 700px;
}

.hero .highlight {
  color: var(--secondary-color);
}

.hero p {
  font-size: 1.2rem;
}

.hero .btn {
  padding: 0.75rem 1.5rem;
  background-color: var(--secondary-color);
  color: var(--primary-color);
  transition: background 0.3s ease;
}

.hero .btn:hover {
  background-color: transparent;
  color: var(--secondary-color);
}

.hero .btn.outline {
  background: transparent;
  color: var(--secondary-color);
  border: 2px solid var(--secondary-color);
}

.hero .btn.outline:hover {
  background-color: var(--secondary-color);
  color: var(--primary-color);
}
</style>
