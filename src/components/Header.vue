<template>
    <div :style="navPadding">
        <b-navbar variant='faded' type='light'>
            <b-navbar-brand tag='h1' id='head' class='mb-0'>Charles Carlson</b-navbar-brand>
        <b-navbar-nav class="ml-auto">
            <b-nav-text :style="myStyle">carlson.charles20@gmail.com</b-nav-text>
        </b-navbar-nav>
        </b-navbar>
    </div>
</template>

<script>
export default {
  data () {
    return {
      myStyle: {
        color: 'white',
        fontFamily: 'monospace'
      },
      navPadding: {
        padding: '15px',
        marginBottom: '5px'
      }
    }
  }
}
</script>

<style scoped>
div{
    background-color:#252526;
}
#head{
    font-family: monospace;
    color: white;
}
</style>
