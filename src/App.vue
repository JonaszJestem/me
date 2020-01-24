<template>
  <v-app class="app" :style="{ 'background-image': 'url(' + require('@/assets/forest.jpg') + ')' }">
    <div class="menu">
      <v-btn text >Home</v-btn>
    </div>
      <v-row class="flex content justify-center">
        <v-col class="col-8 flex justify-center">
          <v-img class="profile" :src="require('@/assets/me.jpeg')"/>
          <div class="welcome-message">
          <h1 class="text-center">Hi, I'm Jonasz</h1>
            <div class="social">
              <a href="https://github.com/JonaszJestem">
                <img src="https://img.icons8.com/material-rounded/384/000000/github.png" alt="GitHub Account"/>
              </a>
            </div>
          </div>
        </v-col>
      </v-row>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'App',

  components: {

  },

  data: () => ({
  })
})
</script>

<style lang="scss">
  .menu {
    display: flex;
    justify-content: flex-end;

    .v-btn {
      margin: 1rem;
      span {
        font-size: 1.25rem;
      }
    }
  }
  .content {
    .profile {
      height: 15rem;
      width: 15rem;
      border-radius: 50%;
      margin: 5rem auto 2rem;
      border: 3px solid black;

      -webkit-box-shadow: 3px 3px 6px 5px grey; /* Safari 3-4, iOS 4.0.2 - 4.2, Android 2.3+ */
      -moz-box-shadow: 3px 3px 6px 5px grey; /* Firefox 3.5 - 3.6 */
      box-shadow: 3px 3px 6px 5px grey; /* Opera 10.5, IE 9, Firefox 4+, Chrome 6+, iOS 5 */
    }

    .welcome-message {
      > h1 {
      -webkit-text-stroke: 1px gray;
        color: white;
        font-size: 4.5rem;
      }

      .social {
        width: 100%;
        display: flex;
        justify-content: center;

        img {
          height: 5rem;
          background-color: white;
          border-radius: 50%;
        }
      }
    }
  }
</style>
