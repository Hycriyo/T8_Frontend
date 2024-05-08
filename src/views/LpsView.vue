<template>
    <main class="lps">
        <h2>
            LP's
        </h2>
        <section class="d-flex justify-content-center">
            <article>
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

<style scoped lang="less">

main>section>article
{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}

main>section>article>div
{
    display: flex;
    border: 1px solid;
    width: calc(100vw - 32px);
    max-width: 600px;
    height: 100vw;
    margin-bottom: 16px;
}


@media screen and (orientation: landscape) and (max-width: 991px)
{
    main>section>article
    {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
    }

    main>section>article>div
    {
        display: flex;
        border: 1px solid;
        width: 400px;
        height: 50vh;
        margin-bottom: 16px;
        margin-left: 8px;
        margin-right: 8px;
    }
}

@media screen and (min-width: 992px)
{
    main>section>article
    {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
    }

    main>section>article>div
    {
        display: flex;
        border: 1px solid;
        width: 600px;
        height: 600px;
        margin-bottom: 16px;
        margin-left: 8px;
        margin-right: 8px;
    }
}
</style>