<style lang='less'>
page {
  width: 100%;
  height: 100%;
  overflow: hidden;
  .swiper-content {
    width: 100%;
    height: 100%;
    image {
      width: 100%;
      height: 100%;
    }
  }
  video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
}
</style>
<template>
  <video id="video" custom-cache="{{false}}" bindplay="play" autoplay enable-progress-gesture="{{false}}"
  show-center-play-btn="{{false}}" controls="{{false}}" bindended="playend" src="{{current.url}}"></video>
  <swiper class="swiper-content" circular="{{true}}" vertical="{{true}}" bindchange="changeVideo">
    <swiper-item wx:for="{{list}}" wx:key="{{item.id}}">
      <image src="{{item.url}}.jpg"></image>
    </swiper-item>
  </swiper>
  <cover-view class="over" bindtouchstart="touchstart" bindtouchend="touchend">
  <cover-view>
</template>

<script>
import wepy from 'wepy'

export default class Index extends wepy.page {
  config = {
    navigationBarTitleText: '首页'
  }

  data = {
    current: {
      url: ''
    },
    list: [
      {
        'id': 75659,
        'content': '可爱的音乐加上萌萌的你，动作不协调也要跳?',
        'url': 'http://ttsoss.oss-cn-beijing.aliyuncs.com/video/bb581a99e2457da3b8116a4338d005de.0.mp4',
        'status': 0,
        'likenum': 402,
        'source': '好看'
      },
      {
        'id': 75649,
        'content': '爸爸的套路太深',
        'url': 'http://ttsoss.oss-cn-beijing.aliyuncs.com/video/60b1a204d46e9432fa24780f916753ef.0.mp4',
        'status': 0,
        'likenum': 303,
        'source': '好看'
      },
      {
        'id': 75642,
        'content': '猜谜语',
        'url': 'http://ttsoss.oss-cn-beijing.aliyuncs.com/video/80f190752361d69796f7291ba9412cf2.0.mp4',
        'status': 0,
        'likenum': 805,
        'source': '好看'
      },
      {
        'id': 75641,
        'content': '这结局亮了??',
        'url': 'http://ttsoss.oss-cn-beijing.aliyuncs.com/video/f7dc20ce1a3168f63dc6e83d3d0ebb7e.0.mp4',
        'status': 0,
        'likenum': 656,
        'source': '好看'
      },
      {
        'id': 75638,
        'content': '厉害了我的妹……???',
        'url': 'http://ttsoss.oss-cn-beijing.aliyuncs.com/video/3566469cf228f4b0d386dd34112281c6.0.mp4',
        'status': 0,
        'likenum': 1454,
        'source': '好看'
      }
    ]
  }

  methods = {
    changeVideo (e) {
      this.current = this.list[e.detail.current]
      this.$apply()
    },
    play () {
      console.log('play')
    },
    playend () {
      console.log('playend')
    },
    touchstart () {

    },
    touchend () {

    }
  }

  onLoad() {
    this.current = this.list[0]
  }
}
</script>
