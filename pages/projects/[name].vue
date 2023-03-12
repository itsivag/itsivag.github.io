<template>
    <div class="flex flex-col">
        <NuxtLink to="/projects">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                class="w-12 h-8 rotate-180 mt-8 mx-4 border border-white p-1 rounded-sm hover:bg-yellow-500">
                <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
            </svg>
        </NuxtLink>
        <div class="my-auto">
            <h1 class="text-5xl p-4 text-yellow-500 capitalize">
                {{ project_name + " :" }}
            </h1>

            <div v-if="about.length != 0" class="flex">
                <p class="flex-1 text-2xl p-4">
                    {{ about }}
                </p>
                <div v-if="project_name == 'Wallbyte'"
                    class="flex-1 border-l border-yellow-500 pl-5 flex items-center justify-center">
                    <img src="/wallbyte.png" class="w-28 rounded-lg">
                    <a class="mx-6"
                        href="https://play.google.com/store/apps/details?id=com.superbeta.wallbyte&hl=en_IN&gl=US&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1"
                        target="_blank">
                        <img class="w-48 ml-auto inline-block" alt="Get it on Google Play"
                            src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png">
                    </a>
                </div>

                <div v-if="project_name == 'dlapp'"
                    class="flex-1 border-l border-yellow-500 pl-5 flex items-center justify-center">
                    <img src="/dlapp.png" class="w-28 rounded-lg p-4 bg-white">
                </div>
            </div>
            <div v-else>
                404
            </div>
        </div>
    </div>
</template>

<script setup>
const project_name = useRoute().params.name
const { data } = await useAsyncData('projects', () => queryContent('/projects').findOne())
const about = ref("")
for (const project of data.value.body) {
    if (project.name == project_name) {
        about.value = project.about
    }
}
</script>

<style>
.my-line {
    border-left: 1px solid #eab308;
}
</style>