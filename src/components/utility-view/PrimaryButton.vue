<script>
export default {
    name: "PrimaryButton",
    props: {
        text: String
    }
}
</script>

<template>
    <div>
        {{ text }}
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/colors.scss' as *;

div {
    width: 185px;
    height: 35px;
    background-color: $primary-color;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;

    &:hover {
        background-color: white;
        color: $primary-color;
        cursor: pointer;
    }
}
</style>