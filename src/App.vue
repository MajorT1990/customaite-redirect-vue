<template>
  <div>Redirecting to the new domain..</div>

</template>

<script>
export default {
  name: "App",
  data() {
    return {
      value: "World"
    };
  },
  beforeMount() {
    var old = window.location.href
    if(old.includes('adore4customs')){
      var n = old.replace(/adore4customs/g, 'customaite')
      window.location.replace(n);
    } else {
      window.location.replace("https://app-dev.customaite.ai");
    }
}
};
</script>
