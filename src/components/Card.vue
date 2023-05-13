<template>
    <div class="card">
        <div class="card-image-wrapper">
            <img :src="imageUrl" :alt="title" class="card-image" />
        </div>
        <div class="card-content">
            <h3 class="card-title">{{ title }}</h3>
            <p class="card-description">{{ description }}</p>
            <button class="start-button">Start</button>
        </div>
    </div>
</template>
  
  
<script>
export default {
    props: {
        title: {
            type: String,
            required: true,
        },
        imageUrl: {
            type: String,
            required: true,
        },
        description: {
            type: String,
            required: true,
        },
    },
};
</script>
  