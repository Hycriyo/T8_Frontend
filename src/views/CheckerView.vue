<template>
    <div class="checker">
        <h2>
            Checker
        </h2>
        <section>
            <article>
                <h3>
                    Vul hier de informatie in:
                </h3>
                <form>
                    <div>
                        <label for="naam">Naam LP:</label>
                        <input type="text" id="naam" name="naam" required>
                    </div>
                    <div>
                        <label for="datum">Jaartal:</label>
                        <input type="text" id="datum" name="datum" required>
                    </div>
                    <div>
                        <label for="limited">Is het een limited edition?</label>
                        <input type="checkbox" id="limited" name="limited" required>
                    </div>
                    <div>
                        <label for="condition">Is de LP in goede conditie?</label>
                        <input type="checkbox" id="condition" name="condition" required>
                    </div>
                    <div>
                        <label for="hoes">Albumhoes conditie:</label>
                        <select id="hoes" name="hoes" required>
                            <option value="">Kies conditie</option>
                            <option value="slecht">Slecht</option>
                            <option value="gebruikt">Gebruikt</option>
                            <option value="zo goed als nieuw">Zo goed als nieuw</option>
                        </select>
                    </div>
                    <div>
                        <input type="submit" value="Informatie ophalen">
                    </div>
                </form>
            </article>
            <article>
                <h3>
                    Uitslag:
                </h3>
            </article>
        </section>
    </div>
</template>