<script setup >
import { onMounted, ref } from 'vue'



const portfolioItems = ref([
  {
    image:
      'https://x10aibots.com/home/assets/mockups/phones-1.png',
    category: 'Branding',
    title: 'Branding Design',
    buttonText: 'View Details',
    buttonLink: 'https://x10aibots.com'
  },
  {
    image:
      'https://cdn.tailgrids.com/2.0/image/marketing/images/portfolio/portfolio-01/image-02.jpg',
    category: 'Marketing',
    title: 'Best Marketing tips',
    buttonText: 'View Details',
    buttonLink: '#'
  },
  {
    image:
      'https://cdn.tailgrids.com/2.0/image/marketing/images/portfolio/portfolio-01/image-03.jpg',
    category: 'Development',
    title: 'Web Design Trend',
    buttonText: 'View Details',
    buttonLink: '#'
  },
  {
    image:
      'https://cdn.tailgrids.com/2.0/image/marketing/images/portfolio/portfolio-01/image-04.jpg',
    category: 'Design',
    title: 'Business Card Design',
    buttonText: 'View Details',
    buttonLink: '#'
  },
  {
    image:
      'https://cdn.tailgrids.com/2.0/image/marketing/images/portfolio/portfolio-01/image-05.jpg',
    category: 'Marketing',
    title: 'Digital marketing',
    buttonText: 'View Details',
    buttonLink: '#'
  },
  {
    image:
      'https://cdn.tailgrids.com/2.0/image/marketing/images/portfolio/portfolio-01/image-06.jpg',
    category: 'Branding',
    title: 'Creative Agency',
    buttonText: 'View Details',
    buttonLink: '#'
  }
])

const selectedCategory = ref('All')

const uniqueCategories = ref([])
const filteredItems = ref([])

// Extract unique categories from portfolioItems
onMounted(() => {
  uniqueCategories.value = Array.from(new Set(portfolioItems.value.map((item) => item.category)))
  filterItems()
})

const selectCategory = (category) => {
  selectedCategory.value = category
  filterItems()
}

const filterItems = () => {
  if (selectedCategory.value === 'All') {
    filteredItems.value = portfolioItems.value
  } else {
    filteredItems.value = portfolioItems.value.filter(
      (item) => item.category === selectedCategory.value
    )
  }
}
</script>

<template>
    
  <!-- ====== Portfolio Section Start -->
  <section class="pt-6 pb-6 lg:pt-[80px] lg:pb-[90px] dark:bg-dark dark:text-white dark:bg-gray-700 ">
    <div class="container mx-auto ">
      <div class="-mx-4 flex flex-wrap">
        <div class="w-full px-4">
          <div class="mx-auto mb-[60px] max-w-[510px] text-center">
            <span class="text-primary mb-2 block text-lg font-semibold"> My Portfolio </span>
            <h2
              class="text-dark mb-3 text-3xl leading-[1.208] font-bold sm:text-4xl md:text-[40px]"
            >
              My Recent Projects
            </h2>
            <p class="text-body-color text-base dark:text-dark-6">
              Here are some of my recent projects. I have worked on a variety of projects, including branding, marketing, development, and design.
            </p>
          </div>
        </div>
      </div>

      <div class="w-full flex flex-wrap justify-center -mx-4">
        <div class="w-full px-4">
          <ul class="flex flex-wrap justify-center mb-12 space-x-1">
            <li class="mb-1">
              <button
                v-for="category in ['All', ...uniqueCategories]"
                :key="category"
                @click="selectCategory(category)"
                :class="{
                  'bg-primary text-blue-700': selectedCategory === category,
                  'text-body-color dark:text-dark-6 hover:bg-primary hover:text-blue-700':
                    selectedCategory !== category
                }"
                class="inline-block rounded-lg py-2 px-5 text-center text-base font-semibold transition md:py-3 lg:px-8"
              >
                {{ category }}
              </button>
            </li>
          </ul>
        </div>
      </div>

      <div class="flex flex-wrap -mx-4">
        <div class="w-full px-6 md:w-1/2 xl:w-1/3" v-for="item in filteredItems" :key="item.title">
          <div class="relative mb-12">
            <div class="overflow-hidden rounded-[10px]">
              <img :src="item.image" alt="portfolio" class="w-full" />
            </div>
            <div
              class="relative z-10 mx-7 -mt-20 rounded-lg dark:bg-gray-800 dark:border-gray-700 bg-white dark:bg-dark-2 py-[34px] shadow-md px-3 text-center shadow-portfolio dark:shadow-sm-light dark:shadow-box-dark"
            >
              <span class="text-primary mb-2 block text-sm font-medium">{{ item.category }}</span>
              <h3 class="text-dark dark:text-white mb-5 text-xl font-bold">{{ item.title }}</h3>
              <a
                :href="item.buttonLink"
                class="text-body-color dark:text-dark-6 hover:border-primary hover:bg-primary inline-block rounded-md border border-stroke dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 dark:border-dark-3 py-[10px] px-7 text-sm font-medium transition hover:text-blue-700"
              >
                {{ item.buttonText }}
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- ====== Portfolio Section End -->
</template>
