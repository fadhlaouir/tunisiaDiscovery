<template>

  <v-container>
    <v-toolbar flat class="mainHeader">
      <v-toolbar-title> Tunisia Discovery Project </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn text><router-link to="/home"> Home </router-link></v-btn>
        <v-btn text><router-link to="/"> Destinations </router-link></v-btn>
        <v-btn text><router-link to="/hotels"> Hotels </router-link></v-btn>
        <v-btn text><router-link to="/events">Events </router-link></v-btn>
        <v-btn text><router-link to="/cars"> Cars </router-link></v-btn>

      </v-toolbar-items>

      <div class="hidden-sm-and-up">
        <v-menu offset-y>
          <v-list class="responsiveMenu">
            <v-list-item>
              <v-list-item-title><router-link to="/home"> Home </router-link></v-list-item-title>
              <v-list-item-title><router-link to="/places"> Places  </router-link></v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title><router-link to="/hotels"> Hotels  </router-link></v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title><router-link to="/events"> Events </router-link></v-list-item-title>
              <v-list-item-title><router-link to="/cars"> Cars </router-link></v-list-item-title>
          </v-list-item>
          </v-list>
        </v-menu>
      </div>
       <v-toolbar-side-icon></v-toolbar-side-icon>
            <v-toolbar-title>{{appTitle}}</v-toolbar-title>
           
            <v-spacer></v-spacer>
            <span>Not a member yet?</span>
            <v-spacer></v-spacer>
            <v-btn color="blue lighten-3" router-link to="/signin"> SIGN IN</v-btn>
            <v-btn color="blue lighten-3" router-link to="/signup"> SIGN UP </v-btn>
    </v-toolbar>
  </v-container>
</template>

<script>
export default {
  name: "Navbar",
  data: () => ({
  })
};
</script>

