<template>
  <div>
    <header class="header">
      <b-navbar toggleable="md" type="dark">
        <b-navbar-brand>
          <b-img src="/images/logo.png" width="40" />
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item-dropdown text="圖表" left>
              <b-dropdown-item
                :to="{
                  name: 'anyChartStock'
                }"
                >anyChart</b-dropdown-item
              >
              <b-dropdown-item
                :to="{
                  name: 'highChartStock'
                }"
                >highCharts</b-dropdown-item
              >
            </b-nav-item-dropdown>
            <b-nav-item-dropdown text="工具" left>
              <b-dropdown-item
                :to="{
                  name: 'activity'
                }"
                >動態牆</b-dropdown-item
              >
              <b-dropdown-item
                :to="{
                  name: 'draggableTable'
                }"
                >Draggable Table</b-dropdown-item
              >
              <b-dropdown-item
                :to="{
                  name: 'vueTextHighlight'
                }"
                >Vue Text Highlight</b-dropdown-item
              >
              <b-dropdown-item
                :to="{
                  name: 'colorMode'
                }"
                >Color Mode</b-dropdown-item
              >
            </b-nav-item-dropdown>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </header>
    <nuxt />
  </div>
</template>

<style lang="scss" scoped>
.header {
  background-color: #040303;
}
</style>

<style>
body {
  background-color: #0d101d;
}
</style>
