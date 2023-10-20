<script setup>
import jumbrotonVue from '../components/jumbroton/jumbroton.vue'
import navbarVue from '../components/navbar/navbar.vue'
import footerVue from '../components/footer/footer.vue'
import BookedModal from '../components/modal/BookedModal.vue'
import DetailModal from '../components/modal/DetailModal.vue'
</script>

<template>
  <navbarVue />
  <jumbrotonVue />

  <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4 p-3">
    <div class="max-w-sm rounded overflow-hidden shadow-lg">
      <img
        class="w-full"
        src="https://cdn.motor1.com/images/mgl/7ZmKp6/s3/chevrolet-corvette.webp"
        alt="Sunset in the mountains"
      />
      <div class="px-3 py-4">
        <div class="font-semibold text-xl col-span-2">FERRARI SPIDER</div>
        <small class="text-gray-700"> FERRARI SPIDER SPORT CARS </small>
      </div>
      <div class="px-3 grid grid-cols-2">
        <button
          type="button"
          class="text-white shadow-lg bg-blue-700 hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 font-medium rounded-full text-sm px-5 py-2.5 text-center mr-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          Booking
        </button>
        <button
          type="button"
          class="text-white shadow-lg bg-yellow-400 hover:bg-yellow-500 focus:outline-none focus:ring-4 focus:ring-yellow-300 font-medium rounded-full text-sm px-5 py-2.5 text-center mr-2 mb-2 dark:focus:ring-yellow-900"
        >
          Detail
        </button>
      </div>
    </div>
    <div class="max-w-sm rounded overflow-hidden shadow-lg">
      <img
        class="w-full"
        src="https://cdn.motor1.com/images/mgl/7ZmKp6/s3/chevrolet-corvette.webp"
        alt="Sunset in the mountains"
      />
      <div class="px-3 py-4">
        <div class="font-semibold text-xl col-span-2">FERRARI SPIDER</div>
        <small class="text-gray-700"> FERRARI SPIDER SPORT CARS </small>
      </div>
      <div class="px-3 grid grid-cols-2">
        <button
          data-modal-target="BookedModal" data-modal-toggle="BookedModal"
          type="button"
          class="text-white shadow-lg bg-blue-700 hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 font-medium rounded-full text-sm px-5 py-2.5 text-center mr-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          Booking
        </button>
        <button
          data-modal-target="DetailModal" data-modal-toggle="DetailModal"
          type="button"
          class="text-white shadow-lg bg-yellow-400 hover:bg-yellow-500 focus:outline-none focus:ring-4 focus:ring-yellow-300 font-medium rounded-full text-sm px-5 py-2.5 text-center mr-2 mb-2 dark:focus:ring-yellow-900"
        >
          Detail
        </button>
      </div>
    </div>
  </div>

  <footerVue />

  <!-- modal -->
  <BookedModal/>
  <DetailModal />
</template>
