<template>
<!-- Main modal -->
<div id="BookedModal" tabindex="-1" aria-hidden="true" class="fixed top-0 left-0 right-0 z-50 hidden w-full p-4 overflow-x-hidden overflow-y-auto md:inset-0 h-[calc(100%-1rem)] max-h-full">
    <div class="relative w-full max-w-2xl max-h-full">
        <!-- Modal content -->
        <div class="relative bg-white rounded-lg shadow dark:bg-white">
            <!-- Modal header -->
            <div class="flex items-start justify-between p-4 border-b rounded-t dark:border-gray-600">
                <h3 class="text-xl font-semibold text-gray-900 dark:text-black">
                    Booking
                </h3>
                <button type="button" class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ml-auto inline-flex justify-center items-center dark:hover:bg-white dark:hover:text-black" data-modal-hide="BookedModal">
                    <svg class="w-3 h-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 14">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 6 6m0 0 6 6M7 7l6-6M7 7l-6 6"/>
                    </svg>
                    <span class="sr-only">Close modal</span>
                </button>
            </div>
            <!-- Modal body -->
            <div class="p-6 space-y-6">
              <form>
                <div class="mb-6">
                  <label for="nopol" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Nopol</label>
                  <input type="text" id="nopol" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                </div>
                <div class="mb-6">
                  <div class="grid grid-cols-2 gap-4">
                    <div>
                      <label for="date_in" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Date In</label>
                    <input type="date" id="date_in" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                    </div>
                    <div>
                      <label for="date_out" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Date Out</label>
                    <input type="date" id="date_out" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                    </div>
                  </div>                  
                </div>
                <div class="mb-6">
                  <div class="grid grid-cols-2 gap-4">
                    <div>
                      <label for="time_in" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Time In</label>
                      <input type="time" id="time_in" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                    </div>
                    <div>
                      <label for="time_out" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Time Out</label>
                      <input type="time" id="time_out" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                    </div>
                  </div>                  
                </div>
                <div class="mb-6">
                  <label for="car_model" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Car Model</label>
                  <input type="text" id="car_model" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                </div>
                <div class="mb-6">
                  <label for="customer_nic" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Customer Nic</label>
                  <input type="number" id="customer_nic" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                </div>
                 <div class="mb-6">
                  <label for="customer_name" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Customer Name</label>
                  <input type="text" id="customer_name" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                </div>
                <div class="mb-6">
                  <label for="customer_name" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Customer Number</label>
                  <input type="number" id="customer_name" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                </div>
                <div class="mb-6">
                  <label for="customer_email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-black">Email (optional)</label>
                  <input type="email" id="customer_email" class="bg-white border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-white-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-black dark:focus:ring-blue-500 dark:focus:border-blue-500" required>
                </div>
              </form>
            </div>
            <!-- Modal footer -->
            <div class="flex items-center p-6 space-x-2 border-t border-gray-200 rounded-b dark:border-gray-600">
                <button data-modal-hide="BookedModal" type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Booking Now</button>
                <button data-modal-hide="BookedModal" type="button" class="text-gray-500 bg-white hover:bg-gray-100 focus:ring-4 focus:outline-none focus:ring-blue-300 rounded-lg border border-gray-200 text-sm font-medium px-5 py-2.5 hover:text-gray-900 focus:z-10 dark:bg-gray-700 dark:text-gray-300 dark:border-gray-500 dark:hover:text-white dark:hover:bg-gray-600 dark:focus:ring-gray-600">Close</button>
            </div>
        </div>
    </div>
</div>

</template>