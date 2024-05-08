<template>
    <main class="over_ons">
        <h2>
            Over Ons
        </h2>
        <section>
            <article>
                <p>
                    Vinyl Addicts is een webwinkel met uitsluitend tweedehands vinyl singles en lp’s. Er is continu nieuw aanbod in allerlei genres. 
                    Zo kan het aanbod iedere keer variëren van mooie classic albums tot leuke 1,00 euro singles voor in de jukebox.
                </p>
                <p>
                    Al onze platen zijn in zeer goed afspeelbare staat, alhoewel we er soms voor kiezen om zeldzamere platen van iets mindere kwaliteit toch te plaatsen. 
                    Dit staat dan altijd duidelijk aangegeven door middel van een omschrijving of een van de volgende codes:
                </p>
                <ul>
                    <li>
                        NM (Near Mint) – In nieuwstaat<br><br>
                    </li>
                    <li>
                        VG+ (Very Good Plus) - Enkele gebruikerssporen en in zeer goede afspeelbare staat<br><br>
                    </li>
                    <li>
                        VG (Very Good) – Wat meer gebruikerssporen en in goede afspeelbare staat<br><br>
                    </li>
                    <li>
                        G+ (Good Plus) – Behoorlijk wat gebruikerssporen, maar nog steeds goed afspeelbaar
                    </li>
                </ul>
                <p>
                    M (Mint) is niet van toepassing, omdat deze code alleen geldt voor nieuw vinyl.<br><br>
                    G (Good) en F (Fair) is ook niet aanwezig, aangezien deze kwaliteit niet goed afspeelbaar is en daarom bieden we dit ook niet aan.
                </p>
                <p>
                    Voor de hoezen gelden dezelfde codes (NM, VG+, VG en G+) wat respectievelijk betekent van nieuwstaat tot gebruikte staat met eventueel stickers, namen op hoes en soms seam split (ingescheurde hoes).
                </p>
            </article>
        </section>
    </main>
</template>

<style scoped lang="less">
main>section
{
    display: flex;
    justify-content: center;
}
main>section>article
{
    display: flex;
    flex-direction: column;
    
    width: 100vw;
    padding: 32px;
    padding-top: 0;
}

@media screen and (orientation: landscape) and (max-width: 991px)
{
    main>section>article
    {
        width: 650px;
    }
}

@media screen and (min-width: 992px)
{
    main>section>article
    {
        width: 650px;
    }
}
</style>