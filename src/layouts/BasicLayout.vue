<template>
  <div id="basicLayout">
    <a-layout style="height: 488px">
      <a-layout-header class="header">
        <GlobalHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer">
        <a href="http://localhost:8080" target="_blank"> design by 金涵博 </a>
      </a-layout-footer>
    </a-layout>
  </div>
</template>

<style>
#basicLayout {
}
#basicLayout .content {
  background: Linear-gradient(to right, #bbb, #fff);
  margin-bottom: 16px;
}
#basicLayout .footer {
  background: #efefef;
  padding: 16px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  text-align: center;
}
</style>
<script>
import GlobalHeader from "@/components/GlobalHeader";
export default {
  components: { GlobalHeader },
};
</script>
