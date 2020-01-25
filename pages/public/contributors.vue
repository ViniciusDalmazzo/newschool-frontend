<template>
  <section>
    <HeaderBar :title="'CONTRIBUIDORES'" :backPage="true"></HeaderBar>

    <v-layout align-center justify-center>
      <v-flex style="text-align: -webkit-center;">
        <v-container class="pt-0">
          <v-row>
            <v-col v-for="people in peoples" :key="people.id" cols="12">
              <v-card
                raised
                hover
                max-width="344"
                min-width="200"
                min-height="200"
              >
                <v-avatar
                  style="border-radius:50%"
                  class="mx-auto d-block mt-2"
                  size="150"
                >
                  <img class="mt-2" :src="people.image" />
                </v-avatar>
                <v-card-text class="text-center">
                  <h6
                    class="category text-gray font-weight-thin mb-2"
                    style="text-transform: uppercase"
                  >
                    {{ people.role }}
                  </h6>
                  <h4 class="card-title subtitle-1">
                    {{ people.name }}
                  </h4>
                  <v-btn
                    class="mt-3"
                    fab
                    dark
                    :href="people.linkedInkUrl"
                    target="_blank"
                    style="border-radius:50px !important;background:linear-gradient(45deg, #007de0, #00609f, #7ba2da);"
                  >
                    <v-icon dark>mdi-linkedin-box</v-icon>
                  </v-btn>
                  <v-btn
                    class="mt-3"
                    fab
                    dark
                    :href="people.instagramLink"
                    target="_blank"
                    style="border-radius:50px !important;background:linear-gradient(45deg, #405de6, #5851db, #833ab4, #c13584, #e1306c, #fd1d1d);"
                  >
                    <v-icon dark>mdi-instagram</v-icon>
                  </v-btn>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-flex>
    </v-layout>
    <navigation-bar />
  </section>
</template>

<router>
  {
    path: '/contribuidores'
  }
</router>

<script>
import NavigationBar from '~/components/NavigationBar.vue';
import HeaderBar from '~/components/Header.vue';

export default {
  components: {
    HeaderBar,
    NavigationBar,
  },

  data() {
    return {
      peoples: [
        {
          id: 1,
          image:
            'https://media-exp2.licdn.com/dms/image/C4E03AQHzZVRHTMYxyg/profile-displayphoto-shrink_800_800/0?e=1585180800&v=beta&t=3Q82hNUf8Tp4cVxku7bAKmkkHonIq7b25GOYvFaEKb0',
          name: 'Joao Paulo Malara (Jotapê)',
          role: 'CEO / CO-FOUNDER',
          linkedInkUrl:
            'https://www.linkedin.com/in/joao-paulo-malara-jotap%C3%AA-ab9712131',
          instagramLink: 'https://www.instagram.com/joaomalara_',
        },
        {
          id: 2,
          image:
            'https://media-exp2.licdn.com/dms/image/C4D03AQFCu5UUnHMB8Q/profile-displayphoto-shrink_800_800/0?e=1585180800&v=beta&t=mCBeTtYAZ4fd6Gnoya9wQPo1-brI-lcO520ITSQ3Qus',
          name: 'Leonardo Oliveira Balsalobre',
          role: 'Front-end Developer',
          linkedInkUrl: 'https://www.linkedin.com/in/leonardo-balsalobre/',
          instagramLink: '',
        },
      ],
    };
  },
};
</script>

<style scoped></style>
