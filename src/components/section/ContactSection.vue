<script setup>
import BaseButton from '../Elements/BaseButton.vue';
import BaseParagraph from '../Elements/BaseParagraph.vue';
import BaseTextArea from '../Elements/BaseTextArea.vue';
import BaseTitle from '../Elements/BaseTitle.vue';
import InputField from '../Elements/InputField.vue';
import SubTitle from '../Elements/SubTitle.vue';


</script>

<template>
  <section class="contact">
    <div class="container">
      <BaseTitle class="text-center mb-2 text-secondary">Contact Me</BaseTitle>
      <div class="medium-2 gap-2">

        <div class="contact-info">
          <SubTitle>Let's Discuss</SubTitle>
          <BaseParagraph>Have a question or want to discuss a project? Feel free to contact me using the information below:</BaseParagraph>
          <ul>
            <li>
             <i class="fa-solid fa-envelope fa-3x"></i>
              <div>
                <SubTitle>Email</SubTitle>
              <BaseParagraph>hello@yourportfolio.com</BaseParagraph>
              </div>
            </li>
            <li>
             <i class="fa-solid fa-phone fa-3x"></i>
              <div>
                <SubTitle>Phone</SubTitle>
              <BaseParagraph>+1 (555) 123-4567</BaseParagraph>
              </div>
            </li>
            <li>
             <i class="fa-solid fa-location-dot fa-3x"></i>
              <div>
                <SubTitle>Address</SubTitle>
              <BaseParagraph>Creative District, Suite 456</BaseParagraph>
              </div>
            </li>
          </ul>
        </div>

        <div class="form">
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
                <InputField type="text" placeholder="Subject" />
              </div>
              <div>
                <label for="message"></label>
                <BaseTextArea rows="6" id="message" placeholder="Enter Message..."></BaseTextArea>
              </div>
              <BaseButton class="bg-secondary">Send Message</BaseButton>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.contact {
  padding: 3.75rem 0;
  background-color: var(--primary-color);
  color: var(--alternative-color);
}
.contact ul {
  padding: 0;
  margin: 0;
  list-style: none;
}
.contact ul i{
  color: var(--secondary-color);
}
.contact ul li {
  display: flex;
  align-items: start;
  gap: 1rem;
  margin-top: 2rem;
}
.contact ul li p{
 margin: 0;
}
input,
select,
textarea {
  padding: 1rem;
  margin: 0;
  border: 1px solid var(--alternative-color);
  color: var(--alternative-color);
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