<template>
    <div class="theme-container">
        <div class="theme-default-content">
            <h1>خطأ 404</h1>

            <blockquote>{{ getMsg() }}</blockquote>

            <RouterLink to="/">
                العودة للصفحة الرئيسية
            </RouterLink>
        </div>
    </div>
</template>

<script>
    const msgs = [
        `الصفحة المطلوبة غير موجودة`,
    ]

    export default {
        methods: {
            getMsg() {
                return msgs[Math.floor(Math.random() * msgs.length)]
            }
        }
    }
</script>

<style lang="stylus">
    @font-face
        font-family GanjNamehSans
        src url('../fonts/GanjNamehSans-Regular.woff2') format('woff2'), url('../fonts/GanjNamehSans-Regular.woff') format('woff'), url('../fonts/GanjNamehSans-Regular.ttf') format('truetype')
</style>
