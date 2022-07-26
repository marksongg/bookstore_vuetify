<template>
  <v-card class="breadcrumbsCard">
    <v-toolbar
          color="info"
          theme="dark"
    >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>Breadcrumbs组件</v-toolbar-title>

        <v-spacer></v-spacer>
    </v-toolbar>
    <div class="box">
        <v-breadcrumbs :items="items"></v-breadcrumbs>

        <v-breadcrumbs
        :items="items"
        large
        ></v-breadcrumbs>

        <v-breadcrumbs
        :items="items"
        divider="-"
        ></v-breadcrumbs>

        <v-breadcrumbs
        :items="items"
        divider="."
        ></v-breadcrumbs>

        <v-breadcrumbs :items="items">
            <template v-slot:divider>
                <v-icon icon="mdi-forward"></v-icon>
            </template>
        </v-breadcrumbs>

        <v-breadcrumbs :items="items">
            <template v-slot:divider>
                <v-icon icon="mdi-chevron-right"></v-icon>
            </template>
        </v-breadcrumbs>
    </div>
  </v-card>
</template>

<script>
export default {
  name: 'BreadcrumbsComp',
  data: () => ({
    items: [
    {
        text: 'Dashboard',
        disabled: false,
        href: 'breadcrumbs_dashboard',
    },
    {
        text: 'Link 1',
        disabled: false,
        href: 'breadcrumbs_link_1',
    },
    {
        text: 'Link 2',
        disabled: true,
        href: 'breadcrumbs_link_2',
    },
    ],
}),
}
</script>

<style scoped>

  .box {
    padding-left: 10px;
  }
</style>