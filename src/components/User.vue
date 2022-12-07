<template>
  <span class="user">
    <span class="name">{{ usuario.name}}</span>
    <span class="handle">{{ usuario.handle }}</span>
  </span>
</template>

<script>
export default {
  props:["usuario"]
}
</script>
