<template>
    <div class="w-full relative bg bg-gradient-to-t from-black">
        <img src="@/assets/img/stars_bg.webp" class="absolute w-full top-0 left-0 z-0" />
        <div class="p-10">
            <img src="@/assets/img/logo.webp" class="w-24" />
        </div>

        <div class="text-center relative z-10" style="height: calc(100vh - 322px);">
            <h1 class="font-semibold text-4xl text-gray-200">Log in or sign up to continue</h1>

            <div class="mt-16">
                <input class="border border-blue-200 bg-transparent text-xl text-blue-200 rounded-lg w-[70px] px-4 py-3 opacity-40 font-light tracking-wider" placeholder="+63">
                <input class="border border-blue-200 bg-transparent text-xl text-blue-200 rounded-lg px-4 py-3 opacity-40" placeholder="Enter mobile number">
            </div>
        </div>

        <div class="w-full max-w-6xl mx-auto">
            <div class="grid grid-cols-4">
                <div class="flex-1">
                    <h1 class="text-gray-300 font-semibold text-lg">Company</h1>

                    <ul class="flex flex-col mt-5 gap-2 text-sm">
                        <li>
                            <a class="text-blue-200 opacity-60 font-medium tracking-wide">Supported Devices</a>
                        </li>
                        <li>
                            <a class="text-blue-200 opacity-60 font-medium tracking-wide">Interest Based Ads</a>
                        </li>
                    </ul>   
                </div>
                <div class="flex-1">
                    <h1 class="text-gray-300 font-semibold text-lg">View Website in</h1>

                    <ul class="flex flex-col mt-5 gap-2 text-sm">
                        <li>
                            <a class="text-blue-200 opacity-60 font-semibold tracking-wide">English</a>
                        </li>
                    </ul>   
                </div>
                <div class="flex-1">
                    <h1 class="text-gray-300 font-semibold text-lg">Need Help?</h1>

                    <ul class="flex flex-col mt-5 gap-2 text-sm">
                        <li>
                            <a class="text-blue-200 opacity-60 font-semibold tracking-wide">Help</a>
                        </li>
                        <li>
                            <a class="text-blue-200 opacity-60 font-semibold tracking-wide">Feedback</a>
                        </li>
                    </ul>   
                </div>
                <div class="flex-1">
                    <h1 class="text-gray-300 font-semibold text-lg">Connect with Us</h1>

                    <ul class="flex flex-row mt-5 gap-2 text-sm">
                        <li>
                            <a class="text-blue-200 opacity-60 font-semibold tracking-wide">Help</a>
                        </li>
                        <li>
                            <a class="text-blue-200 opacity-60 font-semibold tracking-wide">Feedback</a>
                        </li>
                    </ul>   
                </div>
            </div>

            <div class="flex flex-row mt-5 text-sm pb-8">
                <div class="flex-1 flex flex-col gap-1 text-blue-200 opacity-60">
                    <p class="tracking-wide">© 2022 Disney and its related entities. All Rights Reserved.</p>
                    <ul class="flex flex-row gap-4 font-medium">
                        <li class="tracking-wide">
                            Privacy Policy
                        </li>
                        <li class="tracking-wide">
                            Subscriber Agreement
                        </li>
                        <li class="tracking-wide">
                            Supplemental Privacy Policy For Philippines
                        </li>
                    </ul>
                </div>
                <div class="flex flex-row gap-2">
                    <div class="w-[150px]">
                        <img src="@/assets/img/google-playstore.webp"/>
                    </div>
                    <div class="w-[150px]">
                        <img src="@/assets/img/ios-appstore.webp"/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.bg {
    background-color: #081633;
}
</style>