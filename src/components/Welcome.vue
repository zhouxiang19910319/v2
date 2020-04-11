<template>
  <v-container fluid class="d-flex">
    <div id="left_bar"></div>

    <div id="right_content">
      <p class="display-3">德一的清净园</p>

      <v-card tile>
        <v-list flat>
          <v-list-item-group v-model="item" color="primary">
            <v-list-item v-for="(item, i) in items" :key="i">
              <v-list-item-content>
                <v-list-item-title v-text="item.text"></v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-card>
    </div>

  </v-container>
</template>

<script>
export default {
  data: () => ({
    item: 1,
    items: [
      { text: "佛经原文" },
      { text: "佛经浅释" },
      { text: "读书笔记" },
      { text: "联系方式" }
    ]
  })
};
</script>

<style>
.container {
  border: 1px solid red;
}
</style>
