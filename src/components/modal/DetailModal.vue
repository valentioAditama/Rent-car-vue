<template>
  <!-- Main modal -->
  <div id="DetailModal" tabindex="-1" aria-hidden="true" class="fixed top-0 left-0 right-0 z-50 hidden w-full p-4 overflow-x-hidden overflow-y-auto md:inset-0 h-[calc(100%-1rem)] max-h-full">
      <div class="relative w-full max-w-3xl max-h-full">
          <!-- Modal content -->
          <div class="relative bg-white rounded-lg shadow dark:bg-white">
              <!-- Modal header -->
              <div class="flex items-start justify-between p-4 border-b rounded-t dark:border-gray-600">
                  <h3 class="text-xl font-semibold text-gray-900 dark:text-black">
                      Detail
                  </h3>
                  <button type="button" class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ml-auto inline-flex justify-center items-center dark:hover:bg-white dark:hover:text-black" data-modal-hide="DetailModal">
                      <svg class="w-3 h-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 14">
                          <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 6 6m0 0 6 6M7 7l6-6M7 7l-6 6"/>
                      </svg>
                      <span class="sr-only">Close modal</span>
                  </button>
              </div>
              <!-- Modal body -->
              <div class="p-6 space-y-6">
                <div class="grid grid-cols-2">
                  <div>
                    <div class="mb-6">
                    <label for="nopol" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Nopol</label>
                    <input type="text" id="nopol" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="brand" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Brand</label>
                    <input type="text" id="brand" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="car_model" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Car Model</label>
                    <input type="text" id="car_model" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="kilometer" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Kilometer</label>
                    <input type="number" id="kilometer" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="color" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Color</label>
                    <input type="text" id="color" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="passengers" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Passengers</label>
                    <input type="number" id="passengers" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="detail" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Detail</label>
                    <input type="text" id="detail" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  <div class="mb-6">
                    <label for="status_car" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Status Car</label>
                    <input type="text" id="status_car" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                  </div>
                  </div>
                  <div class="flex items-center">
                   <div class="grid-rows-3 ml-5">
                    <img
                      class="w-full h-54 object-cover"
                      src="https://cdn.motor1.com/images/mgl/7ZmKp6/s3/chevrolet-corvette.webp"
                      alt="Sunset in the mountains"
                    />
                     <img
                      class="w-full h-54 object-cover"
                      src="https://cdn.motor1.com/images/mgl/7ZmKp6/s3/chevrolet-corvette.webp"
                      alt="Sunset in the mountains"
                    />
                     <img
                      class="w-full h-54 object-cover"
                      src="https://cdn.motor1.com/images/mgl/7ZmKp6/s3/chevrolet-corvette.webp"
                      alt="Sunset in the mountains"
                    />
                   </div>
                  </div>
                </div>
              </div>
              <!-- Modal footer -->
              <div class="flex items-center p-6 space-x-2 border-t border-gray-200 rounded-b dark:border-gray-600">
                  <button data-modal-hide="DetailModal" type="button" class="text-gray-500 bg-white hover:bg-gray-100 focus:ring-4 focus:outline-none focus:ring-blue-300 rounded-lg border border-gray-200 text-sm font-medium px-5 py-2.5 hover:text-gray-900 focus:z-10 dark:bg-gray-700 dark:text-gray-300 dark:border-gray-500 dark:hover:text-white dark:hover:bg-gray-600 dark:focus:ring-gray-600">Close</button>
              </div>
          </div>
      </div>
  </div>
  
  </template>