<template lang="html">
<div class="dark-mode">
  <div class="w3-quarter">
    <h1 class="w3-text-green">Binary Translator</h1>
  </div>
  <div class="w3-container w3-padding-32" id="contact">
    <h3 class="w3-border-bottom w3-border-light-grey w3-padding-16">Contact</h3>
    <p>Binary Translator</p>
    <form target="_blank">
      <input class="w3-input w3-border" type="text" placeholder="Name" required name="Name">
      <input class="w3-input w3-section w3-border" type="text" placeholder="Email" required name="Email">
      <input class="w3-input w3-section w3-border" type="text" placeholder="Subject" required name="Subject">
      <input class="w3-input w3-section w3-border" type="text" placeholder="Comment" required name="Comment">
      <button class="w3-button w3-black w3-section" type="button">
        <i class="fa fa-paper-plane"></i> SEND MESSAGE
      </button>
    </form>
  </div>
</div>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
.dark-mode {
  background-color: black;
  color: white;
}

</style>
