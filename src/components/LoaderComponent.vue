<template>
  <tr className="loader_inner">
    <td className="loader_box">
      <div className="loader"></div>
    </td>
  </tr>
</template>

<style scoped>
.loader_box {
  position: fixed;
  top: 50%;
  left: 50%;
}

.loader {
  color: #7ebc3c;
  font-size: 10px;
  position: relative;
  transform: translateZ(0);
  animation-delay: -0.16s;
}

.loader,
.loader:before,
.loader:after {
  border-radius: 50%;
  width: 25px;
  height: 25px;
  animation-fill-mode: both;
  animation: load 1.8s infinite ease-in-out;
}

.loader:before,
.loader:after {
  content: '';
  position: absolute;
  top: 0;
}

.loader:before {
  left: -3.5em;
  animation-delay: -0.32s;
}

.loader:after {
  left: 3.5em;
}

@-webkit-keyframes load {
  0%,
  80%,
  100% {
    box-shadow: 0 2.5em 0 -1.3em;
  }
  40% {
    box-shadow: 0 2.5em 0 0;
  }
}

@keyframes load {
  0%,
  80%,
  100% {
    box-shadow: 0 2.5em 0 -1.3em;
  }
  40% {
    box-shadow: 0 2.5em 0 0;
  }
}
</style>
