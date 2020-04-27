<template>
<div>
    <b-container fluid="sm" >
      <b-row>
        <b-col :style='colStyle'>
        <h1>Skills</h1>
        <ul id='ul1' :style="containerStyle">
            <li v-for="(item, index) in items" v-bind:key='item'>
                <span id='s1' style="color: #858585">{{index}}</span><span style="color: #6A9955">{{item.sentence}}</span>
            </li>
        </ul>
        </b-col>
      </b-row>
    </b-container>
</div>
</template>

<script>
// TODO: add underlines or add color to important keywords
export default {
  data () {
    return {
      items: [
        {sentence: '/*'},
        {sentence: 'My primary langauges are Python, Javascript/node.js, and C++'},
        {sentence: 'However, I enjoy trying new things. I have used Go and Dr.Racket for school and projects.'},
        {sentence: 'Frameworks I use the most are Vue.js and ExpressJS. I am also proficient with Django, Flask, and React-native'},
        {sentence: 'Along the way, I have picked up Docker and Kubernetes for my undergrad research and implemented alongside with AWS EKS'},
        {sentence: 'I like to tinker around with new technologies, and personally feel stateless enviroments'},
        {sentence: 'are the future for software development'},
        {sentence: '*/'}
      ],
      containerStyle: {
        border: '0 none',
        borderColor: '#252526',
        paddingLeft: '5px',
        paddingRight: '5px',
        paddingTop: '10px'
      },
      colStyle: {
        borderStyle: 'solid',
        borderWidth: '15px',
        marginTop: '10px'
      }
    }
  }
}
</script>

<style scoped>
#s1{
    margin-right: 25px;
}
h1{
    color:white;
    font-family: monospace;
}
p{
    color:white;
    font-family: monospace;
    margin-top: 10px;
    margin-bottom: 25px;
}
#ul1{
    display: inline-block;
    vertical-align: top;
    color:white;
    font-family: monospace;
    list-style-type: none;
}
#ul2{
    display: inline-block;
    vertical-align: top;
    color:white;
    font-family: monospace;
}
</style>
