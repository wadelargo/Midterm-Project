<template>
  <text :class="type">
    {{ title }}
  </text>
</template>

<script>
export default {
  props: {
    title: String,
    type: String,
  },
};
</script>

<style scoped>
text {
  padding: 100px; 
  border: 1px solid black;
  margin: 10px; 
  font-size: 20px; 
  max-width: 100%; 
  box-sizing: border-box; 
  text-align: center;
  transition: background-color 0.3s; 
}

.regular,
.happy,
.sad,
.angry {
  width: 100%; /* Ensure that all text types take full width */
}

.regular {
  background-color: rgba(0, 0, 255, 0.835);
  color: white;
  border-radius: 10px;
  font-size: 25px;
}

.regular:hover {
  background-color: blue;
}

.happy {
  background-color: rgba(0, 128, 0, 0.787);
  color: white;
  border-radius: 10px;
  font-size: 25px;
}

.happy:hover {
  background-color: green;
}

.sad {
  background-color: rgba(253, 253, 12, 0.674);
  color: black;
  border-radius: 10px;
  font-size: 25px;
}

.sad:hover {
  background-color: yellow;
}

.angry {
  background-color: rgba(255, 0, 0, 0.724);
  color: white;
  border-radius: 10px;
  font-size: 25px;
}

.angry:hover {
  background-color: red;
}
</style>
