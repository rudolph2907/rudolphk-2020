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
      <hr />
      <div class="has-text-centered">
        <h2 class="title is-4">Send a message</h2>
      </div>
      <form name="contact" method="POST" data-netlify="true">
        <div class="field is-horizontal">
          <div class="field-label is-normal">
            <label class="label">From</label>
          </div>
          <div class="field-body">
            <div class="field">
              <p class="control is-expanded">
                <input
                  name="name"
                  class="input"
                  type="text"
                  placeholder="Name"
                  required
                />
              </p>
            </div>
            <div class="field">
              <p class="control is-expanded">
                <input
                  class="input is-success"
                  name="email"
                  type="email"
                  placeholder="Email"
                  required
                  value="alex@smith.com"
                />
              </p>
            </div>
          </div>
        </div>

        <div class="field is-horizontal">
          <div class="field-label is-normal">
            <label class="label">Message</label>
          </div>
          <div class="field-body">
            <div class="field">
              <div class="control">
                <textarea
                  name="message"
                  class="textarea"
                  placeholder="Explain how I can help you"
                  required
                ></textarea>
              </div>
            </div>
          </div>
        </div>

        <div class="field is-horizontal">
          <div class="field-label">
            <!-- Left empty for spacing -->
          </div>
          <div class="field-body">
            <div class="field">
              <div class="control">
                <button class="button is-primary">
                  Send message
                </button>
              </div>
            </div>
          </div>
        </div>
      </form>
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
