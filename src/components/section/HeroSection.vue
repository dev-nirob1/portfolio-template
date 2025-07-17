<template>
  <section class="hero">
    <div class="overlay">
      <div class="content">
        <h1>Hi, I'm <span class="accent">MD AL HASAN NIROB</span></h1>
        <p class="tagline">Front-End Developer specializing in React & Vue</p>
        <div class="buttons">
          <a href="#contact" class="btn">Contact Me</a>
          <a href="#" class="btn outline" download>Download CV</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  background: url('https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?auto=format&fit=crop&w=1650&q=80') 
    center/cover no-repeat fixed;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  color: #C5C6C7;
}

.overlay {
  background: rgba(31, 40, 51, 0.85); /* #1F2833 with transparency */
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.content {
  text-align: center;
  max-width: 700px;
}

.accent {
  color: #66FCF1;
}

.tagline {
  font-size: 1.2rem;
  margin-top: 1rem;
  color: #C5C6C7;
}

.buttons {
  margin-top: 2rem;
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  justify-content: center;
}

.btn {
  padding: 0.75rem 1.5rem;
  background-color: #66FCF1;
  color: #1F2833;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  transition: background 0.3s ease;
  text-decoration: none;
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
