<template>
    <div>
        <div class="flex h-full overflow-hidden">
            <img v-if="!displayImg" src="https://picsum.photos/id/234/800/316" class="mx-auto">
            <img v-else :src="showImg.src" :alt="showImg.alt" class="mx-auto">
        </div>
        <div class="flex justify-center mt-4">
            <span v-for="(img,i) in imgs" :key="i" class="mx-4 outline-none cursor-pointer" @click="setImg(img)"><i class="text-xs text-gray-600 fa fa-circle"></i></span>
        </div>
    </div>
</template>

<script>
    export default {
        data:()=>({
            displayImg:false,
            showImg:{
                src:"",
                alt:""
            },
            imgs:[
                {src:"https://picsum.photos/id/237/800/316", alt:"imagen de perro"},
                {src:"https://picsum.photos/id/236/800/316", alt:"imagen de casa"},
                {src:"https://picsum.photos/id/235/800/316", alt:"imagen de montaña"},
                {src:"https://picsum.photos/id/234/800/316", alt:"imagen de torre eifel"},
            ]
        }),
        methods:{
            setImg(img){
                this.displayImg= true;
                this.showImg.src=img.src
                this.showImg.alt=img.alt
                return;
            }

        }
    }
</script>