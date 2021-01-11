<template>
<div>
    <NuxtLink class="link active" style="text-decoration: none; color : black"  to="/">Connexion</NuxtLink>
    <NuxtLink class="link inactive" style="text-decoration: none; color : black"  to="/signup">Inscription</NuxtLink>

    <!-- Icon -->
    <div class="fadeIn first">
      <Logo />
    </div>

    <!-- Login Form -->
    <form>
      <input type="email" class="fadeIn second" name="login" placeholder="Email">
      <input type="text" class="fadeIn third" name="login" placeholder="Mot de passe">
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
  props : [
    'SubmitButtonName'
  ]
}
</script>

<style>

</style>
