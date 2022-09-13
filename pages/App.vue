<template>
    <div>
    <carousel :slides="slides" :interval="5000" controls indicators/>
    </div>
</template>

<script>

export default {
    data: () => ({
        slides: [
            "https://picsum.photos/id/1032/900/400",
            "https://picsum.photos/id/1033/900/400",
            "https://picsum.photos/id/1037/900/400",
            "https://picsum.photos/id/1035/900/400",
            "https://picsum.photos/id/1036/900/400",
        ],
    }),
}
</script>
