<template>
  <div>
    <v-app-bar
       absolute
      color="#6A76AB"
      dark>

      <template v-slot:extension>
        <v-tabs align-with-title>
          <v-tab class="tabs-biologia">Biologia</v-tab>
          <v-tab class="tabs-matematica">matematicas</v-tab>
          <v-tab class="tabs ciencias">ciencias</v-tab>
        </v-tabs>
      </template>

      
    </v-app-bar>
  </div>
</template>