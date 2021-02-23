<template>
    <div 
        class="border-2 rounded-md flex flex-col w-64 items-center pt-4 pb-7 px-4 space-y-4  cursor-pointer"
        :class="[value.color, value.border_color, value.texhover, value.textcolor]">
        <img :src="value.image" class="w-20 h-20">
        <span class="text-2xl font-bold uppercase"> {{value.name}}</span>
        <span class="text-center leading-tight">{{value.description}}</span>
        <a :href="value.link" target="_blank"
         class="border-2 py-4 px-10 rounded-full font-light"
         :class="[value.hovertxt, value.butborder]"
         >VIEW </a>
    </div>
</template>

<script>
export default {
    props:["value"],
}
</script>