<template>
  <div>
    <q-layout view="hHh Lpr lff" class="rounded-borders">
      <q-header elevated class="bg-pink-2">
        <q-toolbar>
          <q-toolbar-title class="q-animate--fade text-center text-black">♥ HAPPY BIRTHDAY JENJEN ♥</q-toolbar-title>
        </q-toolbar>
      </q-header>

      <q-drawer
        v-model="drawer"
        show-if-above

        :mini="miniState"
        @mouseover="miniState = false"
        @mouseout="miniState = true"

        :width="200"
        :breakpoint="500"
        bordered
        class="bg-grey-3"
      >
        <q-scroll-area class="fit">
          <q-list padding>
            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="favorite" />
              </q-item-section>

              <q-item-section>
                Beepo
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="favorite" />
              </q-item-section>

              <q-item-section>
                Boop
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="favorite" />
              </q-item-section>

              <q-item-section>
                You're
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="favorite" />
              </q-item-section>

              <q-item-section>
                Awesome
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="favorite" />
              </q-item-section>

              <q-item-section>
                ♥
              </q-item-section>
            </q-item>
          </q-list>
        </q-scroll-area>
      </q-drawer>

      <q-page-container>
        <q-page class="relative-position">
          <div class="overlay"></div>
          <q-img
            src="/images/405EE1B3-B05A-4135-9901-4B26DDE3B3D2.webp"
            fit="fill"
          >
            <div class="absolute-full text-subtitle2 flex flex-center">
              <p class="text-center">
                Hi Jenjen ♥<br>
                Let me start of by wishing you the happiest of birthdays.<br>
                You have been such a blessing to me, and I will never be able to express in words<br>
                how lucky I feel to know you. In beauty, personally, presence, and everything else you do no less<br>
                than excell. In my books, no other person goes beyond you. You deserve all the blessings<br>
                the world can offer you. You deserve no less than the top.<br><br>

                You're strong, you're passionate, you're ambitious, you're tenacious, you're independent.<br><br>

                I wake up every day, knowing that there is always something I can do and want to do<br>
                to make your day better. It gives me the most fulfilling feeling when I do<br>
                and I will continue chasing that feeling for as long as I live. I sure as hell will make sure I'll<br>
                never let you go out of my life. YOU AIN'T LOSING MEEEEE~! <br><br>

                Thank you for being the blessing that you are. Your presence has made my day better each day. ♥<br>
                You truly mean the world to me, Jenna.<br>
                Have the happiest birthday. ♥
              </p>
            </div>
          </q-img>
        </q-page>
      </q-page-container>
    </q-layout>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      drawer: ref(false),
      miniState: ref(true)
    }
  }
}
</script>

<style lang="scss">
.pagebg {
  background: url("/images/405EE1B3-B05A-4135-9901-4B26DDE3B3D2.webp") center center no-repeat;
}
</style>
