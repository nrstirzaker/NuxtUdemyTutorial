<template>
  <h1>A single user, with Id: {{$route.params.id}} page</h1>
</template>
<script>
export default {
  validate (data) {
    console.log(data);
    return !isNaN(data.params.id);
  }
}
</script>