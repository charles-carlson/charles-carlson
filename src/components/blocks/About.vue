<template>
    <div>
        <b-container fluid="sm">
        <b-row>
        <b-col :style="containerStyle">
        <h1>README</h1>
        <p id='header'>##About Me<br></p>
        <p>
        Welcome to my website! Built with Vue.js<br>
        I am a driven software developer, with a passion for software design.<br>
        My main strengths are: Creativity, Adaptability, and Ambition<br></p>
        <p>
        Detail-oriented with a hard work ethic, I bring a toolset of knowledge<br>
        ranging from web development to software design.<br>
        Self-teaching and my education has provided me with the means<br>
        to be an efficient and detailed programmer<br></p>
        <p>
        From the age of 13 when I first built my own computer,<br>
        I knew I wanted to become enveloped in the computer science field.<br>
        </p>
        </b-col>
        <b-col :style="containerStyle2">
            <h1>Education</h1>
            <p id='header'>##School</p>
            <p>St. Olaf College, May 2020, Bachelor of Arts in Computer Science</p>
            <p id='header'>##GPA</p>
            <p>3.1/3.39</p>
            <p id='header'>##Coursework</p>
            <p>Hardware Design, Software Design, Algorithms and Data-structures,<br>
            Robotics, Mobile Computing, Parallel Distributed Computing,<br>
            Principles of Computer Science, Linear Algebra, Mathematical Reasoning, Capstone   </p>
        </b-col>
        </b-row>
        </b-container>
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
      },
      containerStyle: {
        borderStyle: 'solid',
        borderWidth: '15px'
      },
      containerStyle2: {
        borderStyle: 'solid',
        borderWidth: '15px',
        marginLeft: '10px'
      }
    }
  }
}
</script>

<style scoped>
#header{
    color:#569cd6
}
h1{
    font-family: monospace;
    color: white;
}
p{
    font-family: monospace;
    color: white;
}
</style>
