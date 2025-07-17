<template>
  <footer class="footer">
    <div class="container">
      <p>© 2025 MD AL HASAN NIROB. All rights reserved.</p>
      <div class="socials">
        <a href="https://github.com/yourusername" target="_blank" aria-label="GitHub">🐙</a>
        <a href="https://linkedin.com/in/yourprofile" target="_blank" aria-label="LinkedIn">💼</a>
        <a href="mailto:youremail@example.com" aria-label="Email">📧</a>
      </div>
      <button class="back-to-top" @click="scrollTop" aria-label="Back to top">⬆️</button>
    </div>
  </footer>
</template>

<script setup>
const scrollTop = () => {
  window.scrollTo({ top: 0, behavior: 'smooth' })
}
</script>

<style scoped>
.footer {
  background-color: #0B0C10;
  color: #C5C6C7;
  padding: 1.5rem 2rem;
  text-align: center;
  position: relative;
}

.container {
  max-width: 1100px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

p {
  margin: 0;
  font-size: 0.9rem;
  flex-grow: 1;
  text-align: center;
}

.socials {
  display: flex;
  gap: 1.5rem;
  font-size: 1.5rem;
}

.socials a {
  color: #66FCF1;
  text-decoration: none;
  transition: color 0.3s ease;
}

.socials a:hover {
  color: #45d5cb;
}

.back-to-top {
  background: transparent;
  border: none;
  font-size: 1.5rem;
  cursor: pointer;
  color: #66FCF1;
  transition: color 0.3s ease;
}

.back-to-top:hover {
  color: #45d5cb;
}
</style>
