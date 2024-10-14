<template lang="">
    <div >
        Bai 3
        <div :class="{card}">
            <div :class="{img}"></div>
            <div :class="{content}">
                <button>Add to card</button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="">
    .card{
        height: 300px;
        width: 500px;
        /* border: 5px; */
    }
</style>