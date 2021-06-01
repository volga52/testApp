<template>
    <div>
        {{ status }}
        <input v-model="firstname" />
        <br>
        {{ fullUserName }}
        <input v-model="lastname" />
        <button @click.once="sendDataToServer">Send</button>
        <hr>
    </div>
</template>

<script>
export default {
    data: () => ({
        status: 'not sender',
        firstname: "",
        lastname: "",
    }),
    methods: {
        sendDataToServer() {
            const sendUp = {
                firstname: this.firstname,
                lastname: this.lastname,
            };

            console.log(sendUp);
            this.status = 'sended';
        },
    },
    computed: {
        fullUserName() {
            return `${this.firstname.toUpperCase()} ${this.lastname.toUpperCase()}`;
        },
    },
};
</script>