<template>
    <main clas="contact">
        <h2>
            Contact Formulier
        </h2>
        <section>
            <article>
                <form>
                    <div>
                        <label for="name">Naam:</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div>
                        <label for="email">Email:</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div>
                        <label for="telefoon">Telefoonnummer:</label>
                        <input type="tel" id="telefoon" name="telefoon" required>
                    </div>
                    <div>
                        <label for="opmerking">Vraag / Opmerking:</label>
                        <input type="text" id="opmerking" name="opmerking" required>
                    </div>
                    <div>
                        <label for="aanmelden">Aanmelden voor nieuwsbrief</label>
                        <input type="checkbox" id="aanmelden" name="aanmelden" required>
                    </div>
                    <div>
                        <input type="submit" value="Contact formulier verzenden">
                    </div>
                </form>
                <!-- <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2482.6437943526366!2d-0.07797572239614403!3d51.51975070979966!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x48761d4a5813272b%3A0x5cece164622283ec!2sVinyl%20Addicts!5e0!3m2!1snl!2snl!4v1710700929362!5m2!1snl!2snl" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe> -->
            </article>
        </section>
    </main>
</template>

<style scoped lang="less">
main>section
{
    display: flex;
}
main>section>article
{
    display: flex;
    align-items: center;
    flex-direction: column;
    width: 100vw;
}

main>section>article>iframe
{
    width: 100vw;
    padding: 16px;
}

main>section>article>form
{
    display: flex;
    flex-direction: column;
    width: 100vw;
    padding: 16px;
}

main>section>article>form>div
{
    display: flex;
    flex-direction: column;
    margin: 4px;
}

main>section>article>form>div>label
{
    text-align: center;
}

main>section>article>form>div>input
{
    text-align: center;
}

#opmerking
{
    height: 10em;
    text-align: left;
}

@media screen and (orientation: landscape) and (max-width: 991px)
{
    main>section>article>form
    {
        max-width: 80vw;
    }
}

@media screen and (min-width: 992px)
{
    main>section>article>form
    {
        max-width: 40vw;
    }
    main>section>article>iframe
    {
        max-width: 40vw;
    }
}
</style>