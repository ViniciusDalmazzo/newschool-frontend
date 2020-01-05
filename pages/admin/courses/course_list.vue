<template>
  <v-container class="layout">
    <v-row>
      <v-col>
        <v-card height="100%" class="mx-auto">
          <v-card-text style="height: 100px;" class="grey lighten-5">
            <h1 class="title-title">Meus Cursos</h1>
          </v-card-text>
          <v-card-text style="position: relative">
            <v-btn
              rounded
              absolute
              fab
              dark
              top
              right
              color="#6102b5"
              class="mx-4 rounded-button"
            >
              <v-icon size="50">mdi-plus</v-icon>
            </v-btn>
            <v-card-text class="text-center mt-12">
              <h1 class="no-content-ops">Ops! ):</h1>
            </v-card-text>
            <v-card-text class="text-center">
              <h2 class="no-content-course">Você não criou nenhum curso</h2>
            </v-card-text>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <navigation-bar />
  </v-container>
</template>
<router>
{
    path: '/admin/listar-cursos'
}
</router>
<script>
import NavigationBar from '~/components/NavigationBar.vue'
export default {
  components: {
    NavigationBar,
  },
}
</script>
<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,500,900&display=swap');
.layout {
  padding: unset !important;
}
.title-title {
  font-size: 25px !important;
  font-weight: bold !important;
  line-height: 50px;
  padding-left: 10px;
  text-transform: uppercase;
  color: #6102b5;
}
.header_courses {
  color: #ffffff !important;
}
.content_courses {
  text-align: center;
  color: #f8f8f8 !important;
}
.no-content-ops {
  font-size: 35px !important;
  font-weight: bold !important;
  line-height: 15px !important;
  text-transform: uppercase !important;
  color: #d2bfec;
}
.no-content-course {
  font-size: 15px !important;
  font-weight: 500 !important;
  line-height: 15px !important;
  text-transform: unset !important;
  color: #b3b3b3;
}
.line {
  border: 0;
  height: 0;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
  border-bottom: 1px solid rgba(255, 255, 255, 0.3);
}
.rounded-button {
  border-radius: 50px !important;
}
</style>