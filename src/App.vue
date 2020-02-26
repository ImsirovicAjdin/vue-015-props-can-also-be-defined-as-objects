<template>
  <div id="app">
    <HelloWorld :message="datacontent"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  data() {
    return {
      datacontent: `This content was passed from App's data function
       to the Vue component called HelloWorld.
       The data was bound to HelloWorld's "message" prop using the 
       shorthand v-bind syntax.
       the data passed was also validated using the "message" prop 
       by ensuring that it's type is String and that it is required.`
    };
  }
};
</script>

