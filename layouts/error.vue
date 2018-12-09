<template>
    <div>
        <h2 v-if='error.statusCode==404'>
            this is a 404 page, the page which you found is not exist.
        </h2>
        <h2 v-else>
            error code : 500
        </h2>
    </div>
</template>

<script>
    export default {
        props:['error']
    }
</script>