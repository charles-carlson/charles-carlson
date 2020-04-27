<template>
<div>
    <b-container :style="containerStyle">
    <b-row :style="colStyle">
        <b-col ><h1>Projects</h1></b-col>
    </b-row>
    <b-row :style="colStyle">
        <b-col>
        Some of the projects I have worked on range from<br> web applications to GUI applications and drones.<br>
        <a href="https://github.com/charles-carlson">For general projects go to my github</a>
        </b-col>
    </b-row>
    <b-card no-body border-variant="dark" :style='cardStyle'>
        <b-tabs no-fade card vertical>
            <b-tab lazy>
                <template v-slot:title>
                    <font-awesome-icon :icon="['fas', 'rocket']" :style="tabStyle"/>
                </template>
                <h1>{{projects.proj1}}</h1>
                <p>
                    {{content.s1}}<br>
                    {{content.s2}}<br>
                    {{content.s3}}
                </p>
        <b-button href="https://github.com/sredna43/launch">Github</b-button>
            </b-tab>
            <b-tab lazy>
                <template v-slot:title>
                    <font-awesome-icon :icon="['fas','save']" :style="tabStyle"/>
                </template>
                <h1>{{projects.proj2}}</h1>
                <p>
                    {{content.s4}}<br>
                    {{content.s5}}<br>
                    {{content.s6}}
                </p>
                <b-button href="https://github.com/hannahdettmann/stoStow">Github</b-button>
            </b-tab>
            <b-tab lazy>
                <template v-slot:title>
                    <font-awesome-icon :icon="['fas','robot']" :style="tabStyle"/>
                </template>
                <h1>{{projects.proj3}}</h1>
                <p>
                    {{content.s7}}<br>
                    {{content.s8}}<br>
                    {{content.s9}}
                </p>
                <b-button href="https://github.com/charles-carlson/DroneGo">Github</b-button>
            </b-tab>
        </b-tabs>
    </b-card>
    </b-container>
</div>
</template>

<script>
export default {
  data () {
    return {
      projects: {
        proj1: 'Launch',
        proj2: 'StoStow',
        proj3: 'Tello Drone Racing Program'
      },
      content: {
        s1: 'Worked on team to create a web application deployment system',
        s2: "Uses Docker and Kubernetes to deploy a user's web application",
        s3: "by containerizing their source code taken from a user's github",
        s4: 'Created a RESTful API for a prototype site for the St. Olaf student government',
        s5: 'RESTful API is done in node.js with ExpressJS and the frontend was done with Reactjs',
        s6: "Web application is meant to bring the government's storage to a digital library",
        s7: 'With a team, we created automated racing programs for Tello Drones in Go',
        s8: 'The framework we used was Gobot. We created multiple race algorithms for the drones to fly.',
        s9: 'We tested the difference in human piloting versus our own algorithm in different scenarios.'
      },
      tabStyle: {
        color: '#858585',
        highlight: 'white'
      },
      colStyle: {
        color: 'white',
        fontFamily: 'monospace',
        marginBottom: '5px'
      },
      cardStyle: {
        marginTop: '15px',
        maxWidth: '50rem',
        maxHeight: '25rem'
      },
      containerStyle: {
        borderStyle: 'solid',
        borderWidth: '15px',
        marginTop: '10px'
      }
    }
  }
}
</script>

<style scoped>
h1{
  color:white;
  font-family: monospace;
}
p{
    color:white;
    font-family: monospace;
}
.card{
  border:none
}

</style>
