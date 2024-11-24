<script setup>
import Card from './Card.vue';
const onClickAdd = () => {
    alert('qoshish')
}
</script>

<template>
    <div class="grid grid-cols-4 gap-5">
        <Card title="Erkaklar krasofkasi Nike Blazer Mid " 
        image-url="/sneakers/sneakers-1.jpg"
        :price="100"
        :is-favorite="true"
        :onClickAdd="onClickAdd"
        />
        
      </div>
</template>