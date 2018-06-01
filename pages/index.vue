<template>
  <div>  
    <section id="top-home">
      <div class="container text-center">
        <img src="~/assets/img/MD_web_logo_05.png" alt="MD" v-in-viewport>
        <h1 class="title">
        </h1>
        <div>
          <h2 class="subtitle"> 
            <vue-typer text='Coding and Innovation'></vue-typer>
          </h2>
        </div>        
      </div>
      <div class="gradient-background"></div>
    </section>
    <section id="sub-home">
      <div class="container text-center">
         <h1 class="title" v-in-viewport>
          <span>Hi!,</span>
          <br>
          I'm a freelance creative front-end developer with 5+ years of professional experience, based in Buenos Aires.
        </h1> 
        <a href="#" v-scroll-to="'#about'">More about me..</a><br>
        <a href="href://linkedin.com/in/maurodollinger/" title="mauro dollinger linkedIn">My linkedIn profile</a><br>
      </div>
      
    </section>

    <section id="skills" >
      <div class="container text-center">
        <h3>Skills</h3>

        <div class="box-skills">
          <div class="skill" v-for="skill in skillsLeft" v-in-viewport>
            <div class="skill-name">{{skill.name}}</div>
            <div class="skill-back" >
              <div class="skill-range" :style="{width:(skill.range*10) + '%'}"></div>
            </div>
          </div>
        </div>
        <div class="box-skills">
          <div class="skill" v-for="skill in skillsRight" v-in-viewport>
            <div class="skill-name">{{skill.name}}</div>
            <div class="skill-back">
              <div class="skill-range" :style="{width:(skill.range*10) + '%'}"></div>
            </div>
          </div>
        </div>

        <div class="box-info" id="about" v-in-viewport>
          <p>"I have been working on this for more than five years. I began developing games in AS3, then I migrate to HTML5 and JavaScript, and nowadays I’m developing web apps using Vue.JS. My career on the area gave me abilities on scrum and task management. My formal education is diverse. Furthermore of informatics I’ve study art, design and music. These knowledge gave me an analytic, creative and innovator profile. What I like the most of my job is to challenge me to new risks."</p>
        </div>
      </div>
    </section>

    <section id="abilities">
      <div class="container text-center">
        <h3>Abilities</h3>

        <div class="box-abilities">
          <div class="ability col-xs-12 col-sm-6 col-md-4" v-for="ability in abilities" v-in-viewport>
            <div class="ability-circle"><img :src="`img/${ability.img}`" :alt="ability.name"></div>
            <div class="ability-name">{{ability.name}}</div>
            <div class="ability-desc">{{ability.desc}}</div>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container text-center">
        <h3>Contact</h3>

        <div class="box-contact">
          <div class="col-xs-12">
            <input type="text" name="name" placeholder="Your Name">  
          </div>   
          <div class="col-xs-12">
            <input type="email" name="email" placeholder="Your Email">
          </div>
          <div class="col-xs-12">
            <textarea name="comment" placeholder="Leave a message.."></textarea>
          </div>
          <div class="col-xs-12">
            <input type="submit" name="" value="Submit your message">
          </div>  
        </div>
      </div>
    </section>
  </div>
</template>

<script>

if (process.browser) {
  var VueTyper = require('vue-typer').VueTyper
}
export default {
  components: {
    VueTyper
  },
  data(){
    return{
      skillsLeft:[
        {name:'HTML5',range:9},
        {name:'Sass',range:8},
        {name:'CSS',range:9},
        {name:'Bootstrap',range:8},
        {name:'Vue',range:7},
        {name:'React',range:5},
        {name:'JavaScript',range:8}
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
        {name:'Responsive',desc:'Scalable on multiple devices',img:'responsive.png'},
        {name:'Dynamic Animations',desc:'Suit transitions and cool effects',img:'animations.png'},
        {name:'Cross-Browsing',desc:'Visible on top browsers',img:'crossbrowsing.png'},
        {name:'Fast',desc:'Optimized code, compressed, clean',img:'fast.png'},
        {name:'Pixel Perfect Code',desc:'Designs well represented',img:'pixelperfect.png'},
        {name:'Semantic',desc:'Taking advantage of HTML5 power',img:'semantic.png'}
      ]
    }
  }
}
</script>

<style>

</style>
