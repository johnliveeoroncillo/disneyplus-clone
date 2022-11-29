<template>
    <div class="w-full">
        <div class="mt-16 flex flex-col gap-2 inter-semibold text-left">
            <h1 class="on-surface-sec font-semibold text-xl">Enter code sent to</h1>
            <h1 class="on-surface text-2xl flex flex-row justify-between">
                <p class="inter-semibold">+63 9XXXXXXXXX</p>
                
                <button class="font-medium flex flex-row gap-2 items-center text-lg" @click="$root.$emit('login')">
                    <svg class="w-5 h-5" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" zoomAndPan="magnify" viewBox="0 0 375 374.999991" preserveAspectRatio="xMidYMid meet" version="1.0"><path fill="#ffffff" d="M 80.179688 334.480469 L 120.21875 322.730469 C 123.464844 321.761719 126.542969 320.40625 129.445312 318.664062 C 132.351562 316.921875 135 314.847656 137.386719 312.441406 L 322.066406 127.761719 C 336.363281 113.46875 337.757812 91.609375 325.179688 79.03125 L 296.886719 50.738281 C 284.308594 38.148438 262.449219 39.554688 248.15625 53.851562 L 63.476562 238.53125 C 61.070312 240.914062 59 243.5625 57.257812 246.464844 C 55.515625 249.371094 54.15625 252.445312 53.1875 255.691406 L 41.4375 295.738281 C 40.992188 297.085938 40.640625 298.457031 40.382812 299.851562 C 40.125 301.25 39.960938 302.65625 39.890625 304.074219 C 39.824219 305.492188 39.851562 306.90625 39.976562 308.320312 C 40.101562 309.734375 40.320312 311.132812 40.636719 312.519531 C 40.949219 313.902344 41.359375 315.257812 41.855469 316.589844 C 42.355469 317.917969 42.941406 319.207031 43.617188 320.457031 C 44.289062 321.707031 45.042969 322.902344 45.882812 324.050781 C 46.71875 325.199219 47.628906 326.28125 48.613281 327.304688 C 50.023438 328.703125 51.5625 329.949219 53.222656 331.039062 C 54.882812 332.132812 56.632812 333.050781 58.476562 333.792969 C 60.320312 334.535156 62.21875 335.089844 64.171875 335.457031 C 66.125 335.824219 68.09375 335.996094 70.078125 335.96875 C 73.519531 335.957031 76.882812 335.460938 80.179688 334.480469 Z M 265.472656 71.167969 C 266.765625 69.796875 268.265625 68.71875 269.976562 67.929688 C 271.683594 67.140625 273.480469 66.695312 275.363281 66.597656 C 276.132812 66.554688 276.878906 66.660156 277.609375 66.910156 C 278.335938 67.164062 278.992188 67.542969 279.570312 68.050781 L 307.867188 96.347656 C 310.457031 98.941406 309.675781 105.519531 304.753906 110.445312 L 276.410156 138.789062 L 237.128906 99.507812 Z M 64.933594 302.636719 L 76.683594 262.582031 C 77.492188 259.996094 78.859375 257.75 80.792969 255.84375 L 219.816406 116.824219 L 259.09375 156.101562 L 120.070312 295.128906 C 118.164062 297.058594 115.917969 298.425781 113.332031 299.234375 L 73.285156 310.984375 C 72.683594 311.234375 72.058594 311.40625 71.414062 311.492188 C 70.765625 311.578125 70.117188 311.574219 69.472656 311.488281 C 68.824219 311.402344 68.203125 311.230469 67.601562 310.976562 C 67 310.722656 66.445312 310.394531 65.929688 309.992188 C 65.527344 309.476562 65.199219 308.921875 64.945312 308.320312 C 64.691406 307.71875 64.519531 307.097656 64.433594 306.449219 C 64.34375 305.804688 64.34375 305.15625 64.429688 304.507812 C 64.515625 303.863281 64.683594 303.238281 64.933594 302.636719 Z M 64.933594 302.636719 " fill-opacity="1" fill-rule="nonzero"/></svg>
                    Edit
                </button>
            </h1>

            <div class="flex flex-row gap-2 mt-3">
                <input class="border border-blue-200 !border-red-600 border-opacity-40 bg-transparent text-lg text-center font-medium on-surface rounded-lg w-[50px] px-4 py-3" v-for="d in 4" :key="d" value="2">    
            </div>

            <span class="text-red-600 font-semibold text-sm">Incorrect code entered. Please enter again.</span>

            <div class="flex flex-row mt-4 gap-8">
                <button class="on-surface inter-semibold tracking-wide text-lg flex flex-row gap-2">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 mt-[3px]">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12.76c0 1.6 1.123 2.994 2.707 3.227 1.068.157 2.148.279 3.238.364.466.037.893.281 1.153.671L12 21l2.652-3.978c.26-.39.687-.634 1.153-.67 1.09-.086 2.17-.208 3.238-.365 1.584-.233 2.707-1.626 2.707-3.228V6.741c0-1.602-1.123-2.995-2.707-3.228A48.394 48.394 0 0012 3c-2.392 0-4.744.175-7.043.513C3.373 3.746 2.25 5.14 2.25 6.741v6.018z" />
                    </svg>

                    Resend code
                </button>

                <button class="on-surface inter-semibold tracking-wide text-lg flex flex-row gap-2">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 mt-[3px]">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M20.25 3.75v4.5m0-4.5h-4.5m4.5 0l-6 6m3 12c-8.284 0-15-6.716-15-15V4.5A2.25 2.25 0 014.5 2.25h1.372c.516 0 .966.351 1.091.852l1.106 4.423c.11.44-.054.902-.417 1.173l-1.293.97a1.062 1.062 0 00-.38 1.21 12.035 12.035 0 007.143 7.143c.441.162.928-.004 1.21-.38l.97-1.293a1.125 1.125 0 011.173-.417l4.423 1.106c.5.125.852.575.852 1.091V19.5a2.25 2.25 0 01-2.25 2.25h-2.25z" />
                    </svg>
                    Request by call
                </button>
            </div>
        </div>
        

        <button class="mt-16 text-white bg-gradient-to-r from-blue-600 to-blue-800 rounded py-3 px-8 text-lg font-bold w-full flex flex-row gap-4 items-center justify-center">
            Continue
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
            </svg>
        </button>

        <p class="mt-20 on-surface-sec font-semibold text-[15px] text-center">Having trouble logging in? <a class="font-bold text-blue-500">Get Help</a></p>
    </div>
</template>