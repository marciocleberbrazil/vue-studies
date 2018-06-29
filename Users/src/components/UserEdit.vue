<template>
    <div class="component">
        <h3>You may edit the User here</h3>
        <p>Edit me!</p>
        <p>User age: {{userAge}}</p>
        <button @click="editAge()">Update age</button>
    </div>
</template>

<script>
    import { eventBus } from '../main';

    export default {
        props: {
            userAge: Number
        },
        methods: {
            editAge() {
                this.userAge = 38;
                eventBus.changeAge(this.userAge);
            }
        }
    }
</script>

<style scoped>
    div {
        background-color: lightgreen;
    }
</style>
