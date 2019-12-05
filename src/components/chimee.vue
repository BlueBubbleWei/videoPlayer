<template>
  <div>
    <section id="wrapper">
      <container
        style="z-index: 1; width: 100%; height: 100%; position: relative; display: block;"
      >
        <video
          tabindex="-1"
          controls=""
          width="100%"
          height="100%"
          preload="auto"
          src="https://hdl-ws.upaimv.cn/upaimv/12738928.flv"
        ></video>
      </container>
    </section>
  </div>
</template>
<script>
import ChimeePlayer from "chimee-player";
import kernelFlv from "chimee-kernel-flv";
export default {
  data() {
    return {};
  },
  created() {
    new ChimeePlayer({
      wrapper: "#wrapper", // video dom容器
      src: "https://hdl-ws.upaimv.cn/upaimv/12738928.flv",
      controls: true,
      kernels: {
        flv: kernelFlv
      }
    });
  }
};
</script>
