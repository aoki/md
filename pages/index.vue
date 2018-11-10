<template>
  <div id="main-container">
    <vue-split
      id="split"
      :elements="[
      '#editor',
      '#preview'
    ]"
      direction="horizontal"
      :min-size="100"
      :gutter-size="1"
      :snap-offset="50"
    >
      <div id="editor">
        <p>Editor</p>
      </div>
      <div id="preview">
        <p>Preview</p>
      </div>
    </vue-split>
  </div>
</template>

<script>
import VueSplit from 'vue-splitjs'

export default {
  components: {VueSplit},
}
</script>

<style scoped>
  .gutter {
    background-color: red !important;
  }
  #main-container {
    flex-basis: 100%;
  }
  #split {
    /*background: red;*/
    display: flex;
    height: 100%;
  }

  #editor {
    /*background: #00b786;*/
    flex-grow: 1;
    padding: 4px;
  }

  #preview {
    /*background: #8ceaf6;*/
    flex-grow: 1;
    padding: 4px;
  }
</style>
