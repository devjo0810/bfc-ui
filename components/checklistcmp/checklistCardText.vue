<template>
    <div>
        <div v-for="(companyData, index) in textData " :key="index">
            <h3 class="text-lg text-gray-700">
                Checklist name
            </h3>
            <p class="mt-1 text-sm text-gray-500">
                checklist item count : {{ companyData.volume }}
            </p>
            <p class="mt-1 text-sm text-gray-500">
                checklist item open : {{ companyData.openDate }}
            </p>
            <p class="mt-1 text-sm text-gray-500">
                checklist item close : {{ companyData.closeDate }}
            </p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            textData: []
        }
    },

    async asyncData() {
        try {
            const response = await $get('')
            const textData = response.data

            return {
                textData
            };
        } catch {
            console.error('Error get <p> Data', error)
        }

    },
}
</script>