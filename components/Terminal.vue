<template>
  <div class="terminal">
    <div class=fakeMenu>
      <div class="fakeButtons fakeClose"></div>
      <div class="fakeButtons fakeMinimize"></div>
      <div class="fakeButtons fakeZoom"></div>
    </div>
    <div class="fakeScreen">
      <p class="line1">$ Hello I'm Jaume. <span class="wave">👋</span><span class="cursor1">_</span></p>
      <p class="line2">$ I'm a full stack web developer.<span class="cursor2">_</span></p>
      <p class="line3">&nbsp;&nbsp;&ldquo;Let's work together!&rdquo;&nbsp;&#93;<span class="cursor3">_</span></p>
      <p class="line4">><span class="cursor4">_</span></p>
    </div>
  </div>

</template>

<script>
  export default {
    name: "Terminal"
  }
</script>

<style scoped>

  .fakeButtons {
    height: 10px;
    width: 10px;
    border-radius: 50%;
    border: 1px solid #000;
    position: relative;
    top: 6px;
    left: 6px;
    background-color: #ff3b47;
    border-color: #9d252b;
    display: inline-block;
  }

  .fakeMinimize {
    left: 11px;
    background-color: #ffc100;
    border-color: #9d802c;
  }

  .fakeZoom {
    left: 16px;
    background-color: #00d742;
    border-color: #049931;
  }

  .fakeMenu {
    width: 400px;
    box-sizing: border-box;
    height: 25px;
    background-color: #bbb;
    margin: 0 auto;
    border-top-right-radius: 5px;
    border-top-left-radius: 5px;
    display:flex;
  }

  .fakeScreen {
    background-color: #151515;
    box-sizing: border-box;
    width: 400px;
    margin: 0 auto;
    padding: 20px;
    border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px;
  }

  p {
    /*position: relative;*/
    left: 50%;
    /*margin-left: -10.5em;*/
    text-align: left;
    font-size: 1.25em;
    font-family: monospace;
    white-space: nowrap;
    overflow: hidden;
  }

  span {
    color: #fff;
    font-weight: bold;
  }

  .line1 {
    color: #9CD9F0;
    -webkit-animation: type .5s 1s steps(20, end) forwards;
    -moz-animation: type .5s 1s steps(20, end) forwards;
    -o-animation: type .5s 1s steps(20, end) forwards;
    animation: type .5s 1s steps(20, end) forwards;
  }

  .cursor1 {
    -webkit-animation: blink 1s 2s 2 forwards;
    -moz-animation: blink 1s 2s 2 forwards;
    -o-animation: blink 1s 2s 2 forwards;
    animation: blink 1s 2s 2 forwards;
  }

  .line2 {
    color: #CDEE69;
    -webkit-animation: type .5s 4.25s steps(20, end) forwards;
    -moz-animation: type .5s 4.25s steps(20, end) forwards;
    -o-animation: type .5s 4.25s steps(20, end) forwards;
    animation: type .5s 4.25s steps(20, end) forwards;
  }

  .cursor2 {
    -webkit-animation: blink 1s 5.25s 2 forwards;
    -moz-animation: blink 1s 5.25s 2 forwards;
    -o-animation: blink 1s 5.25s 2 forwards;
    animation: blink 1s 5.25s 2 forwards;
  }

  .line3 {
    color: #E09690;
    -webkit-animation: type .5s 7.5s steps(20, end) forwards;
    -moz-animation: type .5s 7.5s steps(20, end) forwards;
    -o-animation: type .5s 7.5s steps(20, end) forwards;
    animation: type .5s 7.5s steps(20, end) forwards;
  }

  .cursor3 {
    -webkit-animation: blink 1s 8.5s 2 forwards;
    -moz-animation: blink 1s 8.5s 2 forwards;
    -o-animation: blink 1s 8.5s 2 forwards;
    animation: blink 1s 8.5s 2 forwards;
  }

  .line4 {
    color: #fff;
    -webkit-animation: type .5s 10.75s steps(20, end) forwards;
    -moz-animation: type .5s 10.75s steps(20, end) forwards;
    -o-animation: type .5s 10.75s steps(20, end) forwards;
    animation: type .5s 10.75s steps(20, end) forwards;
  }

  .cursor4 {
    -webkit-animation: blink 1s 11.5s infinite;
    -moz-animation: blink 1s 8.5s infinite;
    -o-animation: blink 1s 8.5s infinite;
    animation: blink 1s 8.5s infinite;
  }

  @-webkit-keyframes blink {
    0% {
      opacity: 0;
    }
    40% {
      opacity: 0;
    }
    50% {
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }

  @-moz-keyframes blink {
    0% {
      opacity: 0;
    }
    40% {
      opacity: 0;
    }
    50% {
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }

  @-o-keyframes blink {
    0% {
      opacity: 0;
    }
    40% {
      opacity: 0;
    }
    50% {
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }

  @keyframes blink {
    0% {
      opacity: 0;
    }
    40% {
      opacity: 0;
    }
    50% {
      opacity: 1;
    }
    90% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }

  @-webkit-keyframes type {
    to {
      width: 17em;
    }
  }

  @-moz-keyframes type {
    to {
      width: 17em;
    }
  }

  @-o-keyframes type {
    to {
      width: 17em;
    }
  }

  @keyframes type {
    to {
      width: 17em;
    }
  }

  span.wave {
    animation-name: wave-animation;
    animation-duration: 2s;
    animation-iteration-count: infinite;
    transform-origin: 70% 70%;
    display: inline-block;
  }

  @keyframes wave-animation {
    0% {
      transform: rotate(0.0deg)
    }
    10% {
      transform: rotate(-10.0deg)
    }
    20% {
      transform: rotate(12.0deg)
    }
    30% {
      transform: rotate(-10.0deg)
    }
    40% {
      transform: rotate(9.0deg)
    }
    50% {
      transform: rotate(0.0deg)
    }
    100% {
      transform: rotate(0.0deg)
    }
  }

</style>
