<template>
    <div>
        <div :is="viewAtual"></div>

        <b-button v-b-toggle.sidebar-variant>Testes</b-button>
        <b-sidebar id="sidebar-variant" title="Menu" bg-variant="dark" text-variant="light" shadow>
            <div class="px-3 py-2">
                <b-button><i class="fa fa-exchange" aria-hidden="true"></i> Transferência de dados </b-button>
            </div>
        </b-sidebar>
    </div>
</template>

<script>
    import DataTransfer from '../DataTransfer/DataTransfer'
    export default {
        name: "Main",
        data() {
            return {
                viewAtual: null,

            }
        },
        comments:{
            DataTransfer
        }
    }
</script>

<style scoped>

</style>

<!--
    https://stackoverflow.com/questions/39391218/vuejs-swap-component-on-click
    https://stackoverflow.com/questions/44808395/click-on-a-button-and-changes-component-in-vuejs-2
-->
