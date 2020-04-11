<template>
  <div class="card-container">
      <div class="image-wrapper">
          <img src="../../assets/images/image_card.jpg" alt="">
      </div>
      <div class="title-wrapper">
          <h1 class="title">Ales Smith</h1>
          <p class="subtitle">hhhhhhhhhasdjasda</p>
          <hr>
          <div class="icon-btns">
              <ul>
                  <li><i class="iconfont icon-facebook"></i></li>
                  <li><i class="iconfont icon-tuitetwitter44"></i></li>
                  <li><i class="iconfont icon-instagram"></i></li>
                  <li><i class="iconfont icon-Gmail"></i></li>
              </ul>
          </div>
      </div>
  </div>
</template>

<script>

export default {

}
</script>

<style>
    .card-container {
        width: 700px;
        height:650px;
        margin: 0 auto;
        animation: cardContainerLoad 2s;
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        background: -webkit-linear-gradient(left bottom,rgb(121,150,137),rgb(55,68,110));
    }

    @keyframes cardContainerLoad {
        from {
            opacity: 0;
            transform: translate3d(0,10%,0)
        }
        to {
            opacity: 1;
            transform: none;
        }
    }

    .card-container .image-wrapper {
        font-size: 0px;
    }

    .card-container .image-wrapper img {
        width: 600px;
        border-radius: 8px 8px 0 0 ;
    }

    .card-container .title-wrapper {
        background-color: #fff;
        border-radius: 0 0 8px 8px;
        width:600px;
        margin: 0 auto;
    }

    .card-container .title-wrapper .title {
        text-align: center;
        padding: 20px 0;
    }

    .card-container .title-wrapper .subtitle {
    text-align: center;
    font-size: 20px;
    padding: 0;
    color: rgb(79, 92, 99);
    }

    .card-container .title-wrapper hr {
    border: 0;
    height: 1px;
    background-color: rgb(179, 192, 199);;
    margin: 0 10px;
    }

    .card-container .title-wrapper  .icon-btns {
    padding: 20px 0;
    }

    .card-container .title-wrapper  .icon-btns ul {
    list-style: none;
    padding: 0;
    margin: 0;
    text-align: center;
    }

    .card-container .title-wrapper  .icon-btns ul li{
    display: inline-block;
    border: 1px solid #000;
    padding: 5px 15px;
    border-radius: 35px;
    cursor: pointer;
    border-color: rgb(79, 92, 99);
    transition: .2s;
    }

    .card-container .title-wrapper  .icon-btns ul li:hover {
    border-color: rgb(179, 192, 199);
    }

    .card-container .title-wrapper  .icon-btns ul li:hover i {
    color: rgb(179, 192, 199);
    }

    .card-container .title-wrapper .icon-btns ul li i {
    font-size: 25px;
    color: rgb(79, 92, 99);
    transition: .2s;
    }

</style>