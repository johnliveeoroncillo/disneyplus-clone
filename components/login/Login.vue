<template>
    <div class="w-full relative bg">
        <img src="@/assets/img/stars_bg.webp" class="absolute w-full top-0 left-0 z-0" />
        <div class="p-10">
            <img src="@/assets/img/logo.webp" class="w-24" />
        </div>

        <div class="relative z-10 h-[200px] w-[max-content] mx-auto">
            <h1 class="font-semibold text-3xl on-surface inter-semibold block texxt-center">Log in or sign up to continue</h1>

            <transition name="slide">
                <LoginCard v-if="login" />
                 <LoginOtp v-else-if="otp" />
            </transition>
        </div>
        <div class="bg-gradient-to-t from-black h-[600px]"></div>
        <div class="w-full bg-black pt-4 inter-regular">
            <div class="max-w-6xl mx-auto">
                <div class="grid grid-cols-4">
                    <div class="flex-1">
                        <h1 class="font-semibold text-lg on-surface">Company</h1>

                        <ul class="flex flex-col mt-5 gap-2 text-sm">
                            <li>
                                <a class="tracking-wide on-surface-sec">Supported Devices</a>
                            </li>
                            <li>
                                <a class="tracking-wide on-surface-sec">Interest Based Ads</a>
                            </li>
                        </ul>   
                    </div>
                    <div class="flex-1">
                        <h1 class="font-semibold text-lg on-surface">View Website in</h1>

                        <ul class="flex flex-col mt-5 gap-2 text-sm">
                            <li>
                                <a class="font-semibold tracking-wide on-surface-sec flex flex-row gap-2">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 font-bold">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12.75l6 6 9-13.5" />
                                    </svg>
                                    English
                                </a>
                            </li>
                        </ul>   
                    </div>
                    <div class="flex-1">
                        <h1 class="font-semibold text-lg on-surface">Need Help?</h1>

                        <ul class="flex flex-col mt-5 gap-2 text-sm">
                            <li>
                                <a class="font-semibold tracking-wide on-surface-sec">Help</a>
                            </li>
                            <li>
                                <a class="font-semibold tracking-wide on-surface-sec">Feedback</a>
                            </li>
                        </ul>   
                    </div>
                    <div class="flex-1">
                        <h1 class="font-semibold text-lg on-surface">Connect with Us</h1>

                        <ul class="flex flex-row mt-5 gap-5 text-sm">
                            <li>
                                <a class="font-semibold tracking-wide on-surface-sec">
                                    <img src="@/assets/img/1.svg" class="w-8 font-bold" />
                                </a>
                            </li>
                            <li>
                                <a class="font-semibold tracking-wide on-surface-sec">
                                    <img src="@/assets/img/2.svg" class="w-8 font-bold" />
                                </a>
                            </li>
                            <li>
                                <a class="font-semibold tracking-wide on-surface-sec">
                                    <img src="@/assets/img/3.svg" class="w-8 font-bold" />
                                </a>
                            </li>
                        </ul>   
                    </div>
                </div>

                <div class="flex flex-row mt-5 text-sm pb-8 font-medium">
                    <div class="flex-1 flex flex-col gap-1 on-surface-sec">
                        <p class="tracking-wide">© 2022 Disney and its related entities. All Rights Reserved.</p>
                        <ul class="flex flex-row gap-4">
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
    </div>
</template>

<script>
export default {
    data() {
        return {
            login: false,
            otp: false,
        }
    },
    created() {
        this.$root.$on('login-otp', () => {
            this.login = false;
            setTimeout(() => {
                this.otp = true;
            }, 400);
        })
        this.$root.$on('login', () => {
            this.otp = false;
            setTimeout(() => {
                this.login = true;
            }, 400);
        })
    },
    beforeDestroy() {
        this.$root.$off('login-otp');
    },
    mounted() {
        setTimeout(() => {
            this.login = true;
        }, 500);
    }
}
</script>