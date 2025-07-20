<script setup>
import BaseParagraph from '../Elements/BaseParagraph.vue';
import BaseTitle from '../Elements/BaseTitle.vue';

const skills = [
  { name: 'HTML5', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg' },
  { name: 'CSS3', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg' },
  { name: 'JavaScript', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg' },
  { name: 'React', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg' },
  { name: 'Vue', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg' },
  { name: 'Firebase', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg' },
  { name: 'Git', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg' },
  { name: 'Node.js', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg' },
  { name: 'Vite', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vite/vite-original.svg' },
]
</script>
<template>
  <section id="skills" class="skills">
    <div class="container">
      <BaseTitle class="mb-1 text-secondary">My Skills & Tools</BaseTitle>
      <BaseParagraph>
        I specialize in crafting responsive web applications using modern frontend frameworks like <strong>React</strong> and <strong>Vue</strong>. My experience also includes tools like <strong>Firebase</strong>, <strong>Node.js</strong>, and <strong>Git</strong> for full-stack development and collaboration.
      </BaseParagraph>

      <div class="marquee">
        <div class="marquee-content">
          <div v-for="skill in skills" :key="skill.name" class="skill">
            <img :src="skill.icon" :alt="skill.name" />
            <p>{{ skill.name }}</p>
          </div>
          <!-- Repeat for seamless scroll -->
          <div v-for="skill in skills" :key="`${skill.name}-clone`" class="skill">
            <img :src="skill.icon" :alt="skill.name" />
            <p>{{ skill.name }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.skills {
  padding: 3.75rem 0;
  text-align: center;
}

.skills p {
  max-width: 100%;
  margin: 0 auto 2.5rem;
}

.marquee {
  overflow: hidden;
  position: relative;
  width: 100%;
}
.marquee-content {
  display: flex;
  width: max-content;
  animation: scroll 30s linear infinite;
  gap: 3rem;
}
.skill {
  display: flex;
  flex-direction: column;
  align-items: center;
  min-width: 100px;
}

.skill img {
  width: 60px;
  height: 60px;
  object-fit: contain;
  margin-bottom: 0.5rem;
  transition: transform 0.3s ease;
}

.skill img:hover {
  transform: scale(1.2);
}
.skill p {
  font-size: 0.85rem;
  font-weight: 700;
}

@keyframes scroll {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-50%);
  }
}

@media (min-width:768px){
  .skills p {
  max-width: 700px;
}
}
</style>
