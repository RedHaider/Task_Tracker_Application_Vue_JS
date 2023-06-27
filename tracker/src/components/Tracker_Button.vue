<template>
    <button :style="{background:color}" class="btn">{{ text }}</button>
</template>

<script>
export default{
    name: 'Tracker_Button',
    props: {
        text: String,
        color: String,
    }
}
</script>
