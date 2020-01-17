<template>
  <div id="app">
    <div class="left-container">
      <img alt="logo" src="./assets/daikin.png" />
      <p>智能合同审阅</p>
    </div>
    <div class="right-container">
      <div class="upload-container">
        <el-upload
          class="upload-demo"
          drag
          action="https://jsonplaceholder.typicode.com/posts/"
          multiple
        >
          <i class="el-icon-upload"></i>
          <div class="el-upload__text">
            将文件拖到此处，或
            <em>点击上传</em>
          </div>
        </el-upload>
      </div>
      <div class="button-container">
        <el-upload
          class="upload-demo"
          action="https://jsonplaceholder.typicode.com/posts/"
          multiple
        >
          <el-button type="primary" round>上传文件</el-button>
        </el-upload>
        <el-button round>清除缓存</el-button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
#app {
  height: 100vh;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  background-image: url("./assets/background.jpg");
  background-size: 100% 100vh;
}

.left-container {
  float: left;
  width: 40vw;
  text-align: center;

  img {
    margin: 40px;
  }
  p {
    margin-top: -60px;
    font-size: 44px;
    font-weight: bold;
    color: #4682b4;
  }
}

.right-container {
  float: right;
  margin: 40px;
  height: 80vh;
  width: 50vw;
  background-color: rgba(255, 255, 255, 0.8);
  .upload-container {
    margin: 10vh 5vw;

    .el-upload-dragger {
      width: 40vw;
      height: 30vh;
    }
  }

  .button-container {
    margin-top: 10vh;
    text-align: center;

    .upload-demo {
      width: 240px;
      display: inline-block;
    }

    .el-button {
      margin: 20px;
      display: inline-block;
      width: 200px;
    }
  }
}

@media only screen and (max-width: 800px) {
  #app {
    height: 100vh;
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    text-align: center;
    background-image: url("./assets/background.jpg");
    background-size: 100% 100vh;
  }

  .left-container {
    width: 100vw;
    text-align: center;
    display: block;
    img {
      margin: 0;
      width: 50%;
    }

    p {
      margin-top: -80px;
      font-size: 36px;
      font-weight: bold;
      color: #4682b4;
    }
  }

  .right-container {
    margin: 0 10vw;
    width: 80vw;
    height: 50vh;
    text-align: center;
    display: block;

    .upload-container {
    margin: 5vh 5vw;

    .el-upload-dragger {
      width: 40vw;
      height: 30vh;
    }
  }

  .button-container {
    margin-top: -5vh;
    text-align: center;

    .upload-demo {
      width: 240px;
      display: inline-block;
    }

    .el-button {
      margin: 20px;
      display: inline-block;
      width: 200px;
    }
  }
  }
}
</style>
