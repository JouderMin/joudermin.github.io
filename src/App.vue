<template>
  <div id="container">
    <md-list id="select-list">
      <md-list-item>
        <h1 id="title" slot="headline">JouderMin的知识数据库</h1>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" class="item-button">
        <div slot="headline">Hello</div>
        <div slot="supporting-text">World</div>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" @click="toNacsp" class="item-button">
        <div slot="headline">新世纪计算机科学计划</div>
        <div slot="supporting-text">New Age Computer Science Project</div>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" class="item-button">
        <div slot="headline">Hello</div>
        <div slot="supporting-text">World</div>
      </md-list-item>
    </md-list>
  </div>
</template>

<script setup lang="ts">
import { MdList } from '@material/web/list/list';
import { MdListItem } from '@material/web/list/list-item';
import { MdDivider } from '@material/web/divider/divider';

const toNacsp = () => {
  window.location.href = 'https://joudermin.github.io/nacsp/';
};
</script>

<style scoped>
#container {
  width: fit-content;
  height: fit-content;
  padding: 20px;
  padding-top: 0px;
  background-color: var(--md-list-container-color, var(--md-sys-color-surface, #fef7ff));
  border-radius: 8px;
  text-rendering: geometricPrecision !important;
}

#select-list {
  width: 500px;
  max-width: 500px;
  max-height: fit-content;
}

#title {
  text-align: center;
  line-height: 50px;
  height: 50px;
}

.item-button {
  border-radius: 8px;
}
</style>
