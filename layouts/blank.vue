<template>
  <div class="d-flex align-center justify-center" style="height: 100vh" margin="1px">
      <v-sheet width="400" class="mx-auto">
          <v-form fast-fail @submit.prevent="login">
              <v-text-field v-model="username" label="Usuario"></v-text-field>

              <v-text-field v-model="password" label="Contraseña"></v-text-field>
              <a href="#" class="text-body-2 font-weight-regular">¿Olvidaste tu contraseña?</a>

              <v-btn type="submit" color="primary" block class="mt-2">Ingresar</v-btn>

          </v-form>
          <div class="mt-2">
              <p class="text-body-2">¿No tienes una cuenta? <a href="#">Registrarse</a></p>
          </div>
      </v-sheet>
  </div>
</template>

<script>
export default {
  data() {
      return {
          username: '',
          password: '',
      };
  },
  methods: {
      login() {
          // Your login logic here
      },
  },
}
definePageMeta({
  layout: "blank",
});
</script>

<!--   
  <div>
    <center>
      <h1>Bienvenidos a la app de tareas</h1>
      <p>Esta es una aplicación que permite gestionar las tareas de los estudiantes</p>

      <a href="/tareas">Click para iniciar (sin nuxtLink)</a>
<br>
<br>
      <NuxtLink to="/tareas">
        Click para iniciar (Con nuxtLink)
      </NuxtLink>
    </center>

  </div>

-->

<!--


<script>
definePageMeta({
  layout: "blank",
});
</script>
-->