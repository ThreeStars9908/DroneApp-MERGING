<template>
  <div class="page">
    <div class="navbar">
      <div class="navbar-bg"></div>
      <div class="navbar-inner sliding">
        <div class="left">
          <Link back>
            <i class="icon icon-back"></i>
            <span class="if-not-md">Back</span>
          </Link>
        </div>
        <div class="title">Page Transitions</div>
      </div>
    </div>
    <div class="page-content">
      <div class="block block-strong">
        <p>In addition to default theme-specific page transition it is possible to create custom page transition or use
          one of the additional transition effects:</p>
      </div>
      <div class="list links-list">
        <ul>
          ${effects.map((effect) => $h`
          <li><a href="/page-transitions/${effect}" data-transition="${effect}">${effect}</a></li>
          `)}
        </ul>
      </div>
    </div>
  </div>
</template>
<!-- <script>
  export default () => {
    const effects = ['f7-circle', 'f7-cover', 'f7-cover-v', 'f7-dive', 'f7-fade', 'f7-flip', 'f7-parallax', 'f7-push']
    return $render;
  }
</script> -->

<script>
  import { Link } from 'framework7-svelte';
</script>