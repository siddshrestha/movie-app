<template>
  <div id="movie-container">
      <ul>
          <li style="color: white" v-for="(movie, index) in movies" :key="movie.id">{{index}}:{{movie.name}}</li>
      </ul>
  </div>
</template>

<script>
export default {
    data() {
        return {
            movies: [
                {
                    id: 1,
                    name: 'Shawshank Redemption'
                },
                {
                    id: 2,
                    name: 'Seven'
                },
                {
                    id: 3,
                    name: 'Pagglait'
                }
            ]
        }
    },
}
</script>

<style lang='scss' scoped>
	#movie-container {
		padding-top: 1rem;
		display: flex;
		flex-wrap: wrap;
		flex-grow: 2;
		justify-content: center;
	}
</style>