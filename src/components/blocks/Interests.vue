<template>
<div>
    <b-container>
    <p :style="myContainer"> Things I enjoy outside coding :)</p>
    <p>I like to play the oboe.<br>
    I am in one of my school's orchestras and I am really addicted to coffee.<br>
    I have several methods of brewing coffee; my favorite is doing a pourover with the chemex<br>
    And my favorite coffee is usually a light roast from either Ethipoia or Panama<br>
    I have a softspot for videogames and I collect mechanical keyboards.</p>
    <p> Plans for this site is to add a blog component, and go more indepth into all things coffee.</p>
    </b-container>

</div>
</template>

<script>
export default {
  data () {
    return {
      myContainerStyle: {
        alignItems: 'left'
      }
    }
  }
}
</script>

<style scoped>
  div{
    padding: 20px;
  }
   p{
    color:white;
    font-family: monospace;
   }
</style>
