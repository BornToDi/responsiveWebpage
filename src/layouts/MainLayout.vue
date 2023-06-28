<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <div class="bg-blue-grey-6">
      <q-toolbar>
        <q-toolbar-title>
          <div class="text-cyan-11 text-bold">Quasar Website</div>
          <div class="lt-md">
            <div class="q-py-xs">
    <q-btn-dropdown color="pink"  icon="menu" >
      <q-list>
        <q-item clickable v-close-popup @click="onItemClick">
          <q-item-section>
            <q-btn class="q-mx-sm q-py-sm   " outline color="black" label="SingUp" />
          </q-item-section>
        </q-item>

        <q-item clickable v-close-popup @click="onItemClick">
          <q-item-section>
          <q-btn class="q-mx-sm q-py-sm " outline color="black" label="SingIn" />
          </q-item-section>
        </q-item>

       
      </q-list>
    </q-btn-dropdown>
  </div>
          
        </div>
        </q-toolbar-title>

        <div class="gt-sm">
          <q-btn class="q-mx-sm q-py-sm " outline color="cyan-11" label="Sign Up" />
          <q-btn class="q-mx-sm q-py-sm " outline color="cyan-11" label="Sing In" />
        </div>
      </q-toolbar>
    </div>
    </q-header>

    

    <q-page-container>
      <router-view />

    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'


export default defineComponent({
  name: 'MainLayout',

  components: {
   
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
     
    }
  }
})
</script>
