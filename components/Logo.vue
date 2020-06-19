<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
          <b-img class="NuxtLogo" fluid-grow src="../static/hw-logo.svg" ></b-img>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<style>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
