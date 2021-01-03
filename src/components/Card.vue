<template>
    <div>         
        <b-card
            :title="movieData.name"
            :img-src="movieData.img"
            img-alt="Image"
            img-top
            img-height="380"
            tag="article"
            style="max-width: 20rem;"
            class="mb-2"
        >
            <b-card-text>
             {{movieData.desc}}
            </b-card-text>
            <b-card-sub-title>Release Date:
                {{movieData.release}} <br><br>
            </b-card-sub-title>
            <b-card-footer class="mb-3">IMDb Rating:
                {{movieData.rating}}  
            </b-card-footer>

            <b-button href="#" variant="primary">Download</b-button>
        </b-card>
    </div>
</template>
<script>
export default {
    name: 'Card',
    props:['movieData'],
     
}
</script>