<template>
  <div class="mt-10">
    <h5 class="pl-4 text-2xl font-bold text-gray-800">Trabajemos juntos..</h5>
    <div class="flex justify-center mt-10">
      <form @submit.prevent="sendForm">
        <label for="emial" class="flex flex-col">
            <span class="mb-1">Tu correo</span>
          <input type="email" id="emial" class="p-2 tracking-wide bg-gray-100 border border-transparent rounded outline-none focus:bg-white focus:border-gray-700" autocomplete="off" placeholder="mi@empresa.com" required/>
        </label>
        <label for="contact" class="flex flex-col mt-6">
            <span class="mb-1">Tu propuesta</span>
            <textarea name="" id="contact" cols="30" rows="10" class="p-2 tracking-wide bg-gray-100 border border-transparent rounded outline-none focus:border-gray-700 focus:bg-white"></textarea>
        </label>
        <div class="mt-4 text-center ">
        <button type="submit" class="p-2 mx-auto text-white transition duration-150 ease-in bg-indigo-300 border border-transparent rounded hover:bg-white hover:border-indigo-300 hover:text-black">Enviar</button>

        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    sendForm() {
      console.log("ENVIO EL FORMULARIO");
    },
  },
};
</script>

<style lang="scss" scoped></style>
