<template>
  <q-page class="flex flex-center">
    <div class="col">
      <q-input
        bottom-slots
        v-model="text"
        label="Label"
        counter
        maxlength="12"
        :dense="dense"
      >
        <template v-slot:before>
          <q-icon name="event" />
        </template>

        <template v-slot:hint> Field hint </template>

        <template v-slot:append>
          <q-btn round dense flat icon="add" />
        </template>
      </q-input>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageIndex",
});
</script>

<style lang="sass">
// https://uigradients.com/#Turquoiseflow
.q-page
  background: linear-gradient(to bottom, #267871, #136a8a)
</style>