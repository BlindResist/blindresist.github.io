<template>
    <header class="app-header">
        <app-logo />
        <app-navigation />
    </header>
</template>

<script>
export default {
    name: 'app-header',
    data () {
        return {}
    }
}
</script>

<style lang="scss">
.app-header {
    display: flex;
    align-items: center;
    flex-flow: row nowrap;
    justify-content: space-between;
    width: 100%;
    padding: 1rem;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 100;
    pointer-events: none;

    @include breakpoint(v-mobile) {
        padding: 1rem;
        background-color: $white;
    }

    > * {
        pointer-events: auto;
    }
}
</style>
