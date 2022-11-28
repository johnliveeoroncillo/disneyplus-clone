<template>
    <div class="w-[fit-content] mx-auto">
        <div class="mt-16 flex flex-row gap-2 justify-center">
            <input class="border border-blue-200 border-opacity-50 bg-transparent text-lg font-medium text-blue-200 rounded-lg w-[70px] px-4 py-2 opacity-40 tracking-wider" placeholder="+63">
            
            <div class="relative w-[300px]">
                <input type="text" id="floating_outlined" class="block px-4 pb-2.5 py-2  w-full on-surface bg-transparent rounded-lg border border-blue-200 border-opacity-20 appearance-none focus:outline-none focus:ring-0 focus:border-gray-500 peer text-lg" placeholder=" " value="232" />

                <label for="floating_outlined" class="absolute text-gray-600 font-bold text-lg duration-300 transform -translate-y-5 scale-75 top-1 left-3 z-10 origin-[0] px-2 peer-focus:px-2 peer-focus:text-gray-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:-translate-y-1/2 peer-placeholder-shown:top-1/2 peer-focus:top-[1px] peer-focus:scale-75 peer-focus:-translate-y-4 whitespace-nowrap peer-focus:font-bold peer-placeholder-shown:font-medium">Enter mobile number</label>
            </div>
        </div>
        
        <p class="on-surface-100 text-xs mx-auto text-left note mt-2 font-light tracking-wide">We will use your information to personalize and improve your experience and send service updates. We may use your data as described in our  <a href="https://privacy.thewaltdisneycompany.com/en/current-privacy-policy/">Privacy Policy</a> and <a href="https://privacy.thewaltdisneycompany.com/en/current-privacy-policy/supplemental-privacy-policy-for-philippines/">Supplemental Privacy Policy for Philippines</a>. By clicking "Agree and Continue", you agree to our <a href="https://www.apps.disneyplus.com/subscriberagreement/ph/eng"> Subscriber Agreement </a>, <a href="https://privacy.thewaltdisneycompany.com/en/current-privacy-policy/">Privacy Policy</a> and  <a href="https://privacy.thewaltdisneycompany.com/en/current-privacy-policy/supplemental-privacy-policy-for-philippines/">Supplemental Privacy Policy for Philippines</a>.</p>
    

        <button class="mt-28 text-white bg-gradient-to-r from-blue-500 to-blue-900 rounded py-3 px-8 text-lg font-bold w-full flex flex-row gap-4 items-center justify-center">
            Agree and Continue
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
            </svg>
        </button>

        <p class="mt-20 on-surface-sec font-semibold text-[15px]">Having trouble logging in? <a class="font-bold text-blue-500">Get Help</a></p>
    </div>
</template>