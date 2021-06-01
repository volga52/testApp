<template>
    <div>
        <input type="checkbox" v-model="value" />
        <h2 v-if="value">checkbox TRUE</h2>
        <h2 v-else>False checkbox</h2>
        <hr>
        <hr>
        <div v-for="item in goodList" :key="item.id">
            <b>Товар: </b> {{ item.name }}
        </div>
    </div>
</template>

<script>
export default {
    data: () => ({
        value: false,
        goodList: [
            {
                id: 1,
                name: 'Tovar1',
            },
            {
                id: 2,
                name: 'Tovar2',
            },
            {
                id: 3,
                name: 'Tovar3',
            },
        ]
    })
}
</script>