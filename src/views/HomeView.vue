<template>

  <ul class="list-group list-group-flush">
    
    
    <li v-for="book in books"
    :key="book.name"
    :details="book"
    @click="setBook(book.name)"
    >
    <router-link to="/details">{{book.name}}</router-link>
    </li>
    
   
    
  </ul>
</template>

<script>
import axios from "axios";
import Books from "@/components/Books.vue";
import book from "@/book";

export default {
  name: "books",
  data() {
    return {
    books: []
    };
  },
  
 async created() {
      const response = await fetch("https://www.anapioficeandfire.com/api/books");
      const data = await response.json();
      this.books = data;
      },
      

  components: {
    Books,
    
  },
  methods: {
    setBook(booka) {
      book.currentBook = booka;
      console.log(booka);
     
    },
  },
};
</script>
