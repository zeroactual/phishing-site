<template lang="pug">
#IntroducingEagle.eg-theme-agrume
  .eg-slideshow
    slide(enter='fadeIn' leave='bounceOutLeft')
      .center.frontpage
        h1 Phishing
        h4 INFOSYS-3848 Group 4

    slide(:steps=2, enter='bounceInRight' leave='bounceOutDown')
      h3 Breif overview of security
      .left
        eg-transition(enter='bounceInLeft' leave='bounceOutLeft')
          p <b>Firwalls</b> keep attackers from directly accessing network
        eg-transition(enter='bounceInRight' leave='bounceOutRight')
          p(v-if="step >= 2")
            <b>Vue.js</b> supports components and transitions out of the box
        eg-transition(enter='bounceInLeft' leave='bounceOutLeft')
          p(v-if="step >= 2")
            <b>Eagle.js</b> adds navigation logics, scalable components, etc.


    slide(:steps=3, enter='bounceInRight' leave='bounceOutDown')
      h3 What is Phishing?
      .left
        eg-transition(enter='bounceInLeft' leave='bounceOutLeft')
          p(v-if="step >= 2")
            <b>Phishing</b> is a human problem
        eg-transition(enter='bounceInRight' leave='bounceOutRight')
          p(v-if="step >= 3")
            <b>Vue.js</b> supports components and transitions out of the box
        eg-transition(enter='bounceInLeft' leave='bounceOutLeft')
          p(v-if="step >= 3")
            <b>Eagle.js</b> adds navigation logics, scalable components, etc.

    slide(:steps=5, enter='bounceInDown')
      h3 What's in it for you

      eg-transition(enter='fadeIn' leave='fadeOut')
        .quarter(v-if='step >=2')
          h4 EASE OF USE
          p Clear syntax, live preview

      eg-transition(enter='fadeIn' leave='fadeOut')
        .quarter(v-if='step >=3')
          h4 MODULARITY
          p Reuse slides and styles

      eg-transition(enter='fadeIn' leave='fadeOut')
        .quarter(v-if="step >= 4")
         h4 INTERACTIVITY
         p Embed forms and live demos

      eg-transition(enter='fadeIn' leave='fadeOut')
        .quarter(v-if="step >= 5")
          h4 PORTABILITY
          p Play in any browser

    slide(:steps=2, enter='bounceInLeft', leave='bounceOutLeft')
      h3 Increasing activity
      img(src="./assets/rates.png")

    slide(:steps=2, enter='bounceInLeft', leave='bounceOutLeft')
      h3 How's it happen?
      img(src=".//assets/pie_chart.png")


</template>

<script>
import eagle from 'eagle.js'

export default {
  mixins: [eagle.slideshow],
  infos: {
    title: 'Presentation',
    description: 'Wes Jonas, Nicolette Lucido, Alex Mork, and Brett Stockglausner',
    path: 'phishing-deck'
  },
  components: {
  },
  data: function () {
    return {
      username: 'Wes',
      preference: 'Phishing',
      preferences: [
      ],
      slideCategories: {

      },
      preloadedImages: {

      }
    }
  },
  methods: {
    message: function () {
      return
    }
  }
}
</script>

<style lang='scss'>
@import 'node_modules/eagle.js/src/themes/agrume/agrume';
#IntroducingEagle {
  .frontpage {
    img {
      height: 7em;
    }
    img.control-schema {
      width: 8em;
      height: 3em;
    }
  }

  .quarter {
    text-align: center;
    p {
      margin-top: 0;
      text-align: center;
    }
    h4 {
      margin-top: 0;
      margin-bottom: 0
    }
  }
  a {
    color: black;
  }
}
</style>
