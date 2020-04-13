<template>
  <div class="panel">
    <div class="btn-container">
        <input type="text" name="email" placeholder="Email">
        <div class="btn">Email</div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.panel{
  background-color: rgb(51,51,51);
  text-align: center;
  padding: 10% 0;
  font-family: 'Courier New', Courier, monospace;
  position:fixed;
  width: 100%;
}
.panel .btn-container{
  display: inline-block;
}
.panel .btn-container input{
  border: 0;
  outline: 0;
  height: 60px;
  width: 120px;
  border-radius: 30px;
  background-color: rgb(104,101,101);
  color: #fff;
  font-size: 20px;
  padding: 0 20px;
  vertical-align: middle;
  transition: .2s;
}
.panel .btn-container .btn{
  display: inline-block;
  background-color: rgb(239,77,138);
  vertical-align: middle;
}
::-webkit-input-placeholder .btn{
  color: #fff;
  font-size: 20px;
  font-family: 'Courier New', Courier, monospace;
}
.panel .btn-container .btn{
  display: inline-block;
  vertical-align: middle;
  height: 60px;
  font-size: 20px;
  font-weight: bold;
  width: 170px;
  line-height: 60px;
  border-radius: 30px;
  cursor: pointer;
  margin-left: -170px;
  transition: .2s;
}
.panel .btn-container:hover input{
  width: 400px;
  animation: inputAction .4s ease-out;
}
.panel .btn-container:hover .btn{
  width: 100px;
  height: 60px;
  margin-left: -100px;
  animation: btnAction .4s ease-out;
}
@keyframes inputAction{
  0%{
    width: 400px;
  }
  60%{
    width: 450px;
  }
  100%{
    width: 400px;
  }
}
@keyframes btnAction{
  0%{
    width: 100px;
    height: 60px;
    margin-left: -100px;
  }
  60%{
    width: 60px;
    height: 60px;
    margin-left: -60px;
  }
  100%{
    width: 100px;
    height: 60px;
    margin-left: -100px;
  }
}
</style>