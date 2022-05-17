<template>
  <div id="app">
    <div id="nav">
      <!--
      <vs-row v-for="component in this.componentDataList" :key="component.id">
        <vs-col vs-type="flex" vs-justify="left" vs-align="left" vs-w="1">
          <router-link :to="'/' + component.id">
            <NavButton :colour="component.colour" :heading="component.heading" :route="component.id" :id="component.id" @newroute="statechange($event)"/>
          </router-link>
        </vs-col>
      </vs-row>
    </div>
    <router-view/>
    -->
    </div>
    This page is currently undergoing maintainance, please check back later!
  </div>
</template>

<script>
import NavButton from './components/NavButton.vue'

export default {
  name: 'App',
  components: {
    NavButton
  },
  data() {
    return {
      componentDataList: [
        {'colour': "#fcb315", 'heading': "Working at Liberty IT: An Undergrad makes his case", 'id': "main"},
        {'colour': "#094560", 'heading': "Explaining Speculative Execution in Python", 'id': "ifVSelif"},
        {'colour': "#00BFFF", 'heading': "Using Unsupervised Learning to (almost) become a Dodgeball Ace", 'id': "dodgeball"},
        {'colour': "#663399", 'heading': "Can General AI exist within Machine Learning?", 'id': "neurips"},
        {'colour': "#E0218A", 'heading': "Source Code for this Webapp", 'id': "sourceCode"}
      ]
    }
  }
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
