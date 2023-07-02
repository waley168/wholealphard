<template>
    <div>
        <h1>{{keyphrase}}</h1>
        <p></p>
        <NuxtLink to="/about">Post 2</NuxtLink>
    </div>
</template>

<script setup lang="ts">
const keyphrase = '高雄'
const title = `${keyphrase}阿法租車 - 總發Alphard租車, 阿法包車`
const description = `專為${keyphrase}提供Toyota ALPHARD阿法租車服務，服務範圍包括高雄、屏東、台南及嘉義等地區。我們是全台唯一專營ALPHARD/阿法/埃爾法/阿發各式租車服務的業者，提供高品質與專業的服務，讓你的自駕體驗更上一層樓。阿法、埃爾法(ALPHARD)出租附駕駛、總發包車`

useSeoMeta({
    title,
    ogTitle: title,
    description,
    ogDescription: description,
    ogImage: 'https://wholealphard.com/wp-content/uploads/2023/06/wholealphard-banner01.png',
    twitterCard: 'summary_large_image',
})
</script>
