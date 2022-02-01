<template>
    <div class="content">
        <body>
            &nbsp;
            <h1>Your Calculator</h1>
            <p>Here you can see your calculators..<br>
            You can <b>add</b>, <b>subtract</b>, <b>multiply</b> and <b>divide</b>.
            </p>
            &nbsp;
            <h3>Add:</h3>
            <form v-on:submit.prevent="add">
                <input type="number" v-model="add_num1">
                <input type="number" v-model="add_num2">
                <button type="submit">Solve</button>
            </form>
            <p>Result: {{ add_sum }}</p>
            &nbsp;
            <h3>Subtract:</h3>
            <form v-on:submit.prevent="subtract">
                <input type="number" v-model="sub_num1">
                <input type="number" v-model="sub_num2">
                <button type="submit">Solve</button>
            </form>
            <p>Result: {{ sub_sum }}</p>
            &nbsp;
            <h3>Multiply:</h3>
            <form v-on:submit.prevent="multiply">
                <input type="number" v-model="mul_num1">
                <input type="number" v-model="mul_num2">
                <button type="submit">Solve</button>
            </form>
            <p>Result: {{ mul_sum }}</p>
            &nbsp;
            <h3>Divide:</h3>
            <form v-on:submit.prevent="divide">
                <input type="number" v-model="div_num1">
                <input type="number" v-model="div_num2">
                <button type="submit">Solve</button>
            </form>
            <p>Result: {{ div_sum }}</p>
            &nbsp;
        </body>
    </div>
</template>

<script>

    export default {

        data() {

            return {

                add_num1: 0,
                add_num2: 0,
                add_sum: 0,
                sub_num1: 0,
                sub_num2: 0,
                sub_sum: 0,
                mul_num1: 0,
                mul_num2: 0,
                mul_sum: 0,
                div_num1: 0,
                div_num2: 0,
                div_sum: 0,

            };

        },

        methods: {

            add: function() {

                this.add_sum = parseInt(this.add_num1, 10) + parseInt(this.add_num2, 10);

            },

            subtract: function() {

                this.sub_sum = parseInt(this.sub_num1, 10) - parseInt(this.sub_num2, 10);

            },

            multiply: function() {

                this.mul_sum = parseInt(this.mul_num1, 10) * parseInt(this.mul_num2, 10);


            },

            divide: function() {

                this.div_sum = parseInt(this.div_num1, 10) / parseInt(this.div_num2, 10);

            }

        }

    }

</script>

<style>

.content body {
    background-color: deepskyblue;
    width: 99%;
    padding: 10px;
    box-sizing: border-box;
    border-radius: 3px 15px 5px 30px;
}

input {
    background-color: lightgray;
    border-color: darkgray;
}

button {
    background-color: lightgray;
    border-color: darkgray;
}

p {
    font-family: Arial;
    font-size: 20px;
}

</style>