Effeckt.css
===========
/* 重置浏览器默认样式和 */
* {
  box-sizing: border-box; /* 改变所有元素默认盒子模型 */
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0); /* CC 去除默认边距和触摸高亮 */
}

:root {
  font-size: 10px;
  font-family: Helvetica, Arial, "Microsoft YaHei", "Droid Sans", sans-serif;
  text-size-adjust: 100%;
}

html,
body {
  position: relative;
  height: 100%;
  user-select: none;
}

body,
dl,
dd,
h1,
h2,
h3,
h4,
h5,
h6,
p,
form,
figure,
fieldset {
  margin: 0;
}

ol,
li,
ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

input,
textarea,
select,
button {
  font: inherit;
  border-radius: 0;
  outline: none;
  appearance: none;
  tap-highlight-color: rgba(0, 0, 0, 0);
}

img {
  max-width: 100%;
  vertical-align: middle;
  border: none;
}

a {
  color: #000;
  text-decoration: none;
  transition: all 0.1s;
}

b,
i,
cite {
  font-style: normal;
  font-weight: normal;
}

table {
  border-spacing: 0;
  border-collapse: collapse;
}

/* 清除浮动 */
.ks-clear::after,
.clear::after {
  display: block;
  height: 0;
  clear: both;
  content: '\20';
}

.ks-clear,
.clear {
  *zoom: 1;
}

/* flex layout */
.flex-hrz {
  display: flex;
  flex-flow: row wrap;
}

.flex-full {
  flex: 1;
}

.flex-init {
  flex: initial;
}


**A Performant Transitions and Animations Library** : [http://h5bp.github.io/Effeckt.css](http://h5bp.github.io/Effeckt.css)

Ever notice how small flourishes and subtle transitions dramatically increases the value of the experience you enjoy with an app or site?

Designing and developing UIs for the mobile web is tricky, but it's extremely difficult to do that while delivering something that performs at 60fps. The best opportunities to getting jank-free transitions on phones/tablets are CSS transition and keyframe animation based, especially tapping into hardware-accelerated transforms and opacity changes.

@daneden did really nice work with [Animate.css](http://daneden.me/animate/) but I think the web would benefit if we could take that work to the next level. There's already been fantastic experiments and demos exploring CSS-based transitions, but it's distributed all over.

Originally started at [h5bp/lazyweb-requests#122](https://github.com/h5bp/lazyweb-requests/issues/122)

#### Effeckt Trailer

<a href="http://youtu.be/Qc40YDFA4Bg">![image](https://f.cloud.github.com/assets/39191/725426/aa3af38c-e067-11e2-82e4-269086cb845d.png)</a>

## Examples To Add

* [tympanus.net/Development/ModalWindowEffects/](http://tympanus.net/Development/ModalWindowEffects/)
* [tympanus.net/Development/PageTransitions/](http://tympanus.net/Development/PageTransitions/)
* [tympanus.net/Development/PFold/index2.html](http://tympanus.net/Development/PFold/index2.html)
* [leaverou.github.io/animatable/](http://leaverou.github.io/animatable/)
* [lab.hakim.se/ladda/](http://lab.hakim.se/ladda/)
* [lab.hakim.se/kontext/](http://lab.hakim.se/kontext/)
* [lab.hakim.se/avgrund/](http://lab.hakim.se/avgrund/)
* [lab.hakim.se/meny/](http://lab.hakim.se/meny/)

Because there are so many, I expect we could **group things by role**:

* button/touch effects
* state transition
* modal/notification transition
* attention attractors

## Goals

1. Provide a minimal UI. Only use style hooks for transitions and animations.
1. Designer-curated set of classy and reasonable effects. (no [`easeInBounce`](http://easings.net/#easeInBounce))
1. Establish browser support guidelines (e.g. Android 2.3 would gracefully degrade)
1. CSS performance regression testing (a la [bench.topcoat.io](http://bench.topcoat.io))
1. Deliver jank-free *60fps* performance on target browsers/devices
1. If a particular effect cannot deliver target performance (hey `blur()` css filter), it cannot be included.
1. Guidelines on what to avoid when styling these affected elements (avoid expensive CSS)
1. Deliver a builder so users can pull only the CSS they need.
1. There is no hover on the mobile web, so any hover-based effects would be excluded or have a tap-based equivalent.

## Action

* If you know other transition/animation based demos/experiments that make sense to include here, file a ticket.
* If you're interested in helping to define the API, let's hear it! File a ticket.
* A web-based builder is a must. A command-line builder isn't important for this.

## Getting Started

- [https://github.com/h5bp/Effeckt.css/wiki/Getting-Started](https://github.com/h5bp/Effeckt.css/wiki/Getting-Started)

## Code Style Guide

- [https://github.com/h5bp/Effeckt.css/wiki/Code-Style-Guide](https://github.com/h5bp/Effeckt.css/wiki/Code-Style-Guide)

## General Inquiries & Support

- Effeckt.css Mailing List [https://groups.google.com/d/forum/effeckt](https://groups.google.com/d/forum/effeckt)

## Bug Reports & Feature Requests

- [http://github.com/h5bp/Effeckt.css/issues](https://github.com/h5bp/Effeckt.css/issues)
