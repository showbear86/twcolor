<template>
    <div class="range-slider">
      <div ref="slider_thumb" class="range-slider_thumb" :style="`left:${bulletPosition}px;`"> {{ attrSide }}-{{ range[slider_input] }}</div>
      <div class="range-slider_line">
        <div ref="slider_line" class="range-slider_line-fill" :style="`width:${slider_input * (100 / (range.length-1))}%;`"></div>
      </div>
      <input v-model="slider_input" ref="inputSlider" class="range-slider_input" type="range" min="0" :max="range.length-1">
    </div>
</template>

<script setup>
import {ref, onMounted, defineEmits, computed, watch} from 'vue';

const props = defineProps({
  modelValue: {
      default: {},
  },
  attrSide: {
    type: String
  },
  range: {
      type: Array
  }
});


const emit = defineEmits(['update:modelValue']);
const slider_input = ref(props.range.indexOf(props.modelValue));
const slider_line = ref(null);
const slider_thumb = ref(null);
const bulletPosition = ref(null);
const inputSlider = ref(null);

onMounted(() => {
    bulletPosition.value = (slider_input.value / (props.range.length-1)) * (inputSlider.value.offsetWidth - slider_thumb.value.offsetWidth);
});

watch(slider_input, ()=> {
  bulletPosition.value = (slider_input.value / (props.range.length-1)) * (inputSlider.value.offsetWidth - slider_thumb.value.offsetWidth);
  emit('update:modelValue', props.range[slider_input.value]);
});

</script>
  
<style scoped>
.range-slider {
	position: relative;
  min-height:5vmin;
}

.range-slider_input {
	width: 100%;
	position: absolute;
	top: 50%;
	z-index: 3;
	transform: translateY(-50%);
	-webkit-appearance: none;
  appearance: none;
  width: 100%;
  opacity: 0;
	margin: 0;
}

.range-slider_input::-webkit-slider-thumb {
  -webkit-appearance: none;
  appearance: none;
  width: 100px;
  height: 100px;
  cursor: pointer;
	border-radius: 50%;
	opacity: 0;
}

.range-slider_input::-moz-range-thumb {
  width: 14vmin;
  height: 14vmin;
  cursor: pointer;
	border-radius: 50%;
	opacity: 0;
}

.range-slider_thumb {
	width: 8vmin;
	padding:0.35rem 0 0.45rem 0;
	border-width: 0.45vmin;
  border-style:solid;
	border-radius: 50%;
	position: absolute;
	left: 0;
	top: 50%;
	transform: translateY(-50%) translateX(1px);
	display: flex;
	justify-content: center;
	align-items: center;
	font-weight: 700;
	color: #303030;
	z-index: 2;
  @apply border-sky-400 bg-white text-sky-600 text-sm;

}

.range-slider_line {
	height: 0.7vmin;
	width: 100%;
	background-color: #e1e1e1;
	top: 50%;
	transform: translateY(-50%);
	left: 0;
	position: absolute;
  border-radius:999px;
	z-index: 1;
}

.range-slider_line-fill {
	position: absolute;
	height: 0.7vmin;
	width: 0;
  border-radius:999px;
  @apply bg-gradient-to-r from-sky-600 via-sky-500 to-sky-400;
}

</style>