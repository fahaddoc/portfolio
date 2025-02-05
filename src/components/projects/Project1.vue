<script setup lang="ts">

defineProps<{
    imageLeft: string,
    imageRight: string,
    description:string
}>();

</script>

<template>
    <div class="col">
        <div class="row">
            <div class="left-box">
                <img alt="" :src="imageLeft" />
            </div>
            <div class="right-box">
                <img alt="" :src="imageRight" />
            </div>
        </div>
        <div class="description">
            {{description}}
        </div>
    </div>
</template>

<style scoped>
.col{
    display: flex;
    flex-direction: column;
    width: 100%;
    background-color: yellow;
}
.col > .row{
    display: flex;
    justify-content: center;
    width: 100%;
    background-color: red;
}
.row > .left-box{
    display: flex;
    flex: 1;
    width: 100%;
    background-color: white;
}

.row > .right-box{
    display: flex;
    flex: 1;
    width: 100%;
    background-color: #ff926e;
}
</style>