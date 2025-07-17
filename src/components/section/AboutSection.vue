<template>
  <section class="about">
    <div class="container">
      <div class="image">
        <img src="https://images.unsplash.com/photo-1603415526960-f7e0328a3bb2?auto=format&fit=crop&w=800&q=80" alt="Nirob's Photo" />
      </div>
      <div class="info">
        <h2>About Me</h2>
        <p>
          I'm <span class="highlight">MD AL HASAN NIROB</span>, a passionate front-end developer with expertise in
          <strong>React.js</strong>, <strong>Vue.js</strong>, and modern web tools. I build beautiful, responsive, and fast websites that solve real-world problems.
        </p>
        <ul class="highlights">
          <li>💡 Creative problem solver</li>
          <li>🚀 Focused on performance & UX</li>
          <li>🛠 Skilled in Firebase, Git, and APIs</li>
          <li>📚 Always learning & improving</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped>
.about {
  padding: 4rem 2rem;
  background-color: #1F2833;
  color: #C5C6C7;
}

.container {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
}

.image {
  flex: 1 1 300px;
  text-align: center;
}

.image img {
  max-width: 100%;
  border-radius: 10px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
}

.info {
  flex: 1 1 500px;
}

h2 {
  color: #66FCF1;
  margin-bottom: 1rem;
}

.highlight {
  color: #66FCF1;
  font-weight: bold;
}

.highlights {
  margin-top: 1.5rem;
  list-style: none;
  padding: 0;
}

.highlights li {
  margin-bottom: 0.5rem;
  font-size: 1rem;
  line-height: 1.6;
}
</style>
