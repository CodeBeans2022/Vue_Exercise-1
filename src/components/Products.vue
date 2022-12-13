<template>
    <div class="products mb-4">
        <div class="card" v-for="(book, index) in comicBooks" :key="index">
            <img :src="book.image" class="card-img-top">

            <div class="card-body">
                <h5>{{ book.id }}</h5>
                <h6>{{ book.bookTitle }}</h6>
                <p>R{{ book.price }}</p>

            </div>

        </div>
    </div>
</template>

<script>

export default {
    data() {
        return {

            comicBooks: [
                {
                    id: `#1`,
                    price: 80,
                    bookTitle: "X-Men",
                    image: "https://i.postimg.cc/QdC8W5Gm/X-Men.jpg",
                    category: "Marvel Comics"
                },

                {
                    id: `#2`,
                    price: 120,
                    bookTitle: "Avengers",
                    image: "https://i.postimg.cc/gkDjhmwz/Avengers.jpg",
                    category: "Marvel Comics"
                },

                {
                    id: `#3`,
                    price: 80,
                    bookTitle: "Spider-Man",
                    image: "https://i.postimg.cc/xdk1Bm68/Spiderman.jpg",
                    category: "Marvel Comics"
                },

                {
                    id: `#4`,
                    price: 110,
                    bookTitle: "Fantastic Four",
                    image: "https://i.postimg.cc/mZ7tbQBF/Fantastic-Four.jpg",
                    category: "Marvel Comics"
                }

            ]

        }
    }
}

</script>

<style scoped>
.card img {
    object-fit: cover;
}

.card {
    width: 18rem;
}

.products {
    display: flex;
    justify-content: space-around;
}
</style>
