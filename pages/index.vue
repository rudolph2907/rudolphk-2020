<template>
  <div class="container has-padding-30">
    <span class="header is-size-5">
      01. About Me
    </span>
    <div class="is-uppercase is-size-3 has-margin-top-30">
      My name is Rudolph Koegelenberg.<br />I am a Full Stack Developer, Tech
      Consultant, Product Manager, Business Owner, Entrepreneur, Maker,
      Bootstrapper, Freelancer
    </div>
    <div class="is-size-6 has-margin-top-30 content">
      <p>
        Yes, that is a lot of titles, but I do fill them somewhere during the
        day.
      </p>
      <p>
        Web development and everything technology related is my passion,
        together with the outdoors, mountain biking, travelling and CrossFit.
      </p>
      <p>
        Ex-Technical Director in one of South Africa's leading digital agencies.
      </p>
      <p>
        Currently freelancing and owner of a digital consultancy, Nailed
        Digital, where we develop and optimize websites and web applications. We
        also provide add-on services like web consultancy, web analytics, SEO,
        email marketing and digital training.
      </p>
      <p>
        In my over {{ years }} years of experience, I worked with a range of
        different technologies and all types of businesses, for example
        financial institutions, alcohol brands, online gaming brands and retail
        brands. Have a look at my LinkedIn page for a detailed timeline of my
        work experience. I am a full-stack developer, which means I am
        comfortable working with both front-end and back-end technologies.
      </p>
    </div>
    <span class="header is-size-5">
      02. Tech Stack
    </span>
    <div class="is-size-6 has-margin-top-30 content">
      <p>
        I always make sure I stay up to date with the latest technologies and
        use the right technology for the right project:
      </p>
      <div class="is-uppercase is-size-7">
        ASP.NET Core / ServiceStack.NET
        <progress class="progress" value="80" max="100"></progress>
        Node.js / Express.js
        <progress class="progress" value="80" max="100"></progress>
      </div>
      <div class="is-uppercase is-size-7 has-margin-top-30">
        WordPress CMS (PHP)
        <progress class="progress is-primary" value="90" max="100"></progress>
        Umbraco CMS (.NET)
        <progress class="progress is-primary" value="80" max="100"></progress>
      </div>
      <div class="is-uppercase is-size-7 has-margin-top-30">
        HTML
        <progress class="progress is-danger" value="100" max="100"></progress>
        CSS3 / SASS - Bootstrap / Bulma / Tailwind CSS
        <progress class="progress is-danger" value="90" max="100"></progress>
        JavaScript
        <progress class="progress is-danger" value="80" max="100"></progress>
        Vue.js / Nuxt.js - Vuetify / Buefy
        <progress class="progress is-danger" value="90" max="100"></progress>
      </div>
      <div class="is-uppercase is-size-7 has-margin-top-30">
        Tech Consulting
        <progress class="progress is-info" value="70" max="100"></progress>
        Product Management
        <progress class="progress is-info" value="60" max="100"></progress>
        Project Management - JIRA/Trello
        <progress class="progress is-info" value="70" max="100"></progress>
      </div>
      <div class="is-uppercase is-size-7 has-margin-top-30">
        Git
        <progress class="progress is-warning" value="80" max="100"></progress>
        MS SQL / Postgress / MySQL / MongoDB
        <progress class="progress is-warning" value="70" max="100"></progress>
        Server Management / DevOps / AWS
        <progress class="progress is-warning" value="70" max="100"></progress>
      </div>
    </div>
    <span class="header is-size-5">
      03. Experience &amp; Qualifications
    </span>
    <div class="is-size-6 has-margin-top-30 content">
      <p>
        Best to view my qualifications and experience on my
        <a
          href="https://www.linkedin.com/in/rudolphkoegelenberg/"
          target="_blank"
          >LinkedIn page</a
        >.
      </p>
      <p>
        I am have also obtained my MCSD (Microsoft Certified Solutions
        Developer), Google Analytics, Individual Qualification and CrossFit L1
        Trainer Certificate in 2013.
      </p>
      <p>
        I have also been a code mentor since 2014 on CodeMentor.io and
        HackHands.
      </p>
      <p>
        Please <nuxt-link to="contact">contact me</nuxt-link> if you would like
        to setup a meeting to discuss a potential new project or need help
        troubleshooting an issue. Or alternatively you can book as session using
        <a
          href="https://www.codementor.io/@rudolphk?utm_source=github&utm_medium=button&utm_term=rudolphk&utm_campaign=github"
          >CodeMentor.io</a
        >
      </p>
    </div>
    <span class="header is-size-5">
      04. My Services
    </span>
    <div class="is-size-6 has-margin-top-30 content">
      <ul>
        <li>Website / Web Application Development</li>
        <li>Web/Tech Consulting</li>
        <li>Development Troubleshooting</li>
        <li>Training</li>
        <li>Product Management</li>
        <li>Prototyping for Startups</li>
      </ul>
    </div>
  </div>
</template>

<script>
import Progress from '~/components/Progress.vue'

export default {
  name: 'Home',
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
