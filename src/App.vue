<template>
  <div id="app" class="container-fluid">
    <div class="links container-fluid">

    <img :src="avy" class="avatar" alt="avatar" />

      <h1>{{ msg }}</h1>

      <div class="link">
        <a href="https://www.linkedin.com/in/natayafs/">
          <img :src="linkedin" width="30px" alt="linkedin" />
          Linkedin
        </a>
      </div>

      <div class="link">
        <a href="https://github.com/natayafs">
          <img :src="github" width="30px" alt="github" />
          Github
        </a>
      </div>

      <div class="link">
        <a href="https://comit.ar/">
          <img :src="mit" width="30px" alt="mit" />
          Comunidad MIT
        </a>
      </div>

      <div class="link">
        <a href="https://www.youtube.com/watch?v=tabBLNTPInQ">
          <img :src="youtube" width="30px" alt="webinar" />
          Webinar - Silicon Misiones
        </a>
      </div>

      <div class="link">
        <a href="https://open.spotify.com/episode/1JA988AUa8A3bjl2yQGLrW">
          <img :src="microphone" width="30px" alt="microphone" />
          Entrevista - Jonatan Ariste
        </a>
      </div>

      <div class="link">
        <a href="https://www.instagram.com/tv/CFiPGoRJA1s/?utm_source=ig_web_copy_link">
          <img :src="microphone" width="30px" alt="microphone" />
          Entrevista - Radio Circus FM
        </a>
      </div>

      <div class="link">
        <a href="https://enfoquemisiones.com/jonathan-y-nataya-egresados-de-la-universidad-del-conocimiento-es-un-proceso-que-no-solamente-tiene-que-ver-con-formacion-sino-con-inclusion/">
          <img :src="microphone" width="30px" alt="microphone" />
          Entrevista - Enfoque Misiones
        </a>
      </div>

    </div>

    <div class="mt-3 footer">
      <a href="https://twitter.com/natayafs">
          <img :src="twitter" height="30px" alt="twitter" />
      </a>
      <a href="https://instagram.com/natayafs">
          <img :src="instagram" height="30px" alt="instagram" />
      </a>
      <a href="https://cafecito.app/natayafs">
          <img :src="cafecito" height="30px" alt="cafecito" />
      </a>

    </div>
    <div class="footer container-fluid mt-5">
      <sup>Ilustración hecha por <a style="color: #3c373b;" href="https://www.instagram.com/mostrocartoon/">@MostroCartoon</a></sup>
    </div>
    <div class="footer container-fluid">
      <p>Creado con <img :src="heart" width="15px" alt="heart" /> | © 2020 Nataya</p>
    </div>
  </div>
</template>

<script>
import avy from './assets/avy.jpg'
import twitter from './assets/twitter.png'
import github from './assets/github.png'
import cafecito from './assets/cafecito.png'
import linkedin from './assets/linkedin.png'
import microphone from './assets/microphone.png'
import instagram from './assets/instagram.png'
import youtube from './assets/youtube.png'
import mit from './assets/mit.png'
import heart from './assets/heart.png'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Nataya Soledad',
      avy: avy,
      heart: heart,
      twitter: twitter,
      cafecito: cafecito,
      github: github,
      linkedin: linkedin,
      microphone: microphone,
      instagram: instagram,
      youtube: youtube,
      mit: mit
    }
  }
}
</script>

<style>
#app {
  background-size: 100%;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #3c373b;
  margin: 1.5em 0em;
}

* {
  background-color: transparent;
}

.links {
  padding: 0.2em 1.6em;
}

.link {
  margin: 0.5em;
  padding: 0.6em;
  font-weight: bold;
}

.link:nth-child(even) {
  background: rgb(203,227,255);
  background: -moz-linear-gradient(140deg, rgba(203,227,255,1) 0%, rgba(181,208,255,1) 35%, rgba(141,145,255,1) 100%);
  background: -webkit-linear-gradient(140deg, rgba(203,227,255,1) 0%, rgba(181,208,255,1) 35%, rgba(141,145,255,1) 100%);
  background: linear-gradient(140deg, rgba(203,227,255,1) 0%, rgba(181,208,255,1) 35%, rgba(141,145,255,1) 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#cbe3ff",endColorstr="#8d91ff",GradientType=1);
}

.link:nth-child(odd) {
  background: rgb(255,225,158);
  background: -moz-linear-gradient(140deg, rgba(255,225,158,1) 0%, rgba(255,204,89,1) 35%, rgba(255,166,88,1) 100%);
  background: -webkit-linear-gradient(140deg, rgba(255,225,158,1) 0%, rgba(255,204,89,1) 35%, rgba(255,166,88,1) 100%);
  background: linear-gradient(140deg, rgba(255,225,158,1) 0%, rgba(255,204,89,1) 35%, rgba(255,166,88,1) 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#ffe19e",endColorstr="#ffa658",GradientType=1);
}

.avatar {
  width: 10em;
  border-radius: 50%;
  background: linear-gradient(145deg, #eeeeee, #c8c8c8);
  box-shadow:  10px 10px 24px #a7a7a7,
               -10px -10px 24px #ffffff;
  margin-bottom: 2em;
}

h1, h2 {
  font-weight: normal;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 30px;
}

a {
  color: #ffffff;
}

a:hover {
  color: #3c373b;
  text-decoration:none;
  text-transform: uppercase;
}

.footer {
  display: flex;
  justify-content: center;
  background-color: white;
  color: #3c373b;
  font-size: 14px;
}
</style>
