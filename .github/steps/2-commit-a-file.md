<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Tehtävä 2: Lisätään uusi tiedosto ja tehdään commit

_Teit uuden branchin! :tada:_

Brancheja (suomeksi haara) käytetään silloin, kun halutaan muokata projektia ilman, että muutokset menevät päähaaraan eli `main` -branchiin.

Tässä tehtävässä lisätään uusi tiedosto aiemmin luotuun branchiin, tehdään commit ja 'pushataan' muutoset githubiin.

### :keyboard: Tehtävä: Ensimmäinen commit

1. Pidä nämä ohjeet auki selaimessa ja noudata ohjeita git bashissa ja editorissa.

2. Avaa taas git bash. Varmista, että olet edelleen repositorion kansiossa ja aiemmin tekemässäsi branchissa, ja suorita komento `git pull`
   - Tällä komennolla varmistat, että lokaali versiosi sisältää kaikki remote version muutokset.

3. Suorita git bashissa komento `code uusi_tiedosto.md`. Se tekee uuden markdown tiedoston nimeltä 'uusi_tiedosto.md' ja avaa sen vs codessa.
   - Markdown on tiedostotyyppi, jonka pystyy helposti kääntämään pdf:ksi. Github osaa automaattisesti näyttää markdown tiedostot luettavassa muodossa, ja esimerkiksi readme tiedostot ovat yleensä markdown formaatissa.

4. Edellisen komennon jälkeen sinulla pitäisi nyt olla auki vs code ja siellä luomasi markdown tiedosto. Kopioi tiedostoon seuraava teksti ja tallenna (ctrl+S pikanäppäin tallentaa tiedoston)
   ```
   Tämä on uusi tiedosto!
   ```

5. Palaa nyt git bashiin ja suorita komento `git status`
   - `git status` komennolla näet, mihin tiedostoihin on tehty muutoksia, kun verrataan paikallista ja remote versiota repositoriosta
   - Äsken luomasi tiedosto pitäisi näkyä listassa punaisena, koska se on 'untracked' eli sitä ei ole olemassa remote repositoriossa
    ![git-status-example](/images/git-status-example.png)

6. Lisätään tiedosto staged tilaan (eli odottamaan commitin tekoa) `git add uusi_tiedosto.md` komennolla. 
   - `git add` -komento voidaan suorittaa joko yksittäiselle tiedostolle lisäämällä komennon perään lisättävän tiedoston nimi tai lisätä kaikki muutoksia sisältävät tiedostot kerralla komennolla `git add .`

7. Suorita `git status` komento uudelleen. 
   - Uuden tiedoston pitäisi nyt lukea "changes to be committed" listassa vihreänä
   ![stage-changes-example](/images/stage-changes-example.png)
   - Nyt olemme valmiita tekemään commitin. Commitiin lisätään kaikki "changes to be committed" listan muutokset.
   - Muutoksia voi tarkastella tarkemmin `git diff` komennolla. Jos haluat verrata paikallisia ja remote versioita, suorita komento `git diff origin`

8. Tee seuraavaksi commit. Pystymme tekemään commitin ja lisäämään sille viestin yhdellä komennolla `git commit -m "lisää ensimmäinen tiedosto"`
   - On mahdollista myös suorittaa pelkkä `git commit` -komento ja sen jälkeen kirjoittaa commit-viesti avautuvassa editorissa.
   - Hyvän commit-viestin sisällöstä on lisätietoa moodlessa
   - Voit nyt suorittaa vielä kerran `git status`-komennon. Tietokoneen pitäisi kertoa sinulle, että branchisi on yhden commitin verran edellä remote versiota.

9. "Pushaa" commit suorittamalla komento `git push`

10. Odota jälleen n. 20 sekuntia ja sitten päivitä tämä sivu. [GitHub Actions](https://docs.github.com/en/actions) päivittää seuraavan tehtään ohjeen tähän automaattisesti.