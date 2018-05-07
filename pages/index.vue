<template>
  <div>  
    <section id="top-home">
      <div class="container text-center">
        <h1 class="title">
         Logo
        </h1>
        <h2 class="subtitle">Coding and Innovation
        </h2>
      </div>
      <div class="gradient-background"></div>
    </section>
    <section id="sub-home">
      <div class="container text-center">
         <h1 class="title">
          <span>Hi!,</span>
          <br>
          I'm a freelance creative front-end developer with 5+ years of professional experience, based in Buenos Aires.
        </h1>
        <a href="">more about me..</a><br>
        <a href="href://linkedin.com/in/maurodollinger/" title="mauro dollinger linkedIn">Here's my linkedIn profile</a><br>
      </div>
      
    </section>

    <section id="skills">
      <div class="container text-center">
        <h3>Skills</h3>

        <div class="box-skills">
          <div class="skill" v-for="skill in skillsLeft">
            <div class="skill-name">{{skill.name}}</div>
            <div class="skill-range">{{skill.range}}</div>
          </div>
        </div>
        <div class="box-skills">
          <div class="skill" v-for="skill in skillsRight">
            <div class="skill-name">{{skill.name}}</div>
            <div class="skill-range">{{skill.range}}</div>
          </div>
        </div>
      </div>
    </section>

    <section id="abilities">
      <div class="container text-center">
        <h3>Abilities</h3>

        <div class="box-abilities">
          <div class="ability" v-for="ability in abilities">
            <div class="ability-name">{{ability.name}}</div>
            <div class="ability-desc">{{ability.desc}}</div>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container text-center">
        <h3>Contact</h3>
      </div>
    </section>
  </div>
</template>

<script>

export default {
  components: {
  },
  data(){
    return{
      skillsLeft:[
        {name:'Vue',range:7},
        {name:'React',range:5},
        {name:'JavaScript',range:8},
        {name:'Sass',range:8},
        {name:'CSS',range:9},
        {name:'Bootstrap',range:8},
        {name:'HTML5',range:9},
      ],
      skillsRight:[
        {name:'Flex',range:7},
        {name:'Node.js',range:6},
        {name:'Webpack',range:6},
        {name:'Git',range:8},
        {name:'Sketch',range:5},
        {name:'Photoshop',range:8},
        {name:'Illustrator',range:8},
      ],
      abilities:[
        {name:'Responsive Layout',desc:'Visible for multiple devices'},
        {name:'Pixel Perfect Code',desc:''},
        {name:'Dynamic Animations',desc:'Suit transitions and cool effects'},
        {name:'Semantic',desc:'Taking advantage of HTML5 power'},
        {name:'Fast',desc:'Optimized, compressed, clean'},
        {name:'Cross-Browsing',desc:''}
      ]
    }
  }
}
</script>

<style>

</style>
