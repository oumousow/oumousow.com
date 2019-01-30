<template>
    <div>
        <h1>Test : {{ this.params}}</h1>
    </div>
</template>

<script>
export default {
    fetch() {
        console.log("params = ", this.params)
    }
}
</script>

