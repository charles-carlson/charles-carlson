<template>
<div>
  <b-container fluid="sm" :style="containerStyle">
    <b-jumbotron container-fluid :style="jumbostyle">
        <template v-slot:header><span style="color:#569cd6">var</span> <span style="color:#DCDCAA">Experience</span> = ()<span style="color:#569cd6">=></span>{</template>

        <template v-slot:lead :style="leadStyle">
        <span style="color:#4EC9B0">console</span>.<span style="color:#DCDCAA">log</span>(<span style="color:#ce9178">"I have interned as both IT and full-stack engineer.<br>
         I have worked in both BIM/CAD and Fintech respectively<br>
         My primary focus is being a software developer with widespread knowledge amongst many fields."</span>);<br>
        </template>
        };<br>
        <b-button id="linkedIn" href="https://www.linkedin.com/in/charles-carlson/">LinkedIn</b-button>
    </b-jumbotron>
    <b-row>
      <b-col>
        <p>Full-Stack Intern</p>
        <p>ElfinMarket<br>
        London, England</p>
        <p>Revamped the loan calculator on the client site <br>
        making it easier for company’s clients to understand <br>
        their monthly interest and total payment.<br>
        Created functions to automate emails from the backend admin page in Django<br>
        to help supervisor receive daily reports on useful client and finance data.</p>
      </b-col>
      <b-col>
        <p>IT Intern</p>
        <p>AcePLP<br>
        Singapore, Singapore</p>
        <p>Assisted finance interns by creating Visual Basic Macros in Excel
           Setup new workstations, and managed Databases<br>
           alongside with building a new web server for company
           Acted as representative for the company to consult Land and Transportation Authority of Singapore<br>
           about integrating VR/AR technology into the BIM workflow</p>
      </b-col>
    </b-row>
  </b-container>
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
      },
      containerStyle: {
        marginTop: '10px',
        borderStyle: 'solid',
        borderWidth: '15px'
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
