<template>
  <div id="container">
    <md-list id="select-list">
      <md-list-item>
        <h1 id="title" slot="headline">JouderMin的知识数据库</h1>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" @click="toTnoc" class="item-button">
        <div slot="headline">计算笔记</div>
        <div slot="supporting-text">The Note Of Calculation</div>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" @click="toNacsp" class="item-button">
        <div slot="headline">新世纪计算机科学计划</div>
        <div slot="supporting-text">New Age Computer Science Project</div>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" @click="toMcsdg" class="item-button">
        <div slot="headline">现代计算机软件开发指北</div>
        <div slot="supporting-text">Modern Computer Software Development Guide</div>
      </md-list-item>
      <md-divider />
      <md-list-item type="button" @click="toJdn" class="item-button">
        <div slot="headline">我的开发笔记</div>
        <div slot="supporting-text">Jouder's Development Notebook</div>
      </md-list-item>
    </md-list>
  </div>
</template>

<script setup lang="ts">
import { MdList } from '@material/web/list/list';
import { MdListItem } from '@material/web/list/list-item';
import { MdDivider } from '@material/web/divider/divider';

const toTnoc = () => {
  window.location.href = 'https://joudermin.github.io/tnoc/';
};

const toNacsp = () => {
  window.location.href = 'https://joudermin.github.io/nacsp/';
};

const toMcsdg = () => {
  window.location.href = 'https://joudermin.github.io/mcsdg/';
};

const toJdn = () => {
  window.location.href = 'https://joudermin.github.io/jdn/';
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
  box-shadow: rgba(0, 0, 0, 0.4) 0px 30px 90px;
}

#select-list {
  width: 80vw;
  max-width: 500px;
  max-height: fit-content;
}

#title {
  text-align: center;
  line-height: 50px;
  height: fit-content;
}

.item-button {
  border-radius: 8px;
}
</style>
