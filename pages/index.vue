<template>
  <div>
  <div class="w3-top">
  <div class="w3-bar w3-white w3-wide w3-padding">
    <a href="#home" class="w3-bar-item w3-button"><b>LT</b> Lantech Infocom</a>
    <!-- Float links to the right. Hide them on small screens -->
  </div>
</div>

<!-- Header -->
<!-- Page content -->
<div class="w3-content w3-padding" style="max-width:1564px">

  <!-- Project Section -->
  <div class="w3-container w3-padding-32" id="projects">
    <h1 class="w3-border-bottom w3-border-light-grey w3-padding-16">Innovative Tools Built With Latest Technologies</h1>
  </div>

  <div class="w3-row-padding w3-grayscale">
    <a href="/binary-translator">
    <div class="w3-col l3 m6 w3-margin-bottom">
      <h3>Binary Translator</h3>
      <p class="w3-opacity">Education</p>
      <p>An online translator to convert binary code into other major numbering systems.</p>
      <p><button class="w3-button w3-light-grey w3-block">Check tool</button></p>
    </div>
  </a>
    <div class="w3-col l3 m6 w3-margin-bottom">
      <h3>MD5 hash Generator</h3>
      <p class="w3-opacity">Security</p>
      <p>Generate md-5 hash easily with just one click of any given string.</p>
      <p><button class="w3-button w3-light-grey w3-block">Check tool</button></p>
    </div>
    <div class="w3-col l3 m6 w3-margin-bottom">
      <h3>SHA-1 Generator</h3>
      <p class="w3-opacity">Security</p>
      <p>Generate SHA hash easily with just one click of any given string.</p>
      <p><button class="w3-button w3-light-grey w3-block">Check tool</button></p>
    </div>
    <div class="w3-col l3 m6 w3-margin-bottom">
      <h3>Hexadecimal to Decimal</h3>
      <p class="w3-opacity">Numbers</p>
      <p>Convert base-16 hexadecimal numbers to base-10 decimal numbers with this tool.</p>
      <p><button class="w3-button w3-light-grey w3-block">Check tool</button></p>
    </div>
  </div>

  <!-- About Section -->
  <div class="w3-container w3-padding-32" id="about">
    <h3 class="w3-border-bottom w3-border-light-grey w3-padding-16">About Lantech Infocom Tools</h3>
    <p>Lantech infocom tools are developed using innovative and latest technologies for students and technology enthusiasts. All the tools and apps here are developed with the help of Node.js, Vue.js, Nuxt.js. Along with these three technologies, we use
      Python programming language to develop Machine learning and Deep learning conpect apps. All the tools and converters here are totally free for everyone and you can also directly either contact us or mail us if you are want code for any converter
      for an educational purpose.
    </p>
  </div>

  <!-- Contact Section -->
  <div class="w3-container w3-padding-32" id="contact">
    <h3 class="w3-border-bottom w3-border-light-grey w3-padding-16">Contact</h3>
    <p>Lets get in touch and talk about your next project.</p>
    <form v-if="showform" target="_blank">
      <input class="w3-input w3-border" type="text" placeholder="Name" required name="Name">
      <input class="w3-input w3-section w3-border" type="text" placeholder="Email" required name="Email">
      <input class="w3-input w3-section w3-border" type="text" placeholder="Subject" required name="Subject">
      <input class="w3-input w3-section w3-border" type="text" placeholder="Comment" required name="Comment">
      <button @click="showthank()" class="w3-button w3-black w3-section" type="button">
        <i class="fa fa-paper-plane"></i> SEND MESSAGE
      </button>
    </form>
    <form v-if="showthankyou">
      <h1 style="color: green">Thanks for contacting us. We will be in touch.</h1>
    </form>
  </div>

</div>


<!-- Footer -->
<footer class="w3-center w3-black w3-padding-16">
  <p class="w3-text-green">© 2023 Lantech Infocom</p>
</footer>
</div>
</template>

<script>
export default {
  name: 'IndexPage',
  data(){
    return {
      showthankyou: false,
      showform: true
    }
  },
  methods: {
    showthank(){
      this.showthankyou = true;
      this.showform = false;
    }
  }
}
</script>
