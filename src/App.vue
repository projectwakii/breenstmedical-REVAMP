<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from '@/components/HelloWorld.vue'
import HeaderView from '@/views/HeaderView.vue'
import FooterView from '@/views/FooterView.vue'
import ServicesView from '@/views/ServicesView.vue'
import JobsView from '@/views/JobsView.vue'
</script>

<!-- This example requires Tailwind CSS v2.0+ -->
<template>

<!-- Header Banner --> 
<HeaderView /> <!-- lol if adding more views in the future, I must remember to import them -->

<!-- NAVBAR -->
  <div class="relative bg-gray-50">
    <Popover class="relative bg-white shadow">
      <div class="max-w-7xl mx-auto px-4 sm:px-6">
        <div class="flex justify-between items-center py-6 md:justify-start md:space-x-10">
          <div class="flex justify-start lg:w-0 lg:flex-1">
            <a href="#">
              <span class="sr-only">Workflow</span>
              <img class="h-8 w-auto sm:h-10" src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg" alt="" />
            </a>
          </div>
          <div class="-mr-2 -my-2 md:hidden">
            <PopoverButton class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
              <span class="sr-only">Open menu</span>
              <MenuIcon class="h-6 w-6" aria-hidden="true" />
            </PopoverButton>
          </div>

          <!-- NAVBAR LINKS WITH ROUTINGGGGGGG --> 
          <!-- I MADE THESE! --> 
          <PopoverGroup as="nav" class="hidden md:flex space-x-10">
            <RouterLink to="/" class="text-base font-medium text-gray-500 hover:text-gray-900"> Home </RouterLink>
            <RouterLink to="/about" class="text-base font-medium text-gray-500 hover:text-gray-900"> Our Team </RouterLink>
            <RouterLink to="/services" class="text-base font-medium text-gray-500 hover:text-gray-900"> Services </RouterLink>
            <RouterLink to="/Jobs" class="text-base font-medium text-gray-500 hover:text-gray-900"> Jobs </RouterLink>


          </PopoverGroup>
          <!-- END NAVBAR LINKS -->


        </div>
      </div>
<!-- END NAVBAR --> 

  

<!-- I'M NOT SURE --> 
      <transition enter-active-class="duration-200 ease-out" enter-from-class="opacity-0 scale-95" enter-to-class="opacity-100 scale-100" leave-active-class="duration-100 ease-in" leave-from-class="opacity-100 scale-100" leave-to-class="opacity-0 scale-95">
        <PopoverPanel focus class="absolute top-0 inset-x-0 z-10 p-2 transition transform origin-top-right md:hidden">
          <div class="rounded-lg shadow-lg ring-1 ring-black ring-opacity-5 bg-white divide-y-2 divide-gray-50">
            <div class="pt-5 pb-6 px-5">
              <div class="flex items-center justify-between">
                <div>
                  <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg" alt="Workflow" />
                </div>
                <div class="-mr-2">
                  <PopoverButton class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
                    <span class="sr-only">Close menu</span>
                    <XIcon class="h-6 w-6" aria-hidden="true" />
                  </PopoverButton>
                </div>
              </div>
              <div class="mt-6">
                <nav class="grid gap-y-8">
                  <a v-for="item in features" :key="item.name" :href="item.href" class="-m-3 p-3 flex items-center rounded-md hover:bg-gray-50">
                    <component :is="item.icon" class="flex-shrink-0 h-6 w-6 text-indigo-600" aria-hidden="true" />
                    <span class="ml-3 text-base font-medium text-gray-900">
                      {{ item.name }}
                    </span>
                  </a>
                </nav>
              </div>
            </div>
          </div>
        </PopoverPanel>
      </transition>
    </Popover>

<!-- WHATEVER PAGE THE WEBSITE IS ON LOADS THE VIEW!!! THE MOST IMPORTANT PART --> 
<RouterView />

<!-- FOOTER--> 
<FooterView />

</div>
</template>
<!-- END OF PAGE --> 


<script>
import { Popover, PopoverButton, PopoverGroup, PopoverPanel } from '@headlessui/vue'
import {
  BookmarkAltIcon,
  CalendarIcon,
  ChartBarIcon,
  CursorClickIcon,
  MenuIcon,
  PhoneIcon,
  PlayIcon,
  RefreshIcon,
  ShieldCheckIcon,
  SupportIcon,
  ViewGridIcon,
  XIcon,
  HomeIcon, 
  SparklesIcon,
  UserIcon,
  BriefcaseIcon,
} from '@heroicons/vue/outline'
import { ChevronDownIcon } from '@heroicons/vue/solid'

const features = [
  {
    name: 'Home',
    href: '/',
    description: 'Home',
    icon: HomeIcon,
  },
  {
    name: 'Our Team',
    href: '/about',
    description: 'Our team.',
    icon: UserIcon,
  },
  {
    name: 'Services',
    href: '/services',
    description: 'Services.',
    icon: SparklesIcon,
  },
  {
    name: 'Jobs',
    href: '/jobs',
    description: 'Jobs.',
    icon: BriefcaseIcon,
  },
]


export default {
  components: {
    Popover,
    PopoverButton,
    PopoverGroup,
    PopoverPanel,
    ChevronDownIcon,
    MenuIcon,
    XIcon,
  },
  setup() {
    return {
      features,
      callsToAction,
      resources,
      recentPosts,
    }
  },
}
</script>


