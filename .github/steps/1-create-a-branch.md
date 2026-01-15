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

2. Seuraavaksi haluamme luoda paikallisen kloonin repositoriosta. Voit käyttää tähän vs coden työkaluja tai tehdä sen komentorivillä. Alla on ohjeet komentorivin käyttöön mutta moodlesta löytyy ohjeet myös vs coden työkaluille. Komentorivin käytön opettelu on suositeltavaa!

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

3. Luo seuraavaksi uusi haara eli branch nimeltä _my-first-branch_. Saat luotua branchin komennolla `git checkout -b my-first-branch`
   - `git checkout -b` komennossa git checkout kertoo tietokoneelle, että haluamme vaihtaa branchiä. -b taas kertoo, että olemme siirtymässä aivan uuteen branchiin. Tietokone siis ensin tekee uuden branchin ja sen jälkeen siirtyy sinne.
   - Saman voisi tehdä myös kahdella erillisellä komennolla: 1. `git branch my-new-branch` 2. `git checkout my-new-branch`
   -

4. In the field, name your branch `my-first-branch`. In this case, the name must be `my-first-branch` to trigger the course workflow.
5. Click **Create branch: my-first-branch** to create your branch.

   ![create-branch-button](/images/create-branch-button.png)

   The branch will automatically switch to the one you have just created.
   The **main** branch drop-down bar will reflect your new branch and display the new branch name.

6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
