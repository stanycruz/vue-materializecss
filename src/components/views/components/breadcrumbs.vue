<template>
  <main>

<div class="container">
  <div class="row">

    <div class="col s12 m9 l10">

      <!--  Collections Section  -->
      <div id="basic" class="section scrollspy">

        <div class="row">
          <div class="col s12">
            <p class="caption">Breadcrumbs are a good way to display your current location. This is usually used when you have multiple layers of content. </p>
            <h2 class="header">Basic</h2>

            <nav>
              <div class="nav-wrapper">
                <div class="col s12">
                  <a href="#!" class="breadcrumb">First</a>
                  <a href="#!" class="breadcrumb">Second</a>
                  <a href="#!" class="breadcrumb">Third</a>
                </div>
              </div>
            </nav>

            <br><br>
            <pre><code class="language-markup">
  &lt;nav>
    &lt;div class="nav-wrapper">
      &lt;div class="col s12">
        &lt;a href="#!" class="breadcrumb">First&lt;/a>
        &lt;a href="#!" class="breadcrumb">Second&lt;/a>
        &lt;a href="#!" class="breadcrumb">Third&lt;/a>
      &lt;/div>
    &lt;/div>
  &lt;/nav>
            </code></pre>
            <br>
          </div>
        </div>
      </div>
      <!-- End collections -->


    </div>

    <div class="col hide-on-small-only m3 l2">
      <div class="toc-wrapper">
        <div class="buysellads hide-on-small-only">
          <!-- CarbonAds Zone Code -->
          <script async type="text/javascript" src="//cdn.carbonads.com/carbon.js?zoneid=1673&serve=C6AILKT&placement=materializecss" id="_carbonads_js"></script>
        </div>
        <div style="height: 1px;">
          <ul class="section table-of-contents">
            <li><a href="#basic">Basic</a></li>
          </ul>
        </div>
      </div>
    </div>

  </div>
</div>

</main>
</template>

<script type="text/javascript">
var $ = require('jquery');
let prism = require('prismjs');

export default {
  route: {
    activate () {
      this.$nextTick(() => {
        $('.toc-wrapper').pushpin({ top: $('nav').height() });
        $('.scrollspy').scrollSpy();
        prism.highlightAll();
      });
    }
  }
};
</script>
