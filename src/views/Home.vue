<template>
  <div class="home">
    <div class="feature-card">
      <router-link to="/movie/79f8e412">
        <img
          class="featured-img"
          src="data:image/jpeg;base64,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"
          alt="Naruto Poster"
        />
        <div class="detail">
          <h3>Naruto</h3>
          <p>
            Set before the finale of Naruto, the film focuses on Naruto
            Uzumaki's ninja team as they go on a mission to stop the moon from
            falling, and rescue Hanabi Hyuga — Hinata Hyuga's sister — from
            Toneri Otsutsuki, a man who wishes to marry Hinata and punish
            mankind for weaponising chakra.
          </p>
        </div>
      </router-link>
    </div>

    <form @submit.prevent="SearchMovies()" class="search-box">
      <input
        type="text"
        placeholder="What are you looking for ?"
        v-model="search"
      />
      <input type="submit" value="Search" />

      <div class="movies-list">
        <div class="movie" v-for="movie in movies" :key="movie.imdbID">
          <!-- {{ movie.Title }} -->
          <router-link :to="'/movie/' + movie.imdbID" class="movie-link">
            <div class="product-image">
              <img :src="movie.Poster" alt="Movie Poster" />
              <div class="type">{{ movie.Type }}</div>
            </div>
            <div class="detail">
              <p class="year">
                {{ movie.Year }}
              </p>
              <h3>{{ movie.Title }}</h3>
            </div>
          </router-link>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

import { ref } from "vue";
import env from "@/env.js";

export default {
  setup() {
    const search = ref("");
    const movies = ref([]);

    const SearchMovies = () => {
      if (search.value != "") {
        // console.log(search.value); 3221
        console.log(`${env.apikey}`);
        fetch(`https://www.omdbapi.com/?apikey=${env.apikey}&s=${search.value}`)
          // http://www.omdbapi.com/?i=tt3896198&apikey=79f8e412
          .then((res) => res.json())
          .then((data) => {
            movies.value = data.Search;
            search.value = "";
            // console.log(movies.value);
          });
      }
    };

    return {
      search,
      movies,
      SearchMovies,
    };
  },
};
</script>

<style lang="scss">
.home {
  .feature-card {
    position: relative;

    .featured-img {
      display: block;
      width: 100%;
      height: 500px;
      object-fit: cover;

      position: relative;
      z-index: 0;
    }

    .detail {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: rgba(0, 0, 0, 0.6);
      padding: 16px;
      z-index: 1;

      h3 {
        color: #fff;
        margin-bottom: 16px;
      }

      p {
        color: #fff;
      }
    }
  }

  .search-box {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 16px;

    input {
      display: block;
      appearance: none;
      border: none;
      outline: none;
      background: none;

      &[type="text"] {
        width: 100%;
        color: #fff;
        background-color: #496583;
        font-size: 20px;
        padding: 10px 16px;
        border-radius: 8px;
        margin-bottom: 15px;
        transition: 0.4s;

        &::placeholder {
          color: #f3f3f3;
        }
        &:focus {
          box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.2);
        }
      }

      &[type="submit"] {
        width: 100%;
        max-width: 300px;
        background-color: #42bbb3;
        padding: 16px;
        border-radius: 8px;
        color: #fff;
        font-size: 20px;
        text-transform: uppercase;
        transition: 0.4s;

        &:active {
          background-color: #3b8070;
        }
      }
    }
  }
  .movies-list {
    display: flex;
    flex-wrap: wrap;
    margin: 0px 8px;

    .movie {
      max-width: 50%;
      flex: 1 1 50%;
      padding: 16px 8px;

      .movie-link {
        display: flex;
        flex-direction: column;
        height: 100%;

        .product-image {
          position: relative;
          display: block;

          img {
            display: block;
            width: 100%;
            height: 275px;
            object-fit: cover;
          }

          .type {
            position: absolute;
            padding: 8px 16px;
            background-color: #42b883;
            color: #fff;
            bottom: 16px;
            left: 0px;
            text-transform: capitalize;
          }
        }

        .detail {
          background-color: #496583;
          padding: 16px 8px;
          flex: 1 1 100%;
          border-radius: 0px 0px 8px 8px;

          .year {
            color: #AAA;
            font-size: 14px;
          }

          h3 {
            color: #FFF;
            font-weight: 600;
            font-size: 18px;
          }

        }
      }
    }
  }
}
</style>
