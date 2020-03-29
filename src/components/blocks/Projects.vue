<template>
<div>
    <p>Projects</p>
    <p> Some of the projects I have worked on range from web applications to GUI applications and drones.
        <a href="https://github.com/charles-carlson">For general projects go to my github</a>
    </p>
    <p><a href="https://github.com/sredna43/launch">Launch</a></p>
    <p>
        Worked on team to create a web application deployment system<br>
        Uses Docker and Kubernetes to deploy a user's web application <br>
        by containerizing their source code taken from a user's github</p>

    <p><a href="https://github.com/hannahdettmann/stoStow"> StoStow</a></p>
    <p> Created a RESTful API for a prototype site for the St. Olaf student government<br>
    RESTful API is done in node.js with ExpressJS and the frontend was done with Reactjs<br>
    Web application is meant to bring the government's storage to a digital library</p>
    <p><a href="https://github.com/charles-carlson/DroneGo"> Tello Drone Racing Program</a></p>
    <p> With a team, we created automated racing programs for Tello Drones in Go<br>
    The framework we used was Gobot. We created multiple race algorithms for the drones to fly.<br>
    We tested the difference in human piloting versus our own algorithm in different scenarios.</p>
    <hr>

</div>
</template>

<script>
import {BIcursor, BIarchive, BIoutlet} from 'bootstrap-vue'
export default {
  components: {
    BIcursor,
    BIarchive,
    BIoutlet
  }
}
</script>

<style scoped>
p{
    color:white;
    font-family: monospace;
}
</style>
