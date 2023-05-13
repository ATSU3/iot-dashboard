<template>
    <div class="list">
        <h2>Choose the Dish</h2>
        <Card v-for="(item, index) in items" :key="index" :title="item.title" :imageUrl="item.imageUrl"
            :description="item.description" />
    </div>
</template>
  
<script>
import Card from "./Card.vue";

export default {
    components: {
        Card,
    },
    data() {
        return {
            items: [
                {
                    title: "Item 1",
                    imageUrl: "https://picsum.photos/300/300",
                    description: "This is the description for Item 1.",
                },
                {
                    title: "Item 2",
                    imageUrl: "https://picsum.photos/300/300",
                    description: "This is the description for Item 2.",
                },
                {
                    title: "Item 3",
                    imageUrl: "https://picsum.photos/300/300",
                    description: "This is the description for Item 3.",
                },
            ],
        };
    },
};
</script>

  