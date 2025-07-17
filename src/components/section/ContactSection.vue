<script setup>
import BaseButton from '../Elements/BaseButton.vue';
import BaseTextArea from '../Elements/BaseTextArea.vue';
import InputField from '../Elements/InputField.vue';


</script>

<template>
  <section class="form">
    <div class="container">
      <form>
          <div>
            <label for="name"></label>
            <InputField id="name" type="text" placeholder="Enter Your Name" />
          </div>
          <div>
            <label for="email"></label>
            <InputField id="email" type="email" placeholder="Enter Your Email" />
          </div>
          <div>
            <label for="phone"></label>
            <InputField type="tel" id="phone" placeholder="Enter Your Phone Number" />
          </div>
        <div class="mt-1">
          <label for="message"></label>
          <BaseTextArea rows="6" id="message" placeholder="Enter Message..."></BaseTextArea>
        </div>
        <BaseButton class="bg-secondary">GET A FREE SERVICE</BaseButton>
      </form>
    </div>
  </section>
</template>

<style scoped>
.form {
  padding: 3.75rem 0;
  background-color: var(--primary-color);
}

input,
select,
textarea {
  padding: 1.25rem;
  margin: 0;
  border: 1px solid var(--alternative-color);
  box-shadow: var(--box-shadow);
  margin-top: 1rem;
}

input:focus,
textarea:focus {
  outline: none;
}

input::placeholder,
textarea::placeholder,
select::placeholder {
  font-size: .9rem;
  color: var(--alternative-color);
}

.form .btn {
  padding: 1.25rem 2rem;
  margin: 1rem 0 0 0;
}

</style>