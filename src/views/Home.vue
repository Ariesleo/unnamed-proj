<template>
  <div class="home">
    <HelloWorld />
    <ButtonLists />
    <TextBox />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import TextBox from '@/components/TextBox.vue';
import ButtonLists from '@/components/ButtonLists.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
    TextBox,
    ButtonLists,
  },
};
</script>
