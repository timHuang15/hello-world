<template>
  <div>
    <h1>垂直对齐</h1>
    <div class="container container-1">
        <span>一段文字</span>
    </div>

    <div class="container container-2">
        <div class="item">
            this is item
        </div>
    </div>

    <div class="container container-3">
        <div class="item">
            this is item
        </div>
    </div>

    <div class="container container-4">
        <div class="item">
            this is item
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {

    }
  },
  mounted() {

  },
  methods: {

  }
}

</script>
<style scoped>
.container {
    border: 1px solid #ccc;
    margin: 10px;
    padding: 10px;
    height: 200px;
}
.item {
    background-color: #ccc;
}

.container-1{
    text-align: center;
    line-height: 200px;
    height: 200px;
}

.container-2 {
    position: relative;
}
.container-2 .item {
    width: 300px;
    height: 100px;
    position: absolute;
    left: 50%;
    margin-left: -150px;
    top: 50%;
    margin-top: -50px;
}

.container-3 {
    position: relative;
}
.container-3 .item {
    width: 200px;
    height: 80px;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%)
}

.container-4 {
    position: relative;
}
.container-4 .item {
    width: 100px;
    height: 50px;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    margin: auto;
}
</style>
