<template>
    <main class="home">
        <h2>
            Home
        </h2>
        <section class="d-flex p-8 flex-lg-row flex-column">
            <article id="slider">
                <div class="images">
                    <img class="img" src="images/slider_images/image1.jpg" alt="Rock and Roll LP">
                </div>
                <div class="images">
                    <img class="img" src="images/slider_images/image2.jpg" alt="Blauwe LP">
                </div>
                <div class="images">
                    <img class="img" src="images/slider_images/image3.jpg" alt="Rode LP">
                </div>
                <a id="prev" onclick="SlidesAction(-1)">&#10094;</a>
                <a id="next" onclick="SlidesAction(1)">&#10095;</a>
            </article>
            <article id="news">
                <div>
                    <a>

                    </a>
                </div>
                <div>
                    <a>

                    </a>
                </div>
                <div>
                    <a>
                        
                    </a>
                </div>
                <div>
                    <a>
                        
                    </a>
                </div>

            </article>
        </section>
    </main>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'HomeView',
  components: {

  }
}

</script>

<style scoped lang="less">
@accentkleur: #F64E8B;

main>section
{
    padding: 8px;
}

main>section>article
{
    display: flex;
    border: 1px solid;
    margin-bottom: 16px;
    height: 100vw;
    width: 100%;
}

#news
{
    display: flex;
    flex-direction: column;
    align-content: space-around;
    justify-content: space-around;
    height: 200vw;
    border: none;
}

#news>div
{
    border: solid 1px;
    height: 25%;
    margin-bottom: 16px;
}

#slider
{
    max-width: 1000px;
    position: relative;
}

.images 
{
    display: none;
    justify-content: center;
    height: 100%;
    width: 100%;
    object-position: contain;
}

.img
{
    width: 100%;
    height: 100%;
    object-fit: cover;
}

#prev,#next
{
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    margin-top: -46px;
    padding: 16px;
    color: @accentkleur;
    font-weight: bold;
    font-size: 32px;
    transition: 0.2s ease;
    border-radius: 0 3px 3px 0;
    user-select: none;
}
#next
{
    right: 0;
    border-radius: 3px 0 0 3px;
}

#prev:hover,#next:hover
{
    color: black;
}

@media screen and (orientation: landscape) and (max-width: 991px)
{
    main>section>article
    {
        height: 80vh;
    }
}

@media screen and (min-width: 992px)
{
    main>section
    {
        flex-direction: row;
        justify-content: space-around;
    }
    main>section>article
    {
        max-width: 40vw;
        max-height: 40vw;
    }

    #news
    {
        flex-wrap: wrap;
        flex-direction: row;
    }

    #news>div
    {
        height: 45%;
        width: 45%;
    }
}
</style>
