<template>
  <div id="wrapper">
    <MyBase></MyBase>
    <Header class=""></Header>
    <Profile></Profile>
    <Skill></Skill>
    <Work></Work>
    <Footer></Footer>
    
  </div>
</template>

<script>
import 'normalize.css';
import MyBase from './components/MyBase';
import Header from './components/Header';
import Profile from './components/Profile';
import Skill from './components/Skill';
import Work from './components/Work';
import Footer from './components/Footer';

export default {
  components: {
    'MyBase': MyBase,
    'Header': Header,
    'Profile': Profile,
    'Skill': Skill,
    'Work': Work,
    'Footer': Footer
  },
  data(){
    return{
    }
  }
}
</script>

<style>

</style>





