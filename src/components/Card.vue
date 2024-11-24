<script setup>
defineProps({
  title: String,
  imageUrl: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickFavorite: Function
})

</script>

<template>
  <div
    class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer hover:-translate-y-2 hover:shadow-xl transition"
  >
    
    <img 
     :src=" !isAdded ? '/liked.svg' : '/unliked.svg'"
      alt=""
      @click="onClickFavorite"
    />

    <img :src="imageUrl" alt="" />

    <p class="mt-2">{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Narx</span>
        <b>{{ price }} $</b>
      </div>

      <img @click="onClickAdd" :src=" !isAdded ? '/btn-plus.svg' : '/btn-checked.svg'" alt="" />
    </div>
  </div>
</template>
