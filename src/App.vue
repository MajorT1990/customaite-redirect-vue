<template>
  <div>Hello {{ value }}
    <script>
  var old = window.location.href
  if(old.includes('adore4customs')){
    var n = old.replace(/adore4customs/g, 'customaite')
    window.location.replace(n);
  } else {
    window.location.replace("https://app-dev.customaite.ai");
  }
  </script>
  
  </div>

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
