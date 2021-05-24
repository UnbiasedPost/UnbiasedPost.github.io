<template>
  <v-layout align-center justify-center row wrap class="ma-2">
    <!-- Co Founders -->
    <v-flex xs12 sm4 md4 v-for="(item, i) in founders" v-bind:key="i">
      <v-card class="pa-2 ma-2" flat>
        <v-layout row>
          <v-flex xs7>
            <v-card-title primary-title>
              <div>
                <h3 class="headline mb-0">{{item.name}}</h3>
              </div>
            </v-card-title>
            <v-card-text>
              <div><strong>Co Founder</strong></div>
              <div class="pt-3"><strong>Phone:</strong></div>
              <div>{{item.phone}}</div>
              <div class="pt-3"><strong>Email:</strong></div>
              <div>{{item.mail}}</div>
            </v-card-text>
          </v-flex>
          <v-flex xs5 class="pt-4">
            <v-img
              :src="item.photo"
              height="125px"
              contain
            ></v-img>
          </v-flex>
        </v-layout>
        <v-divider></v-divider>
        <v-card-actions class="pa-3">
          <v-layout justify-center>
            <v-btn text icon color="black lighten-1" v-if="item.social.facebook.enabled" :href="item.social.facebook.url" target="_blank">
              <v-icon color="black darken-2">mdi-facebook</v-icon>
            </v-btn>
            <v-btn text icon color="black lighten-1" v-if="item.social.twitter.enabled" :href="item.social.twitter.url" target="_blank">
              <v-icon color="black darken-2">mdi-twitter</v-icon>
            </v-btn>
            <v-btn text icon color="black lighten-1" v-if="item.social.linkedin.enabled" :href="item.social.linkedin.url" target="_blank">
              <v-icon color="black darken-2">mdi-linkedin</v-icon>
            </v-btn>
            <v-btn text icon color="black lighten-1" v-if="item.social.github.enabled" :href="item.social.github.url" target="_blank">
              <v-icon color="black darken-2">mdi-github-circle</v-icon>
            </v-btn>
            <v-btn text icon color="black lighten-1" v-if="item.social.google.enabled" :href="item.social.google.url" target="_blank">
              <v-icon color="black darken-2">mdi-google-plus</v-icon>
            </v-btn>
          </v-layout>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
  export default {
    name: 'Contact',
    data () {
      return {
        founders: [
          // Madhumala Ghosh Paul
          {
            name: 'Madhumala Ghosh Paul',
            phone: '',
            mail: '',
            photo: '',
            social: {
              facebook: {
                url: '',
                enabled: false
              },
              twitter: {
                url: '',
                enabled: false
              },
              linkedin: {
                url: '',
                enabled: false
              },
              github: {
                url: '',
                enabled: false
              },
              google: {
                url: '',
                enabled: false
              }
            }
          },

          // Arup Nath Daw
          {
            name: 'Arup Nath Daw',
            phone: '',
            mail: '',
            photo: '',
            social: {
              facebook: {
                url: '',
                enabled: false
              },
              twitter: {
                url: '',
                enabled: false
              },
              linkedin: {
                url: '',
                enabled: false
              },
              github: {
                url: '',
                enabled: false
              },
              google: {
                url: '',
                enabled: false
              }
            }
          },

          // Sayantani Dasgupta
          {
            name: 'Sayantani Dasgupta',
            phone: '',
            mail: '',
            photo: '',
            social: {
              facebook: {
                url: '',
                enabled: false
              },
              twitter: {
                url: '',
                enabled: false
              },
              linkedin: {
                url: '',
                enabled: false
              },
              github: {
                url: '',
                enabled: false
              },
              google: {
                url: '',
                enabled: false
              }
            }
          },

          // Rohit Jha
          {
            name: 'Rohit Jha',
            phone: '',
            mail: '',
            photo: '',
            social: {
              facebook: {
                url: '',
                enabled: false
              },
              twitter: {
                url: '',
                enabled: false
              },
              linkedin: {
                url: '',
                enabled: false
              },
              github: {
                url: '',
                enabled: false
              },
              google: {
                url: '',
                enabled: false
              }
            }
          },

          // Prabir Ghosh
          {
            name: 'Prabir Ghosh',
            phone: '+91 993 33 72215',
            mail: 'mymail.prabir@gmail.com',
            photo: 'prabir.webp',
            social: {
              facebook: {
                url: 'http://www.facebook.com/djprabir',
                enabled: true
              },
              twitter: {
                url: 'http://www.twitter.com/djprabir',
                enabled: true
              },
              linkedin: {
                url: 'https://www.linkedin.com/in/prabir-ghosh',
                enabled: true
              },
              github: {
                url: 'https://github.com/PRABIRSOFT',
                enabled: true
              },
              google: {
                url: 'http://plus.google.com/+PrabirGhoshGplus',
                enabled: true
              }
            }
          },
        ]
      }
    },
  }
</script>
