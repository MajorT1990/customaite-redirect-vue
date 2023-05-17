<template>
  <div>Hello {{ value }}</div>
  <script>
  var old = window.location.href
  if(old.includes('adore4customs')){
    var n = old.replace(/adore4customs/g, 'customaite')
    window.location.replace(n);
  } else {
    window.location.replace("https://app-dev.customaite.ai");
  }
  </script>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      value: "World"
    };
  }
};
</script>
