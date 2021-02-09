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
                    release: '26 April 2019',
                    img:'https://m.media-amazon.com/images/M/MV5BMTc5MDE2ODcwNV5BMl5BanBnXkFtZTgwMzI2NzQ2NzM@._V1_.jpg',
                    rating:'8.4'
                },{
                    id:1,
                    name:'Captain Marvel' ,                   
                    release: '08 March 2019',
                    img:'https://preview.redd.it/69lht2ghnke21.jpg?auto=webp&s=e6204664fb702b09dd4c522f6038796d9f52f1bd',
                    rating:'6.9'
                },{
                    id:1,
                    name:'Infinity War',                    
                    release: '23 April 2018',
                    img:'https://i.pinimg.com/736x/24/a3/33/24a333e4ca1e0b80002d2ff0b576597e.jpg',
                    rating:'8.4'
                },
                {
                    id:1,
                    name:'Black Panther',                    
                    release: '29 January 2018',
                    img:'https://m.media-amazon.com/images/M/MV5BMTg1MTY2MjYzNV5BMl5BanBnXkFtZTgwMTc4NTMwNDI@._V1_.jpg',
                    rating:'7.3'
                },
                {
                    id:1,
                    name:'Thor Ragnarok',                   
                    release: '3 Nov 2017',
                    img:'https://mypostercollection.com/wp-content/uploads/2018/06/Thor-Ragnarok-HD-printable-posters-4.jpg?x35407',
                    rating:'7.9'
                },{
                    id:1,
                    name:'Spider-Man: Homecoming',                   
                    release: '7 July 2017',
                    img:'https://m.media-amazon.com/images/M/MV5BOGQ5YTM3YzctOTVmMC00OGIyLWFkZTYtMWYwOWZhMjA2MWMwXkEyXkFqcGdeQXVyMjUyMTE5MA@@._V1_.jpg',
                    rating:'7.5'
                },
                {
                    id:1,
                    name:'Guardians of the Galaxy Vol.2',                   
                    release: '10 April 2017',
                    img:'https://www.vintagemovieposters.co.uk/wp-content/uploads/2018/04/IMG_3048.jpg',
                    rating:'7.6'
                },
                {
                    id:1,
                    name:'Doctor Strange',                   
                    release: '4 Nov 2016',
                    img:'https://images-na.ssl-images-amazon.com/images/I/A12-NFRep6L._AC_SL1500_.jpg',
                    rating:'7.5'
                },{
                    id:1,
                    name:'Captain America: Civil War',                   
                    release: '6 May 2016',
                    img:'https://m.media-amazon.com/images/M/MV5BMjQ0MTgyNjAxMV5BMl5BanBnXkFtZTgwNjUzMDkyODE@._V1_.jpg',
                    rating:'7.8'
                },{
                    id:1,
                    name:'Ant-Man',                   
                    release: '24 July 2015',
                    img:'https://images-na.ssl-images-amazon.com/images/I/71E9abm2ayL._AC_SL1111_.jpg',
                    rating:'7.3'
                },{
                    id:1,
                    name:'Avengers: Age of Ultron',                   
                    release: '24 April 2015',
                    img:'https://miro.medium.com/max/1024/1*xvU7rLO4sGBe-3TQxb-Vzw.jpeg',
                    rating:'7.3'
                },{
                    id:1,
                    name:'Guardians of the Galaxy',                   
                    release: '8 August 2014',
                    img:'https://i.pinimg.com/originals/0d/33/60/0d3360b89115be4063c0d5fc763f0e7b.jpg',
                    rating:'8.0'
                },{
                    id:1,
                    name:'The Amazing Spider-Man 2',                   
                    release: '1 May 2014',
                    img:'https://m.media-amazon.com/images/M/MV5BOTA5NDYxNTg0OV5BMl5BanBnXkFtZTgwODE5NzU1MTE@._V1_.jpg',
                    rating:'6.6'
                },{
                    id:1,
                    name:'Captain America: The Winter Soldier',                   
                    release: '4 April 2014',
                    img:'https://i.pinimg.com/originals/cf/30/fe/cf30fe159776b66c1b5679008c9d7f6a.jpg',
                    rating:'7.7'
                },{
                    id:1,
                    name:'Iron Man 3',                   
                    release: '26 April 2013',
                    img:'https://i.pinimg.com/originals/cf/81/52/cf8152447ca6b83acbd3567cb2e05661.jpg',
                    rating:'7.1'
                },{
                    id:1,
                    name:'The Amazing Spider-Man',                   
                    release: '29 June 2012',
                    img:'https://m.media-amazon.com/images/M/MV5BMjMyOTM4MDMxNV5BMl5BanBnXkFtZTcwNjIyNzExOA@@._V1_.jpg',
                    rating:'6.9'
                },{
                    id:1,
                    name:'The Avengers',                   
                    release: '27 April 2012',
                    img:'https://i.pinimg.com/originals/b2/09/0d/b2090d1ae0c016943371b6c01dddcf08.jpg',
                    rating:'8.0'
                },{
                    id:1,
                    name:'Thor',                   
                    release: '29 April 2011',
                    img:'https://i.pinimg.com/originals/1e/c7/5f/1ec75fb52d39d18752561e6e32ec99a5.jpg',
                    rating:'7.0'
                },{
                    id:1,
                    name:'Iron Man 2',                   
                    release: '7 May 2010',
                    img:'https://images-na.ssl-images-amazon.com/images/I/81sC6pkIARL._AC_SL1500_.jpg',
                    rating:'7.0'
                },{
                    id:1,
                    name:'Iron Man',                   
                    release: '1 May 2008',
                    img:'https://images-na.ssl-images-amazon.com/images/I/51GQ3614bqL._AC_.jpg',
                    rating:'7.9'
                },
            ]
        }
    },
    
};
</script>
<style scoped>

</style>