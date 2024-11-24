<template>
     <header class="flex justify-between border-b border-slate-200 px-10 py-8">
      <div class="flex items-center gap-4">
        <img src="/logo.png" alt="" class="w-10" />

        <div>
          <h2 class="text-xl font-bold uppercase">Vue Sneakers</h2>
          <p class="text-slate-400">Eng yahshi Krasofkalar</p>
        </div>
      </div>

      <ul class="flex items-center gap-10">
        <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
          <img src="/cart.svg" alt="" />
          <b>100 $</b>
        </li>

        <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
          <img src="/heart.svg" alt="" />
          <span>Yoqtirgan</span>
        </li>
        <li class="flex items-center cursor-pointer gap-3 text-gray-500 hover:text-black">
          <img src="/user.svg" alt="" />
          <span>User</span>
        </li>
      </ul>
    </header>
</template>