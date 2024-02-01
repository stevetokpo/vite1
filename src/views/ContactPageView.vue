<template>
  <main class="h-screen lg:h-fit w-full bg-white lg:bg-gray-700">
    <section class="relative flex flex-col lg:flex-row lg:w-full lg:justify-end items-center" >
      <img src="https://i.imgur.com/1zPW5No.jpg" alt="" class="lg:w-2/3"/>
      <form
        action="#"
        class="bg-white border-4 border-gray-700 p-4 md:p-10 mx-[5%] md:w-4/5 lg:w-1/2 absolute top-[50%] lg:left-[5%] lg:top-auto rounded-3xl z-10"
      >
        <h3 class="text-2xl md:text-3xl bold font-poppins py-4">Envoyez-nous un message</h3>
        <div class="flex flex-col gap-4 md:gap-6">
          <label class="font-semibold flex flex-col gap-2 md:text-xl">
            <span>Nom et Prénom(s) <span class="font-normal">:</span></span>
            <div class="flex gap-4">
              <div>
                <input
                  type="text"
                  class="border-2 gray-500 rounded-md h-10 w-full"
                /><span class="text-sm font-extralight text-gray-400">Nom</span>
              </div>
              <div>
                <input
                  type="text"
                  class="border-2 gray-500 rounded-md h-10 w-full"
                /><span class="text-sm font-extralight text-gray-400">Prénom(s)</span>
              </div>
            </div>
          </label>
          <label class="font-semibold flex flex-col gap-2 md:text-xl">
            <span>Email <span class="font-normal">:</span></span>
            <input type="email" name="" id="" class="border-2 gray-500 rounded-md h-10">
          </label>
          <label class="font-semibold flex flex-col gap-2 md:text-xl">
            <span>Adresse <span class="font-normal">:</span></span>
            <input type="text" name="" id="" class="border-2 gray-500 rounded-md h-10">
          </label>
          <label class="font-semibold flex flex-col gap-2 md:text-xl">
            <span>Objet <span class="font-normal">:</span></span>
            <input type="text" name="" id="" class="border-2 gray-500 rounded-md h-10">
          </label>
          <label class="font-semibold flex flex-col gap-2 md:text-xl">
            <span>Votre message <span class="font-normal">:</span></span>
            <textarea class="border-2 gray-500 rounded-md h-32"></textarea>
          </label>
          <input type="submit" value="Envoyer" class="bg-gray-700 text-lg md:text-3xl lg:text-lg text-white px-6 py-2 md:px-10 rounded-3xl font-bold w-fit mx-auto">
        </div>
      </form>
    </section>
  </main>
</template>
