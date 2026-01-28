<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Tehtävä 1: Esivalmistelut ja ensimmäinen haara eli branch

### Esivalmistelut

Ennen kuin aloitat, varmista, että olet tehnyt moodlen tehtävän "gitin käyttöönotto"

### :keyboard: Tehtävä: Repositorion kloonaus ja ensimmäinen haara eli branch

1. Pidä nämä ohjeet auki yhdellä välilehdellä ja avaa selaimessa toinen välilehti, jossa avaat githubissa tämän saman repositorion. 

2. Seuraavaksi haluamme luoda paikallisen kloonin repositoriosta. Käytämme kloonaukseen git bash komentoriviä.

   1. Klikkaa vihreää **< > Code** valikkoa ja kopioi https välilehdeltä löytyvä linkki

   2. Avaa nyt koneellasi git bash komentorivi
   
   3. Päätä, minne omalla koneellasi haluat tallentaa repositorion. Navigoi valitsemaasi hakemistoon (kansioon) komentorivillä käyttäen _cd_ komentoa. 
      - Git bash aukeaa automaattisesti c/Users/käyttäjänimi hakemistosta. 
      - Näet tämän hetkisestä sijainnistasi löytyvät tiedostot ja alahakemistot komennolla _ls_.
      - Pääset esimerkiksi Documents hakemistoon komennolla _cd Documents_
      ![git-bash-example](/images/git-bash-example.png)

   4. Kun olet navigtoinut sopivaan kansioon kloonaa repositosio komennolla `git clone aiemmin-kopioitu-linkki`
      - Huom! ctrl+V ei toimi git bashissa, käytä sen sijaan shift+ins tai klikkaa hiiren oikealla näppäimellä ja valitse paste
      ![git-clone-example](/images/git-clone-example.png)
      - Komento luo paikallisen version repositoriosta, joka on linkitetty githubissa löytyvään remote versioon.

   5. Lopuksi navigoi kloonaamaasi repositorioon cd komennolla `cd github-alkeet`

3. Luo seuraavaksi uusi haara eli branch nimeltä _my-first-branch_. Saat luotua branchin komennolla `git checkout -b my-first-branch`. Huom! on tärkeää, että käytät tismalleen samaa nimeä branchille, jotta tehtävä menee läpi.
   - `git checkout -b` komennossa git checkout kertoo tietokoneelle, että haluamme vaihtaa branchiä. -b taas kertoo, että olemme siirtymässä aivan uuteen branchiin. Tietokone siis ensin tekee uuden branchin ja sen jälkeen siirtyy sinne.
   - Saman voisi tehdä myös kahdella erillisellä komennolla: 1. `git branch my-new-branch` 2. `git checkout my-new-branch`
   - Branch, jossa olet, pitäisi näkyä tiedosto polun vieressä
    ![create-branch](/images/create-branch.png)

4. Olet nyt tehnyt branchin paikalliseen repositorioosi, mutta se pitää vielä julkaista, jotta se näkyy githubissa. Julkaise branchi komenolla `git push -u origin my-first-branch`

5. Odota n. 20 sekuntia ja päivitä sitten tämä sivu. [GitHub Actions](https://docs.github.com/en/actions) päivittää seuraavan tehtään ohjeen tähän automaattisesti.
