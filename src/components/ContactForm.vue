<template>
    <div class="contactForm">
        <form class="formDisplay" action="https://formspree.io/f/xdojdjnj" method="POST" target="_blank">
            <input type="text" name="name" placeholder="First Name">
            <input type="text" name="name" placeholder="Surname">
            <input type="email" name="name" placeholder="Email" required>
            <button>Submit</button>
        </form>
    </div>
</template>

<script></script>

<style scoped>
.formDisplay {
    display: flex;
    flex-direction: column;
    width: 500px;
    gap: 20px;
    border: 1px solid black;
    border-radius: 20px;
    padding: 35px;
    background-color: palegreen;
}

.contactForm {
    display: flex;
    justify-content: center;
}

input,
button {
    border-radius: 10px;
    padding: 10px;
    text-align: center;
}

button:hover {
    background-color: paleturquoise;
    transition: 2s;
}
</style>
