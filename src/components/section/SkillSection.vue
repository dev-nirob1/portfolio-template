<template>
  <section class="skills">
    <div class="container">
      <h2>My Skills & Tools</h2>
      <div class="grid">
        <div v-for="skill in skills" :key="skill.name" class="skill">
          <img :src="skill.icon" :alt="skill.name" />
          <p>{{ skill.name }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
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

<style scoped>
.skills {
  background-color: #1F2833;
  color: #C5C6C7;
  padding: 4rem 2rem;
  text-align: center;
}

.container {
  max-width: 1100px;
  margin: auto;
}

h2 {
  color: #66FCF1;
  margin-bottom: 2rem;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
  gap: 2rem;
  align-items: center;
  justify-items: center;
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
  margin: 0;
  font-size: 0.9rem;
  font-weight: bold;
}
</style>
