<template>
  <div class="self-wrap">
    <div class="self-wrap-head">
      <slot name="head"></slot>
    </div>
    <div class="self-wrap-info">
      <p class="name"><slot name="name"></slot></p>
      <div class="msg"><slot name="msg"></slot></div>
    </div>
  </div>
</template>

<script>

</script>

<style>
    .self-wrap{
        text-align: right;
        color: #000;
    }
    .self-wrap-head{
        width: 4.2rem;
        height: 4.2rem;
        float: right;
    }
    .self-wrap-info{
        margin-left: 4rem;
        margin-right: 5.2rem;
    }
    .self-wrap-info .name{
        margin-top: .4rem;
        line-height: 1;
        font-size: 1.2rem;
        color: #999;
    }
    .self-wrap-info .msg{
        display: inline-block;
        position: relative;
        margin-top:.6rem;
        padding: .1rem .6rem;
        border-radius: .4rem;
        font-size: 1.6rem;
        text-align: left;
        word-break:break-all;
        background-color: #a0e24d;
    }
    .self-wrap-info .msg:before{
        content: '';
        position: absolute;
        top: .8rem;
        left: 100%;
        display: block;
        width: 0;
        height: 0;
        border-top: .4rem solid transparent;
        border-left: .4rem solid #a0e24d;
        border-bottom: .4rem solid transparent;
    }
</style>
