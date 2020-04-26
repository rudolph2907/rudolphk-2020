<template>
  <div class="container has-padding-30">
    <h1 class="header is-size-5" style="display: inline-block;">
      01. Contact
    </h1>
    <div class="is-size-6 has-margin-top-30 content">
      <p>
        If you looking for help on any of your projects or want to start a new
        project. <strong>Please feel free to contact me:</strong>
      </p>
      <p>
        <strong>Email:</strong>
        <a :href="mailto">{{ email }}</a>
      </p>
      <p>
        <strong>Phone:</strong>
        <a :href="tel">{{ phone }}</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  computed: {
    email() {
      return 'rudolph.koegelenberg@gmail.com'
    },
    mailto() {
      return `mailto:${this.email}`
    },
    phone() {
      return '+27 82 928 7082'
    },
    tel() {
      return `tel:+27829287082`
    }
  },
  data() {
    return {
      years: new Date().getFullYear() - 2004
    }
  },
  head: {
    title:
      'Rudolph K - Full Stack Developer, Tech Consultant, Product Manager, Business Owner, Entrepreneur, Freelancer',
    description:
      'My name is Rudolph Koegelenberg. I am a Full Stack Developer, Tech Consultant, Product Manager, Business Owner, Entrepreneur, Freelancer'
  }
}
</script>
