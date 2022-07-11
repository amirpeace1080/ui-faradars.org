<template>
  <div class="navbar-main">
    <!-- size lg -->
    <v-app-bar class="d-none d-sm-flex pr-14" color="white" fixed>
      <v-toolbar-items class="d-flex align-center">
        <v-toolbar-title class="d-flex align-center">
          <v-img
            width="90"
            height="22"
            src="https://faradars.org/next/svg/faradarsLogo.svg"
          />
        </v-toolbar-title>
        <v-btn color="primary" class="mr-9 all-learn" outlined tile width="116">
          <span>همه آموزش ها</span>
        </v-btn>
        <v-text-field
          class="mr-2 input-search"
          solo
          label="جستجوی آموزش..."
          append-icon="mdi-search-web"
        ></v-text-field>
      </v-toolbar-items>
      <v-spacer></v-spacer>

      <v-toolbar-items class="d-flex align-center">
          <a href="#" style="margin-right: 240px">
            <v-icon class="mr-1">mdi-account-details-outline</v-icon>
          </a>
        <a href="#">
            <span class="ml-3" style="color: #000">تدریس در فرادرس</span>
        </a>
        <a href="#">
            <span class="ml-3" style="color: #000">ورود</span>
        </a>
        <a href="#">
            <span class="ml-3" style="color: #000">ثبت نام</span>
        </a>
      </v-toolbar-items>
    </v-app-bar>

    <!-- size mobile -->
    <v-app-bar class="hidden-sm-and-up" color="white">
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
        <v-toolbar-title class="d-flex align-center">
          <v-img
            width="50"
            height="22"
            src="https://faradars.org/next/svg/faradars-row.svg"
          />
        </v-toolbar-title>
      <v-spacer></v-spacer>
        <v-btn text>
          <v-icon class="mr-2">mdi-search-web</v-icon>
        </v-btn>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute temporary right>
      <v-divider></v-divider>
      <v-list nav dense>
        <v-list-item-group color="primary">
          <v-list-item>
            <v-list-item-content class="mt-1">
              <v-list-item-title>
                <v-icon large>mdi-close</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-content class="mt-2">
              <v-list-item-title>
                <v-icon>mdi-key-variant</v-icon>
                <span class="subtitle-1 mr-1">ورود</span>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-content class="mt-2">
              <v-list-item-title>
                <v-icon>mdi-account-lock</v-icon>
                <span class="subtitle-1 mr-1">ثبت نام</span>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-list-item>
            <v-list-item-content class="mt-2">
              <v-list-item-title>
                <v-icon>mdi-view-dashboard</v-icon>
                <span class="subtitle-1 mr-1">همه آموزش ها</span>
                  <v-icon class="mr-10">mdi-chevron-left</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-list-item>
            <v-list-item-content class="mt-2">
              <v-list-item-title>
                <v-icon>mdi-account-details-outline</v-icon>
                <span class="subtitle-1 mr-1">تدریس درفرادرس</span>
                  <v-icon class="mr-8">mdi-chevron-left</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      group: null,
    };
  },
};
</script>

<style scoped>
/* .navbar-main {
  margin-bottom: 50px;
} */
.all-learn {
  max-height: 36px;
}
.input-search {
  width: 380px;
  height: 36px;
}
</style>