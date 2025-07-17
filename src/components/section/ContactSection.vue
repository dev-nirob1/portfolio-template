<template>
  <section class="contact" id="contact">
    <div class="container">
      <h2>Contact Me</h2>
      <form @submit.prevent="handleSubmit" class="contact-form">
        <input v-model="name" type="text" placeholder="Your Name" required />
        <input v-model="email" type="email" placeholder="Your Email" required />
        <textarea v-model="message" placeholder="Your Message" rows="5" required></textarea>
        <button type="submit" class="btn">Send Message</button>
      </form>
      <div class="socials">
        <a href="https://github.com/yourusername" target="_blank" aria-label="GitHub">🐙 GitHub</a>
        <a href="https://linkedin.com/in/yourprofile" target="_blank" aria-label="LinkedIn">💼 LinkedIn</a>
        <a href="mailto:youremail@example.com" aria-label="Email">📧 Email</a>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const name = ref('')
const email = ref('')
const message = ref('')

const handleSubmit = () => {
  alert(`Thank you, ${name.value}! Your message has been sent.`)
  name.value = ''
  email.value = ''
  message.value = ''
}
</script>

<style scoped>
.contact {
  background-color: #1F2833;
  color: #C5C6C7;
  padding: 4rem 2rem;
  text-align: center;
}

.container {
  max-width: 600px;
  margin: auto;
}

h2 {
  color: #66FCF1;
  margin-bottom: 2rem;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

input,
textarea {
  padding: 0.75rem 1rem;
  border: none;
  border-radius: 6px;
  font-size: 1rem;
  background-color: #0B0C10;
  color: #C5C6C7;
  resize: vertical;
  transition: border 0.3s ease;
}

input:focus,
textarea:focus {
  outline: none;
  border: 2px solid #66FCF1;
}

.btn {
  padding: 0.75rem;
  background-color: #66FCF1;
  color: #1F2833;
  font-weight: bold;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #45d5cb;
}

.socials {
  margin-top: 2rem;
  display: flex;
  justify-content: center;
  gap: 2rem;
  font-size: 1.25rem;
}

.socials a {
  color: #66FCF1;
  text-decoration: none;
  transition: color 0.3s ease;
}

.socials a:hover {
  color: #45d5cb;
}
</style>
