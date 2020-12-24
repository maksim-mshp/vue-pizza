<template>
    <div>
        <h2> Pizza Name: {{pizzaName}}</h2>
        <p>Price: {{pizzaPrice}}</p>
        <slot name='n1'> </slot>
        <slot> </slot>
    </div>
</template>
<script>
    export default {
        props: ['pizzaName', 'pizzaPrice']
    }
</script>