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
                    {{content.s3}}<br>
                    {{content.s4}}<br>
                    {{content.s4_1}}<br>
                    {{content.s4_2}}<br>
                    {{content.s4_3}}
                </p>
        <b-button href="https://github.com/sredna43/launch">Github</b-button>
            </b-tab>
            <b-tab lazy>
                <template v-slot:title>
                    <font-awesome-icon :icon="['fas','save']" :style="tabStyle"/>
                </template>
                <h1>{{projects.proj2}}</h1>
                <p>
                    {{content.s5}}<br>
                    {{content.s6}}<br>
                    {{content.s7}}<br>
                    {{content.s7_1}}
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
                    {{content.s9}}<br>
                    {{content.s10}}<br>
                    {{content.s10_1}}<br>
                    {{content.s10_2}}<br>
                    {{content.s10_3}}<br>
                    {{content.s10_4}}
                </p>
                <b-button href="https://github.com/charles-carlson/DroneGo">Github</b-button>
            </b-tab>
            <b-tab lazy>
              <template v-slot:title>
                <font-awesome-icon :icon="['fas','gamepad']" :style="tabStyle"/>
              </template>
              <h1>{{projects.proj4}}</h1>
              <p>
                {{content.s11}}<br>
                {{content.s12}}<br>
                {{content.s13}}<br>
                {{content.s14}}<br>
                {{content.s14_1}}<br>
                {{content.s14_2}}<br>
                {{content.s14_3}}
              </p>
              <b-button href="https://github.com/charles-carlson/click">Github</b-button>
            </b-tab>
            <b-tab lazy>
              <template v-slot:title>
                <font-awesome-icon :icon="['fas','calendar-alt']" :style="tabStyle"/>
              </template>
              <h1>{{projects.proj5}}</h1>
              <p>
                {{content.s15}}<br>
                {{content.s16}}<br>
                {{content.s17}}<br>
                {{content.s18}}<br>
                {{content.s18}}
              </p>
              <b-button href="https://github.com/charles-carlson/planner">Github</b-button>
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
        proj3: 'Tello Drone Racing Program',
        proj4: 'Clicker Game',
        proj5: 'Todo App'
      },
      content: {
        s1: 'My undergrad research was on utilizing Kubernetes to create a web application deployment system.',
        s2: 'In a team of 4, we developed with python/Flask to create a launcher that would automate the deployment.',
        s3: "By containerizing their source code taken from a user's github, we could designate their application to a pod and be live",
        s4: 'All that is required from the user is a docker file and pushed to their repo.',
        s4_1: 'I learned a lot about the development process, and communication is key for a successful project.',
        s4_2: 'However there were a lot of stressfull moments, especially during our ethics analysis, but',
        s4_3: 'I enjoyed the project immensely, and gained a lot of experience on working with a team on a deadline.',
        s5: 'Created a RESTful API for a prototype site for the St. Olaf student government',
        s6: 'RESTful API is done in node.js with ExpressJS and the frontend was done with Reactjs',
        s7: "Web application is meant to bring the government's storage to a digital library",
        s7_1: 'Got experience working with client that gave input on design decisions for application.',
        s8: 'With a team, we created automated racing programs for Tello Drones in Go',
        s9: 'The framework we used was Gobot. We created multiple race algorithms for the drones to fly.',
        s10: 'We tested the difference in human piloting versus our own algorithm in different scenarios.',
        s10_1: 'This project was a lot of fun; drones/robots was a field I unknown too for a long time.',
        s10_2: 'It had a lot of ambition especially with opencv, but GoCv was having problems, so instead',
        s10_3: 'Backtracked to our original plan of human vs ai flight testing.',
        s10_4: 'At least with human control, we could record the drone footage.',
        s11: 'In a team of 3, we created a react-native mobile game. Click the button for a score, and compare yourself',
        s12: 'against other users. Application showcases our user authentication system, as well as other features including:',
        s13: ' a settings menu, highscore leaderboard, login/logout, and a in-game currency.',
        s14: 'The backend was developed with node.js/ExpressJS and has a Postgresql database.',
        s14_1: 'One of my last senior projects, I will look fondly back on as I had a lot of fun learning about mobile development.',
        s14_2: 'I did feel pressed for time, as the project start date got delayed ahead, yet the deadline stayed the same.',
        s14_3: 'But I overcame that challenge, and spent many hours and tears on creating the best possible product with the amount of time allotted.',
        s15: 'The TODO App, is a simple planner application, however it is developed with React and Next.js.',
        s16: 'For this project, I wanted to learn about server side rendering, and file system databases.',
        s17: 'Rather than use Postgres, I am using SQLite and Sequelize for a MVC structure.',
        s18: 'The backend uses Express, rather than Nextjs api creation. My favorite backend framework is Express or just plain node.js',
        s19: 'I have more plans for this project, as I want to have a dashboard as well as ability to go back to previous days.'
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
