<template>
<div>
    <NuxtLink class="link active" style="text-decoration: none; color : black"  to="/">Connexion</NuxtLink>
    <NuxtLink class="link inactive" style="text-decoration: none; color : black"  to="/signup">Inscription</NuxtLink>

    <!-- Icon -->
    <div class="fadeIn first">
      <Logo />
    </div>

    <!-- Login Form -->
    <form @submit.prevent="submitAuth">
      <input type="email" class="fadeIn second" name="login" v-model="email" placeholder="Email" required>
      <input type="text" class="fadeIn third" name="login" v-model="pwd" placeholder="Mot de passe" required>
      <button class="fadeIn fourth" type="submit">{{SubmitButtonName}}</button>
    </form>

    <!-- Remind Passowrd -->
    <div id="formFooter">
      <NuxtLink class="underlineHover" style="text-decoration: none;" to="/quizz">Mot de passe oublié ?</NuxtLink>
    </div>
</div>

</template>

<script>
export default {
  data (){
    return{
      email : '',
      pwd : ''
    }
  },
  props : [
    'SubmitButtonName',
    'methode'
  ],
  methods : {
    async submitAuth (){
     
      if(this.methode === "signin"){
        console.log("signin ------------------------------------>")
      }      
      if(this.methode === "signup"){
        console.log("signup ------------------------------------>")
      }
    }
  }

}
</script>

<style>

</style>
