<script setup>
import { ref } from 'vue'

const featuresItems = ref([
    {
        icon: `<svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M21.0375 1.2374C11.8125 -0.393851 2.92503 5.7374 1.29378 14.9624C0.450029 19.4061 1.46253 23.9624 4.05003 27.6749C6.63753 31.4436 10.5188 33.9186 14.9625 34.7624C15.975 34.9311 16.9875 35.0436 18 35.0436C26.0438 35.0436 33.2438 29.2499 34.7625 21.0374C36.3938 11.8124 30.2625 2.9249 21.0375 1.2374ZM32.2313 20.5874C32.175 21.0374 32.0625 21.4874 31.95 21.8811L19.2375 17.0999V3.5999C19.6875 3.65615 20.1375 3.7124 20.5313 3.76865C28.4063 5.1749 33.6375 12.7124 32.2313 20.5874ZM16.7063 3.5999V16.7624H3.60003C3.65628 16.3124 3.71253 15.8624 3.76878 15.4124C4.95003 8.83115 10.4063 4.10615 16.7063 3.5999ZM15.4125 32.2311C11.5875 31.5561 8.32503 29.4186 6.13128 26.2124C4.66878 24.1311 3.82503 21.7124 3.60003 19.2374H17.775L31.05 24.2436C28.2938 29.9811 21.9375 33.4686 15.4125 32.2311Z"
                  fill="white"
                />
              </svg>`,
        title: 'Refreshing Design',
        details:
            'We enjoy working with discerning clients and people for whom quality, service, integrity & aesthetics.  '
    },
    {
        icon: `
              <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M18 1.9126C9.5625 1.9126 2.0875 8.3876 2.0875 16.8251C2.0875 25.2626 9.5625 31.7376 18 31.7376C26.4375 31.7376 33.9125 25.2626 33.9125 16.8251C33.9125 8.3876 26.4375 1.9126 18 1.9126ZM18 29.7751C10.875 29.7751 5.0625 23.9626 5.0625 16.8251C5.0625 9.6876 10.875 3.8751 18 3.8751C25.125 3.8751 30.9375 9.6876 30.9375 16.8251C30.9375 23.9626 25.125 29.7751 18 29.7751Z"
                  fill="white"
                />
                <path
                  d="M18 7.10635C15.3375 7.10635 13.1625 9.28135 13.1625 11.9438C13.1625 14.6064 15.3375 16.7814 18 16.7814C20.6625 16.7814 22.8375 14.6064 22.8375 11.9438C22.8375 9.28135 20.6625 7.10635 18 7.10635ZM18 14.1064C16.575 14.1064 15.4875 13.0188 15.4875 11.5938C15.4875 10.1688 16.575 9.08135 18 9.08135C19.425 9.08135 20.5125 10.1688 20.5125 11.5938C20.5125 13.0188 19.425 14.1064 18 14.1064Z"
                  fill="white" />
        `,
        title: 'Easy to Customize',
        details:
            ' I develop customised software solutions for businesses, with a focus on user experience and performance.'
    },
    {
        icon: `
        
        <svg
                width="36"
                height="36"
                viewBox="0 0 36 36"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M30.2625 10.6312C27.1688 7.36875 22.8375 5.34375 18 5.34375C8.60626 5.34375 1.01251 12.9937 1.01251 22.3875C1.01251 25.0312 1.63126 27.6187 2.75626 29.925C2.92501 30.2625 3.20626 30.4875 3.54376 30.6C3.65626 30.6 3.71251 30.6562 3.82501 30.6562C3.82501 30.6562 3.82501 30.6562 3.88126 30.6562C3.88126 30.6562 3.88126 30.6562 3.93751 30.6562C3.99376 30.6562 4.05001 30.6562 4.10626 30.6562C4.21876 30.6562 4.38751 30.6 4.50001 30.5437L6.80626 29.4187C7.42501 29.1375 7.70626 28.35 7.36876 27.7312C7.03126 27.1125 6.30001 26.8312 5.68126 27.1687L4.55626 27.7312C3.88126 26.1 3.60001 24.3562 3.54376 22.5562H5.90626C6.58126 22.5562 7.20001 21.9937 7.20001 21.2625C7.20001 20.5312 6.63751 19.9687 5.90626 19.9687 H 3.71251C4.10626 17.4937 5.17501 15.2437 6.69376 13.3875L8.71876 15.4125C8.94376 15.6375 9.28126 15.8062 9.61876 15.8062C9.95626 15.8062 10.2938 15.6937 10.5188 15.4125C11.025 14.9062 11.025 14.1187 10.5188 13.6125L 8.43751 11.5312C 10.6875 9.5625 13.5563 8.2125 16.7625 7.9875 V 11.4187 C 16.7625 12.0937 17.325 12.7125 18.0563 12.7125 C 18.7313 12.7125 19.35 12.15 19.35 11.4187 V 7.9875 C 22.5 8.26875 25.425 9.5625 27.675 11.5312 L 26.1 13.1062 C 25.5938 13.6125 25.5938 14.4 26.1 14.9062 C 26.325 15.1312 26.6625 15.3 27 15.3 C 27.3375 15.3 27.675 15.1875 27.9 14.9062 L 29.4188 13.3875 C 30.9375 15.2437 31.95 17.4937 32.4 19.9687 H 30.2063 C 29.5313 19.9687 28.9125 20.5312 28.9125 21.2625 C 28.9125 21.9937 29.475 22.5562 30.2063 22.5562 H 32.5688 C 32.5688 24.3562 32.2313 26.1 31.5563 27.7875 L 30.4313 27.225 C 29.8125 26.8875 29.025 27.1687 28.7438 27.7875 C 28.4625 28.4062 28.6875 29.1937 29.3063 29.475 L 31.6125 30.6 C 31.7813 30.7125 32.0063 30.7125 32.175 30.7125 C 32.175 30.7125 32.175 30.7125 32.2313 30.7125 C 32.2313 30.7125 32.2313 30.7125 32.2875 30.7125 C 32.7375 30.7125 33.1875 30.4312 33.4125 30.0375 C 34.5938 27.7312 35.1563 25.0875 35.1563 22.5 C 35.0438 17.8312 33.1875 13.6687 30.2625 10.6312 Z" fill="white" />
              
                  
        `,
        title: 'Maintenance & Support',
        details:
            'I also provide ongoing maintenance and support for the software solutions I develop, ensuring they remain up-to-date and secure.'
    },
    
])
</script>

<template>
    <!-- ====== Services Section Start -->
    
    <section
        class="pt-20 pb-12  lg:pt-[120px] lg:pb-[90px] dark:bg-dark dark:text-white dark:bg-gray-700 dark:border-gray-700 ">
        <div class="container px-8 mx-auto">
            <div class="-mx-4 flex flex-wrap">
                <div class="w-full px-4">
                    <div class="mx-auto mb-12 max-w-[510px] text-center lg:mb-20">
                        <span class="text-primary mb-2 block text-lg font-semibold"> Services </span>
                        <h2
                            class="text-dark dark:bg-gray-700 dark:border-gray-700 dark:text-white mb-3 text-3xl leading-[1.2] font-bold sm:text-4xl md:text-[40px]">
                            What I Offer
                        </h2>
                        <p class="text-body-color text-base dark:text-dark-6">
                            I offer a range of services, from full-stack development to ongoing maintenance and support.
                        </p>
                    </div>
                </div>
            </div>
            <div class="-mx-4 flex flex-wrap">
                <template v-for="(item, index) in featuresItems" :key="index">
                    <div class="w-full px-4 md:w-1/2 lg:w-1/3">
                        <div
                            class="mb-9 rounded-[20px] dark:bg-gray-800 dark:border-gray-400  bg-white dark:bg-dark-2 p-10 shadow-md dark:shadow-sm-light hover:shadow-lg dark:hover:shadow-lg md:px-7 xl:px-10">
                            <div class="bg-primary bg-blue-500 mb-8 flex h-[70px] w-[70px] items-center justify-center rounded-2xl"
                                v-html="item.icon"></div>
                            <div class="relative isolate px-6 pt-4 lg:px-8">
                                <div class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80"
                                    aria-hidden="true">
                                    <div class="relative left-[calc(50%-11rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-gradient-to-tr from-[#ff80b5] to-[#21025a] opacity-30 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]"
                                        style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)" />
                                </div>

                                <div class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]"
                                    aria-hidden="true">
                                    <div class="relative left-[calc(50%+3rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-30 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]"
                                        style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)" />
                                </div>
                            </div>
                            <h4
                                class="text-dark dark:bg-gray-800 dark:border-gray-700 dark:text-white mb-[14px] text-2xl font-semibold">
                                {{ item.title }}
                            </h4>
                            <p class="text-body-color dark:text-dark-6">
                                {{ item.details }}
                            </p>
                        </div>
                    </div>
                </template>
            </div>
        </div>
    </section>
    <!-- ====== Services Section End -->
</template>
