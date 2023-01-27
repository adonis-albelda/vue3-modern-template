<template>
  <div class="grid grid-cols-12 gap-5">
    <div class="lg:col-span-8 col-span-12">
      <Card title="Version's" subtitle="	3 January 2023">
        <div>
          <Badge> new </Badge>
        </div>
        <div class="mt-6 space-y-5">
          <div>
            <Disclosure v-slot="{ open }">
              <DisclosureButton
                class="bg-slate-50 dark:bg-slate-700 dark:bg-opacity-60 rounded-t-md flex justify-between cursor-pointer transition duration-150 font-medium w-full text-start text-base text-slate-600 dark:text-slate-300 px-8 py-4"
              >
                <span
                  >Version 2.0.0
                  <span class="font-light text-xs">
                    - 23 January 2023</span
                  ></span
                >
                <span
                  class="transition-all duration-150 text-xl"
                  :class="open && 'rotate-180 transform '"
                  ><Icon icon="heroicons:chevron-down-solid"
                /></span>
              </DisclosureButton>
              <DisclosurePanel>
                <div
                  class="text-sm text-slate-600 font-normal bg-white dark:bg-slate-900 dark:text-slate-300 rounded-b-md dark:border dark:border-slate-700 dark:border-t-0 border border-slate-100 border-t-0"
                >
                  <div class="px-8 py-4">
                    <div>
                      <span
                        class="flex space-x-3 items-center mt-2 text-slate-600 dark:text-slate-300 text-sm"
                      >
                        <span
                          class="h-2 w-2 bg-primary-500 rounded-full"
                        ></span>
                        <span>Vite and pinia</span></span
                      >
                    </div>
                  </div>
                </div>
              </DisclosurePanel>
            </Disclosure>
          </div>
          <div>
            <Disclosure v-slot="{ open }">
              <DisclosureButton
                class="bg-slate-50 dark:bg-slate-700 dark:bg-opacity-60 rounded-t-md flex justify-between cursor-pointer transition duration-150 font-medium w-full text-start text-base text-slate-600 dark:text-slate-300 px-8 py-4"
              >
                <span
                  >Version 1.0.0
                  <span class="font-light text-xs">
                    - 3 January 2023</span
                  ></span
                >
                <span
                  class="transition-all duration-150 text-xl"
                  :class="open && 'rotate-180 transform '"
                  ><Icon icon="heroicons:chevron-down-solid"
                /></span>
              </DisclosureButton>
              <DisclosurePanel>
                <div
                  class="text-sm text-slate-600 font-normal bg-white dark:bg-slate-900 dark:text-slate-300 rounded-b-md dark:border dark:border-slate-700 dark:border-t-0 border border-slate-100 border-t-0"
                >
                  <div class="px-8 py-4">
                    <div>
                      <span
                        class="flex space-x-3 items-center mt-2 text-slate-600 dark:text-slate-300 text-sm"
                      >
                        <span
                          class="h-2 w-2 bg-primary-500 rounded-full"
                        ></span>
                        <span>Initial Release</span></span
                      >
                    </div>
                  </div>
                </div>
              </DisclosurePanel>
            </Disclosure>
          </div>
        </div>
      </Card>
    </div>
    <div class="lg:col-span-4 col-span-12">
      <Card title="CHANGELOG">
        <h5 class="text-xs font-medium">VERSION HISTORY</h5>
        <ul
          class="space-y-3 mt-6 divide-y dark:divide-slate-700 divide-slate-100"
        >
          <li
            class="flex justify-between items-center text-xs text-slate-600 dark:text-slate-300 pt-3"
          >
            <span>Version 2.0.0 </span>
            <span> 23 January 2023 </span>
          </li>
          <li
            class="flex justify-between items-center text-xs text-slate-600 dark:text-slate-300 first:pt-0 pt-3"
          >
            <span>Version 1.0.0 </span>
            <span> 3 January 2023 </span>
          </li>
        </ul>
      </Card>
    </div>
  </div>
</template>
<script setup>
import Card from "@/components/Card";
import Badge from "@/components/Badge";
import Icon from "@/components/Icon";
import { ref } from "vue";
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
const items = ref([
  {
    title: "Version 1.0.0 - 	3 January 2023",
    content: "",
  },
]);
</script>
<style lang=""></style>
