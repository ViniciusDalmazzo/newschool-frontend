
<template>
  <div>
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
                style="z-index: auto;"
              >
                <v-icon size="50">mdi-plus</v-icon>
              </v-btn>

              <v-card class="mx-auto mt-8" width="100%">
                <v-container class="pa-0">
                  <v-row justify="space-between" class="ma-0">
                    <v-col cols="auto" class="pa-0">
                      <v-img
                        height="100%"
                        width="150"
                        src="https://i1.wp.com/meprepara.com.br/wp-content/uploads/2017/09/gre-math.jpg?fit=1086%2C724&ssl=1"
                      ></v-img>
                    </v-col>

                    <v-col class="pa-0 pt-1 pr-4">
                      <v-row class="flex-column pl-3 fill-height">
                        <h3>Matemática do Zero para o Enem</h3>
                        <p
                          class="text-sm-left pr-4"
                          style="word-break: break-word;"
                        >20 horas de aula com muita teoria e resoluções de exercícios.</p>
                      </v-row>
                    </v-col>

                    <v-col cols="auto" class="text-center pa-0">
                      <v-row class="flex-column ma-0 fill-height" justify="center">
                        <v-col class="px-0" style="background-color:#6102b5;">
                          <v-btn fab x-small icon dark>
                            <v-icon>mdi-pencil</v-icon>
                          </v-btn>
                        </v-col>

                        <v-col class="px-0" style="background-color:#E37579;">
                          <v-btn fab x-small icon dark>
                            <v-icon>mdi-delete</v-icon>
                          </v-btn>
                        </v-col>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-container>
              </v-card>

              <v-card class="mx-auto mt-8" width="100%">
                <v-container class="pa-0">
                  <v-row justify="space-between" class="ma-0">
                    <v-col cols="auto" class="pa-0">
                      <v-img
                        height="100%"
                        width="150"
                        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQtiNHFSSNG_a6fibOzyCCXVOGG_UTsAyFnrxjZ4WLNnx-u03sE&s"
                      ></v-img>
                    </v-col>

                    <v-col class="pa-0 pt-1 pr-4">
                      <v-row class="flex-column pl-3 fill-height">
                        <h3>Fotografia para iniciantes</h3>
                        <p
                          class="text-sm-left pr-4"
                          style="word-break: break-word;"
                        >20 horas de aula com muita teoria e resoluções de exercícios.</p>
                      </v-row>
                    </v-col>

                    <v-col cols="auto" class="text-center pa-0">
                      <v-row class="flex-column ma-0 fill-height" justify="center">
                        <v-col class="px-0" style="background-color:#6102b5;">
                          <v-btn fab x-small icon dark>
                            <v-icon>mdi-pencil</v-icon>
                          </v-btn>
                        </v-col>

                        <v-col class="px-0" style="background-color:#E37579;">
                          <v-btn fab x-small icon dark>
                            <v-icon>mdi-delete</v-icon>
                          </v-btn>
                        </v-col>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-container>
              </v-card>

              <v-card class="mx-auto mt-8" width="100%">
                <v-container class="pa-0">
                  <v-row justify="space-between" class="ma-0">
                    <v-col cols="auto" class="pa-0">
                      <v-img
                        height="100%"
                        width="150"
                        src="https://i.ytimg.com/vi/b5KAz_vzwbw/maxresdefault.jpg"
                      ></v-img>
                    </v-col>

                    <v-col class="pa-0 pt-1 pr-4">
                      <v-row class="flex-column pl-3 fill-height">
                        <h3>Fundamentos do Design Gráfico</h3>
                        <p
                          class="text-sm-left pr-4"
                          style="word-break: break-word;"
                        >20 horas de aula com muita teoria e resoluções de exercícios.</p>
                      </v-row>
                    </v-col>

                    <v-col cols="auto" class="text-center pa-0">
                      <v-row class="flex-column ma-0 fill-height" justify="center">
                        <v-col class="px-0" style="background-color:#6102b5;">
                          <v-btn fab x-small icon dark>
                            <v-icon>mdi-pencil</v-icon>
                          </v-btn>
                        </v-col>

                        <v-col class="px-0" style="background-color:#E37579;">
                          <v-btn fab x-small icon dark>
                            <v-icon>mdi-delete</v-icon>
                          </v-btn>
                        </v-col>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-container>
              </v-card>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
      <navigation-bar />
    </v-container>
  </div>
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