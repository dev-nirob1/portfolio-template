<template>
  <footer class="footer">
    <div class="container">
      <div class="flex justify-between align-center">
        <p>© 2025 All rights reserved.</p>
      <div class="socials">
        <a href="https://github.com/" target="_blank">
          <i class="fa-brands fa-github fa-2x"></i>
        </a>
        <a href="https://linkedin.com/in/" target="_blank">
          <i class="fa-brands fa-linkedin fa-2x"></i>
        </a>
        <a href="mailto:youremail@example.com">
           <i class="fa-solid fa-envelope fa-2x"></i>
        </a>
      </div>
      </div>
    </div>
  </footer>
</template>


<style scoped>
.footer {
  background-color: rgb(from var(--primary-color)r g b / 95%);
  color: var(--alternative-color);
  padding: 1rem;
  text-align: center;
}
.footer .flex {
  flex-direction: column;
}
.socials {
  display: flex;
  gap: 1.5rem;
}
.socials a {
  color: #66FCF1;
  text-decoration: none;
  transition: color 0.3s ease;
}

.socials a:hover {
  color: #45d5cb;
}
@media (min-width: 768px){
  .footer .flex {
  flex-direction: row;
}
}
</style>
