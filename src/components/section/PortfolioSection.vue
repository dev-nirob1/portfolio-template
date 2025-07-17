<template>
  <section class="projects">
    <div class="container">
      <h2>My Projects</h2>
      <div class="grid">
        <div v-for="project in projects" :key="project.title" class="card">
          <img :src="project.image" :alt="project.title" />
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
          <div class="buttons">
            <a :href="project.live" target="_blank" class="btn">Live</a>
            <a :href="project.code" target="_blank" class="btn outline">Code</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
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
    image: 'https://images.unsplash.com/photo-1586201375761-83865001e17c?auto=format&fit=crop&w=800&q=80',
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

<style scoped>
.projects {
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
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.card {
  background-color: #0B0C10;
  border-radius: 8px;
  padding: 1.5rem;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  transition: transform 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  width: 100%;
  height: 160px;
  object-fit: cover;
  border-radius: 6px;
  margin-bottom: 1rem;
}

.card h3 {
  color: #66FCF1;
  margin: 0.5rem 0;
  font-weight: 600;
}

.card p {
  flex-grow: 1;
  font-size: 0.95rem;
  line-height: 1.5;
  margin-bottom: 1.5rem;
}

.buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
}

.btn {
  padding: 0.5rem 1rem;
  background-color: #66FCF1;
  color: #1F2833;
  font-weight: bold;
  border-radius: 5px;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #45d5cb;
}

.btn.outline {
  background: transparent;
  color: #66FCF1;
  border: 2px solid #66FCF1;
}

.btn.outline:hover {
  background-color: #66FCF1;
  color: #1F2833;
}
</style>
