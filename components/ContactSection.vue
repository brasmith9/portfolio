<template>
  <section id="contact" class="contact section contact-me">
    <h1 class="section__title">Contact Me</h1>
    <p class="section__subtitle">Get in Touch</p>
    <article class="mycontainer">
      <form class="contact-me__form" @submit.prevent="handleSubmit">
        <section class="form-element">
          <label for="name">Name</label>
          <input id="name" v-model="formData.name" type="text" required />
        </section>
        <section class="form-element">
          <label for="email">E-mail</label>
          <input id="email" v-model="formData.email" type="email" required />
        </section>
        <section class="form-element">
          <label for="message">Message</label>
          <textarea id="message" v-model="formData.message" required></textarea>
        </section>
        <div class="btn_grp form-group my-4 w-100">
          <button title="Send Message" type="submit" class="btn btn--primary send--btn">
            Send
          </button>
        </div>
      </form>
    </article>
  </section>
</template>

<script>
import emailjs from '@emailjs/browser';
import Swal from 'sweetalert2';
import { onMounted, ref } from 'vue';
export default {
  name: 'ContactSection',
  setup() {
    const formData = ref({
      name: '',
      email: '',
      message: ''
    });
    onMounted(() => {
      // eslint-disable-next-line import/no-named-as-default-member
      emailjs.init(process.env.EMAIL_KEY);
    });
    const handleSubmit = () => {
      const { name, message, email } = ({ ...formData.value });
      // eslint-disable-next-line import/no-named-as-default-member
      emailjs.send(
        process.env.EMAIL_SERVICE,
        process.env.EMAIL_TEMPLATE,
        {
          to_name: 'Isaac',
          from_name: name,
          email,
          message
        },
        process.env.EMAIL_KEY
      ).then((res) => {
        Swal.fire({
          title: 'Sent',
          icon: 'success',
          text: "Thank you for reaching out🤝, I'll be in touch."
        });
      }).catch(() => {
        Swal.fire({
          title: 'Error',
          icon: 'error',
          text: 'Could not send email. Try again later.'
        });
      });
    }

    return {
      handleSubmit,
      formData
    }
  }
}
</script>