<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar class="toolbar">
        <q-avatar size="12rem">
          <img
            class="object-contain"
            src="http://www.ctworks.es/img/logoblanco.png"
            alt="ct works logo"
          />
        </q-avatar>
        <q-toolbar-title class="font-light text-center app-title">
          PDF Make - Quick Test
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <h2 class="q-ml-lg color-primary page-title font-archivo">
        Client database
      </h2>
      <Table />
    </q-page-container>
  </q-layout>
</template>

<script>
import Table from '../components/Table';

export default {
  name: 'MainLayout',
  components: { Table },
  data() {
    return {
      dummyData: true
    };
  }
};
</script>

<style lang="scss">
.toolbar {
  height: 10vh;
}

.app-title {
  font-size: 2.5rem;
}

.page-title {
  font-weight: 500;
  font-size: 3rem;
}
</style>
