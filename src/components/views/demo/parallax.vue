<template>

<header id="demoHeader">
  <nav>
    <div class="container">
      <div class="nav-wrapper">
        <a href="index.html" class="brand-logo">Materialize</a>
        <ul class="right side-nav" id="nav-mobile">
          <li class="hide-on-small-only"><a href="parallax.html"><i class="mdi-navigation-arrow-back"></i></a></li>
        </ul>
        <a class="button-collapse" href="#" data-activates='nav-mobile'><i class="mdi-navigation-menu"></i></a>
      </div>
    </div>
  </nav>
</header>


<!--  Parallax Section  -->
<div class="parallax-container">
  <div class="parallax"><img src="http://materializecss.com/images/parallax1.jpg"></div>
</div>
<div class="section white">
  <div class="row container">
    <h2 class="header">Parallax</h2>
    <p class="grey-text text-darken-3 lighten-3">Parallax is an effect where the background content or image in this case, is moved at a different speed than the foreground content while scrolling.</p>
  </div>
  <div class="row container">
    <h4 class="light">Parallax Demo HTML</h4>
    <pre><code class="language-markup col s12">
&lt;div class="parallax-container">
  &lt;div class="parallax">&lt;img src="http://materializecss.com/images/parallax1.jpg">&lt;/div>
&lt;/div>
&lt;div class="section white">
  &lt;div class="row container">
    &lt;h2 class="header">Parallax&lt;/h2>
    &lt;p class="grey-text text-darken-3 lighten-3">Parallax is an effect where the background content or image in this case, is moved at a different speed than the foreground content while scrolling.&lt;/p>
  &lt;/div>
&lt;/div>
&lt;div class="parallax-container">
  &lt;div class="parallax">&lt;img src="http://materializecss.com/images/parallax2.jpg">&lt;/div>
&lt;/div>
    </code></pre>
  </div>
</div>
<div class="parallax-container">
  <div class="parallax"><img src="http://materializecss.com/images/parallax2.jpg"></div>
</div>

</template>

<script type="text/javascript">

var $ = require('jquery');
let prism = require('prismjs');

export default {
  route: {
    activate () {
      this.$nextTick(() => {
        $('.parallax').parallax();
        prism.highlightAll();
      });
    }
  }
}

</script>

<style media="screen" lang="sass">
  #demoHeader {
    padding-left: 0;
  }
</style>
