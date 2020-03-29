<template>
<div>
    <b-jumbotron container-fluid :style="jumbostyle">
        <template v-slot:header><span style="color:#569cd6">var</span> <span style="color:#DCDCAA">Experience</span> = ()<span style="color:#569cd6">=></span>{</template>

        <template v-slot:lead :style="leadStyle">
        <span style="color:#4EC9B0">console</span>.<span style="color:#DCDCAA">log</span>(<span style="color:#ce9178">"I have interned as both IT and full-stack engineer.<br>
         I have worked in both BIM/CAD and Fintech respectively<br>
         My primary focus is web development specifically with backend"</span>);<br>
        </template>
        };<br>
        <b-button id="linkedIn" href="https://www.linkedin.com/in/charles-carlson/">LinkedIn</b-button>
    </b-jumbotron>
</div>
</template>

<script>
export default {
  data () {
    return {
      jumbostyle: {
        backgroundColor: '#1e1e1e',
        color: 'white',
        fontFamily: 'monospace'
      }
    }
  }
}
</script>

<style scoped>
    #linkedIn{
        margin-top: 20px;
    }
    .display-3{
        font-size: 16px;
    }
    .lead{
        font-size:  16px;
    }
   p{
    color:white;
    font-family: monospace;
   }
</style>
