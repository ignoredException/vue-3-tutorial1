<template>
    <div class="content">
        <div class="nav">
            <a class="active" href="home-site.vue">Home</a>
            <a href="calculator-site.vue">Calculator</a>
        </div>
        <body>
            &nbsp;
            <h1>Home</h1>
            <p>Welcome on the Homepage!</p>
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
}

.nav body {
    background-color: deepskyblue;
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

.nav {
    background-color: gray;
    overflow: hidden;
}

.nav a {
    float: left;
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    font-size: 20px;
}

.nav a:hover {
    background-color: gray;
    color: black;
}

.nav a.active {
    background-color: darkcyan;
    color: white;
}

</style>