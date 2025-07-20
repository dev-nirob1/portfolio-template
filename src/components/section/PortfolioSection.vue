<script setup>
import BaseImage from '../Elements/BaseImage.vue';
import BaseParagraph from '../Elements/BaseParagraph.vue';
import BaseTitle from '../Elements/BaseTitle.vue';
import SubTitle from '../Elements/SubTitle.vue';

const projects = [
  {
    title: 'BlogExpress',
    description: 'A blog platform with role-based dashboards and Firebase Auth.',
    image: 'https://images.unsplash.com/photo-1521737604893-d14cc237f11d?auto=format&fit=crop&w=800&q=80',
    live: '#',
    code: '#'
  },
  {
    title: 'ToyStore',
    description: 'E-commerce website for kids toys with categories and reviews.',
    image: 'https://images.unsplash.com/photo-1521737604893-d14cc237f11d?auto=format&fit=crop&w=800&q=80',
    live: '#',
    code: '#'
  },
  {
    title: 'Accent Adept',
    description: 'Language learning platform with courses and payment integration.',
    image: 'https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=800&q=80',
    live: '#',
    code: '#'
  },
]
</script>
<template>
  <section id="projects" class="projects">
    <div class="container">
      <BaseTitle class="text-center mb-2">My Projects</BaseTitle>
      <div class="medium-2 large-3 gap-2">
        <div v-for="project in projects" :key="project.title" class="card">

          <BaseImage :image="project.image" :alt="project.title" />

          <div class="p-2">
            <SubTitle>{{ project.title }}</SubTitle>
            <BaseParagraph>{{ project.description }}</BaseParagraph>
            <div class="all-2 gap-1">
              <a :href="project.live" target="_blank" class="btn">Live</a>
              <a :href="project.code" target="_blank" class="btn outline">Code</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.projects {
  padding: 3.75rem 0;
}

.card {
  background-color: rgb(from var(--primary-color)r g b / 70%);
  border-radius: .75rem;
  box-shadow: 0 .25rem 10px rgb(from var(--alternative-color) r g b / 30%);
  transition: transform 0.3s ease;
}

.card:hover {
  transform: translateY(-.25rem);
}

.card img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: .75rem;
}
.card p {
  margin: .75rem 0 1.25rem 0;
}
.card .btn {
  padding: .5rem;
  background-color: var(--secondary-color);
  color: var(--primary-color);
  border: 2px solid var(--secondary-color);
}


.projects .btn:hover {
  background-color: transparent;
  color: var(--secondary-color);
}

.projects .btn.outline {
  background: transparent;
  color: var(--secondary-color);
}

.projects .btn.outline:hover {
  background-color: var(--secondary-color);
  color: var(--primary-color);
}
</style>
