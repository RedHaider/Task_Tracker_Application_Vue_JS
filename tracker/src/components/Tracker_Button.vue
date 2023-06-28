<template>
    <button @click="onClick()" :style="{background:color}" class="btn">{{ text }}</button>
</template>

<script>
export default{
    name: 'Tracker_Button',
    props: {
        text: String,
        color: String,
    },
    methods: {
        onClick(){
        console.log('Here i am '+this.color);
    },
}
}
</script>
