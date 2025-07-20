<template>
  <footer class="footer">
    <div class="container">
      <div class="flex justify-between align-center">
        <p>© 2025 Tech<span>Bondhu</span>. All rights reserved.</p>
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
  border-top: 1px solid var(--alternative-color);
  padding: 1rem;
  text-align: center;
}
.footer p span{
  color: var(--secondary-color);
}
.footer .flex {
  flex-direction: column;
}
.footer .socials {
  display: flex;
  gap: 1.5rem;
}
.footer .socials a {
  color: var(--secondary-color);
  text-decoration: none;
  transition: all 0.3s ease-in-out;
}
.footer .socials a:hover{
  scale: 1.05;
}
@media (min-width: 768px){
  .footer .flex {
  flex-direction: row;
}
}
</style>
