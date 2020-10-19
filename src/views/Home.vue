<template>

 *mind your head; this site is still under construction*
<br>
<br>
<h3> TL;DR: </h3>
<ul>
  <li> I'm a  third year law student having my mid-life crisis about whether I want/am suited to practice law. </li>
  <li> I'm participating in the sixth iteration of the TechLadies Bootcamp, developing a product for Itsrainingraincoats' MADWISH -- a programme that matches volunteer English teachers with migrant workers. </li>
</ul>
<h3> I'm keen on getting experience in the following areas: </h3>
<ul>
  <li v-for="(item,index) in opps" :key="index"> 
    <strong>{{item.area}}</strong>: {{item.description}}
  </li>
</ul>

<h3> The long game: </h3>
Solve problems that matter, have some fun along the way, pick up new skills, religiously avoid busywork.
</template>

<script>


export default {
  name: 'Home',
  components: {},
  data() {
    return {
      opps: [
        {
          area: "Legal",
          description: "Work relating to tech, media and telecommunications. IP, data privacy, payments etc, in-house or with a law firm"
        },
        {
          area: "Research",
          description: "Empirical analysis of the law; implications of technological developments for law and policy; assessing access to justice"
        },
        {
          area: "Tech",
          description: "Legal industry & technology companies - Would love a chance to start off in less non-technical roles, learn on the job and eventually transition to a technical role.."
        }

      ]
      
    }
  }
  }


</script>

<style>
ul {
  padding-left: 20%
}

body {
  line-height: 20px
}
</style>
