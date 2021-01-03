<template>
  
  <div>
      <h1>Marvel Cinematic Universe</h1>
    <b-container class="bv-example-row">
        <div class="row">
            <div class="col-3" v-for="(movie, index) in movies" :key="index">
                <Card :movieData="movie"  /> 
            </div>
        </div>
    </b-container>
    <div></div>
  </div>
</template>
<script>
import Card from './Card'
export default {
    components:{
        Card
    },
    data(){
        return{
            movies: [
                {
                    id:1,
                    name:'Avengers:Endgame',
                    desc: 'Avengers: Endgame is a 2019 American superhero film based on the Marvel Comics superhero Avengers.',
                    release: '26 April 2019',
                    img:'https://m.media-amazon.com/images/M/MV5BMTc5MDE2ODcwNV5BMl5BanBnXkFtZTgwMzI2NzQ2NzM@._V1_.jpg',
                    rating:'8.4'
                },{
                    id:1,
                    name:'Captain Marvel',
                    desc: 'Captain Marvel is a 2019 American superhero film based on the Marvel Comics character Carol Danvers.',
                    release: '08 March 2019',
                    img:'https://preview.redd.it/69lht2ghnke21.jpg?auto=webp&s=e6204664fb702b09dd4c522f6038796d9f52f1bd',
                    rating:'6.9'
                },{
                    id:1,
                    name:'Doctor Strange',
                    desc: 'Doctor Strange is a 2016 American superhero film based on the Marvel Comics character of the same name.',
                    release: '4 Nov 2016',
                    img:'https://images-na.ssl-images-amazon.com/images/I/A12-NFRep6L._AC_SL1500_.jpg',
                    rating:'7.5'
                },{
                    id:1,
                    name:'Iron Man 3',
                    desc: 'Iron Man 3 is a 2013 American superhero film based on the Marvel Comics character Iron Man.',
                    release: '26 April 2013',
                    img:'https://i.pinimg.com/originals/cf/81/52/cf8152447ca6b83acbd3567cb2e05661.jpg',
                    rating:'7.1'
                },
            ]
        }
    },
    
};
</script>
<style scoped>

</style>