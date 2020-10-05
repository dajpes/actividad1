<template>
    <div>
        <div class="flex justify-between p-4 mt-16">
            <div v-for="(item,id) in info" :key="id" class="w-1/4 mx-4 text-center ">
                <div class="text-4xl text-blue-400">
                    <i class="fas" :class="item.icon"></i>
                </div>
                <p class="mt-4 text-sm text-gray-700">{{item.text}}</p>
            </div>
        </div>
        <div class="mt-16">
            <h5 class="p-4 text-3xl font-bold text-gray-700 ">Encuentranos..</h5>
            <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d6687.694562514694!2d-74.04901023650419!3d4.678063627822335!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1ses-419!2sco!4v1601918321923!5m2!1ses-419!2sco" width="600" height="450" frameborder="0" style="border:0;"  aria-hidden="false" tabindex="0" class="w-full"></iframe>
        </div>
    </div>
</template>

<script>
    export default {
        data:()=>({
            info:[
                {text:"Nos encargamos de desarrollar sus páginas web rápidas, seguras y confiables",icon:"fa-shipping-fast"},
                {text:"Tenemos los mejores precios del mercado Colombiano, sin desmerecer la calidad del producto",icon:"fa-dollar-sign"},
                {text:"Le ayudamos a posicionar su página web en los primeros resultados de los más importantes buscadores",icon:"fa-search-location"},
            ]
        })
    }
</script>

<style lang="scss" scoped>

</style>