<template>
  <div>
    <h1 class="pt-3 fs-3">Details</h1>
    <div
      class="card position-absolute top-50 start-50 translate-middle text-start"
    >
      <div class="card-body">
        <h5 class="card-title fw-bold">book name</h5>
        <p class="card-text">
          {{ book.book.name }}
        </p>
        <h5 class="card-title fw-bold">+book email</h5>
        <p class="card-text">
          {{ book.book.isbn }}
        </p>
        <h5 class="card-title fw-bold">book authors</h5>
        <p class="card-text">
          {{ books.books.authors }}
        </p>
        <h5 class="card-title fw-bold">country</h5>
        <p class="card-text">
          {{ books.country }}
        </p>
        <div class="text-center">
          <router-link to="/"
            ><button class="btn btn-primary">Back</button></router-link
          >
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import book from "@/book";

export default {
  
}
</script>