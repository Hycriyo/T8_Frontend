<template>
  <div class="home">
    <h2>
        Home
    </h2>
    <section>
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
    </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'HomeView',
  components: {

  }
}

</script>
