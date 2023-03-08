<template>
  <div class="mt-5">
    <h1 class="error-title">DISCULPE 👻</h1>
    <p class="error-body">No conseguimos encontrar esta página</p>

    <div class="mt-5">
      <img :src="getImageUrl" alt="Foto" height="400" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'home-component',
  props: {
    msg: String,
  },
  computed: {
    getImageUrl() {
      const listImg = [
        'https://dacomsa.com/dacomsastorefront/medias/IP-M2-001-850x850.jpg?context=bWFzdGVyfEZyZW5vc3wxODQwMjV8aW1hZ2UvanBlZ3xoOWQvaDU5Lzg4MTMxMTMzMTEyNjIvSVBfTTJfMDAxXzg1MHg4NTAuanBnfDEwYjI5MDE0ZTBjYzQ0NWM1OWViYzYyOWY5NGEwOGNjYzk4OTM5ZjE1MjYwNDczOTYxNTNiZTkwN2Y5M2VkMWU',
        'https://dacomsa.com/dacomsastorefront/medias/IP-SHD2-001-850x850.jpg?context=bWFzdGVyfEZyZW5vc3wxNzQzNjF8aW1hZ2UvanBlZ3xoYmIvaDBkLzg4MTMzMzI4ODk2MzAvSVBfU0hEMl8wMDFfODUweDg1MC5qcGd8ODk3MWFjM2FhMjQzNDRlYTBiYTZiZjIzN2I0YmJhMzU1NmY4NGQzNDM0NTdhNWM1ZTVmODcwMmQ1NzNiNTkzYw',
        'https://dacomsa.com/dacomsastorefront/medias/IP-SHD1-001-850x850.jpg?context=bWFzdGVyfEZyZW5vc3wxNzM5MTN8aW1hZ2UvanBlZ3xoNjkvaDBlLzg4MTMzMzI4MjQwOTQvSVBfU0hEMV8wMDFfODUweDg1MC5qcGd8ZDIyOGRhMDQ5ZjZhOTlkZDE4OTNmNmIzODkxYWI2MDZmYjhkNTFmMjliMmFmNTliMjY2YTQyNzMxZDA3NzMxYQ',
        'https://dacomsa.com/dacomsastorefront/medias/IP-BFD2-001-850x850.jpg?context=bWFzdGVyfEZyZW5vc3wxMDkyMTJ8aW1hZ2UvanBlZ3xoYjUvaDI3Lzg4MTg1MDQ1MzE5OTgvSVBfQkZEMl8wMDFfODUweDg1MC5qcGd8NmUxN2MyODdkOGFhODQ1MTViMTEzMWE2MGM5MDMwNTQ0OTFjYjY4MjIyN2U4YjA0ODdmZjc2MTQzNjFmYWQzZQ',
        'https://dacomsa.com/dacomsastorefront/medias/IP-BFD1-001-850x850.jpg?context=bWFzdGVyfEZyZW5vc3wxMDk1NjZ8aW1hZ2UvanBlZ3xoZmIvaDI0Lzg4MTg1MDQ0OTkyMzAvSVBfQkZEMV8wMDFfODUweDg1MC5qcGd8NzgwYzAxMjljMzFmYzhiNDFhMjU4YTQzZWE2MTY4MGRjMDUyYTBmMzUyMDc0NDk0YjQ4YzgyYzkyZWYyYTAzNg',
        'https://dacomsa.com/dacomsastorefront/medias/IP-SPC1-001-850x850.jpg?context=bWFzdGVyfEZyZW5vc3wxNzIzODh8aW1hZ2UvanBlZ3xoOWMvaGVhLzg4MTMwNzU1NjI1MjYvSVBfU1BDMV8wMDFfODUweDg1MC5qcGd8NzUwYTMwOWU0ZjNhMDg1NDcwOTFhNGIzMmM1OGUzOTdhNDlkNThkYzdjMjkyZDUwZmU0OTE4ZWUwNDZjYzBlZQ',
        //discos
        'https://www.fremax.com.br/storage/97ec0d75-80be-4ea1-ae35-d9e05ea1bda9.jpg',
        'https://www.fremax.com.br/storage/9ac62474-ee62-41f9-b091-8081193cac69.jpg',
      ];
      const numeroAleatorio = Math.floor(Math.random() * listImg.length);
      return listImg[numeroAleatorio];
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.error-title {
  font-weight: 300;
}
.error-body {
  font-family: 'IBM Plex Mono', monospace;
}
</style>
