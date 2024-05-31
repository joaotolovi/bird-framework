<script setup>
import { ref } from 'vue';

const props = defineProps({
  url: String,
  useNextImage: Boolean,
});

const logoSrc = ref(props.useNextImage? '/_next/image?url=%2Fassets%2Fimages%2Flogo.png&w=48&q=75' : '/assets/images/logo.png');
const logoWordsSrc = ref('/assets/images/logo-words.svg');
</script>
