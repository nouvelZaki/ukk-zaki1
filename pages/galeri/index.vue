<template>
    <div class="container-fluid">
        <div class="row px-5 py-3">
            <div v-for="(cover, i) in berita" :key="i" class="col-2 py-2">
                <img :src="cover.cover" style="height:5rem;" alt="">
            </div>
            <div v-for="(cover, i) in berita" :key="i" class="col-2 py-2">
                <img :src="cover.cover" style="height:5rem;" alt="">
            </div>
            <div v-for="(cover, i) in berita" :key="i" class="col-2 py-2">
                <img :src="cover.cover" style="height:5rem;" alt="">
            </div>
        </div>
    </div>
</template>
<script setup>
const supabase = useSupabaseClient()
const berita = ref([])
useHead({ title: "Galery" })

const getBerita = async () => {
    const { data, error } = await supabase
        .from('berita')
        .select('cover')
    if (error) {
        console.error('Error Berita:', error)
    } else {
        berita.value = data
    }
}

onMounted(() => {
    getBerita()
})
</script>
<style scoped>
img {
    width: 100%;
}
</style>

