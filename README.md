<header>

<!--
  <<< Author notes: Course header >>>
  Include a 1280×640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Add your open source license, GitHub uses MIT license.
-->

## Git perusteet
<!-- readme -->

Näissä tehtävissä opetellaan gitin ja githubin käytön perusteet. Lisämateriaalia tehtävien teon avuksi löytyy moodlesta.

Kun olet tehnyt tehtävät, näytä opettajalle, että olet saanut ne valmiiksi.


### Näin aloitat tehtävät:

1. Oikea-klikkaa **Start course** ja avaa linkki uudella välilehdellä
2. Uudella välilehdellä suurin osa kentistä on täytetty sinulle valmiiksi.
  -Owner kenttään valitse oma tilisi
  -Repositorio kannattaa jättää julkiseksi, koska tehtävät käyttävät github actions ominaisuutta, joka on julkisissa repositorioiss täysin ilmainen mutta yksityisissä ilmaista käyttöaikaa on rajallinen määrä (voit poistaa repositorion, kun olet näyttänyt opettajalle olevasi valmis)
  -Skrollaa alas ja paina **Create repository**
3. Kun repositorio on luotu, odota n. 20 sekuntia ja sen jälkeen päivitä tämä sivu. Ohjeeet päivittyvät uuden repositoriosi README sivulle. Sen jälkeen voit sulkea tämän välilehden.

[![Aloita](https://user-images.githubusercontent.com/1221423/235727646-4a590299-ffe5-480d-8cd5-8194ea184546.svg)](https://github.com/new?template_owner=linntahtiomnia&template_name=introduction-to-github2&owner=%40me&name=skills-introduction-to-github3&description=My+clone+repository&visibility=public)

<!-- endreadme -->
<footer>

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

3. Luo seuraavaksi uusi haara eli branch nimeltä _my-first-branch_. Saat luotua branchin komennolla `git checkout -b my-first-branch`. Huom! on tärkeää, että käytät tismalleen samaa nimeä branchille, jotta tehtävä menee läpi.
   - `git checkout -b` komennossa git checkout kertoo tietokoneelle, että haluamme vaihtaa branchiä. -b taas kertoo, että olemme siirtymässä aivan uuteen branchiin. Tietokone siis ensin tekee uuden branchin ja sen jälkeen siirtyy sinne.
   - Saman voisi tehdä myös kahdella erillisellä komennolla: 1. `git branch my-new-branch` 2. `git checkout my-new-branch`
   - Branch, jossa olet, pitäisi näkyä tiedosto polun vieressä
    ![create-branch](/images/create-branch.png)

4. In the field, name your branch `my-first-branch`. In this case, the name must be `my-first-branch` to trigger the course workflow.
5. Click **Create branch: my-first-branch** to create your branch.

   ![create-branch-button](/images/create-branch-button.png)

   The branch will automatically switch to the one you have just created.
   The **main** branch drop-down bar will reflect your new branch and display the new branch name.

6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 2: Commit a file

_You created a branch! :tada:_

Creating a branch allows you to edit your project without changing the `main` branch. Now that you have a branch, it’s time to create a file and make your first commit!

**What is a commit?**: A _[commit](https://docs.github.com/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits)_ is a set of changes to the files and folders in your project. A commit exists in a branch. For more information, see "[About commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits)".

### :keyboard: Activity: Your first commit

The following steps will guide you through the process of committing a change on GitHub. A commit records changes in renaming, changing content within, creating a new file, and any other changes made to your project. For this exercise, committing a change requires first adding a new file to your new branch.

> [!NOTE]
> `.md` is a file extension that creates a Markdown file. You can learn more about Markdown by visiting "[Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)" in our docs or by taking the "[Communicating using Markdown](https://github.com/skills/communicate-using-markdown)" Skills course.

1. On the **< > Code** tab in the header menu of your repository, make sure you're on your new branch `my-first-branch`.

2. Select the **Add file** drop-down and click **Create new file**.

   ![create new file option](/images/create-new-file.png)

3. In the **Name your file...** field, enter `PROFILE.md`.

4. In the **Enter file contents here** area, copy the following content to your file:

   ```
   Welcome to my GitHub profile!
   ```

   ![profile.md file screenshot](/images/my-profile-file.png)

5. Click **Commit changes...** in the upper right corner above the contents box. For commits, you can enter a short commit message that describes what changes you made. This message helps others know what's included in your commit. GitHub offers a simple default message, but let's change it slightly for practice. First, enter `Add PROFILE.md` in the first text-entry field titled "Commit message".

   ![screenshot of adding a new file with a commit message](/images/commit-full-screen.png)

6. In this lesson, we'll ignore the other fields and click **Commit changes**.
7. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

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

3. Luo seuraavaksi uusi haara eli branch nimeltä _my-first-branch_. Saat luotua branchin komennolla `git checkout -b my-first-branch`. Huom! on tärkeää, että käytät tismalleen samaa nimeä branchille, jotta tehtävä menee läpi.
   - `git checkout -b` komennossa git checkout kertoo tietokoneelle, että haluamme vaihtaa branchiä. -b taas kertoo, että olemme siirtymässä aivan uuteen branchiin. Tietokone siis ensin tekee uuden branchin ja sen jälkeen siirtyy sinne.
   - Saman voisi tehdä myös kahdella erillisellä komennolla: 1. `git branch my-new-branch` 2. `git checkout my-new-branch`
   - Branch, jossa olet, pitäisi näkyä tiedosto polun vieressä
    ![create-branch](/images/create-branch.png)

4. In the field, name your branch `my-first-branch`. In this case, the name must be `my-first-branch` to trigger the course workflow.
5. Click **Create branch: my-first-branch** to create your branch.

   ![create-branch-button](/images/create-branch-button.png)

   The branch will automatically switch to the one you have just created.
   The **main** branch drop-down bar will reflect your new branch and display the new branch name.

6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Step 3 >>>
  Just a historic note: the previous version of this step forced the learner
  to write a pull request description,
  checked that `main` was the receiving branch,
  and that the file was named correctly.
-->

## Step 3: Open a pull request

_Nice work making that commit! :sparkles:_

Now that you have made a change to the project and created a commit, it’s time to share your proposed change through a pull request!

**What is a pull request?**: Collaboration happens on a _[pull request](https://docs.github.com/en/get-started/quickstart/github-glossary#pull-request)_. The pull request shows the changes in your branch to other people and allows people to accept, reject, or suggest additional changes to your branch. In a side by side comparison, this pull request is going to keep the changes you just made on your branch and propose applying them to the `main` project branch. For more information about pull requests, see "[About pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)".

### :keyboard: Activity: Create a pull request

You may have noticed after your commit that a message displayed indicating your recent push to your branch and providing a button that says **Compare & pull request**.

![screenshot of message and button](/images/compare-and-pull-request.png)

To create a pull request automatically, click **Compare & pull request**, and then skip to step 6 below. If you don't click the button, the instructions below walk you through manually setting up the pull request.

1. Click on the **Pull requests** tab in the header menu of your repository.
2. Click **New pull request**.
3. In the **base:** dropdown, make sure **main** is selected.
4. Select the **compare:** dropdown, and click `my-first-branch`.

   ![screenshot showing both branch selections](/images/pull-request-branches.png)

5. Click **Create pull request**.
6. Enter a title for your pull request. By default, the title will automatically be the name of your branch. For this exercise, let's edit the field to say `Add my first file`.
7. The next field helps you provide a description of the changes you made. Here, you can add a description of what you’ve accomplished so far. As a reminder, you have: created a new branch, created a file, and made a commit.

   ![screenshot showing pull request](/images/Pull-request-description.png)

8. Click **Create pull request**. You will automatically be navigated to your new pull request.
9. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

> [!NOTE]
> You may see evidence of GitHub Actions running on the tab with the pull request opened! The image below shows a line you might see on your pull request after the Action finishes running.
> 
> ![screenshot of an example of an actions line](/images/Actions-to-step-4.png)

<footer>

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

3. Luo seuraavaksi uusi haara eli branch nimeltä _my-first-branch_. Saat luotua branchin komennolla `git checkout -b my-first-branch`. Huom! on tärkeää, että käytät tismalleen samaa nimeä branchille, jotta tehtävä menee läpi.
   - `git checkout -b` komennossa git checkout kertoo tietokoneelle, että haluamme vaihtaa branchiä. -b taas kertoo, että olemme siirtymässä aivan uuteen branchiin. Tietokone siis ensin tekee uuden branchin ja sen jälkeen siirtyy sinne.
   - Saman voisi tehdä myös kahdella erillisellä komennolla: 1. `git branch my-new-branch` 2. `git checkout my-new-branch`
   - Branch, jossa olet, pitäisi näkyä tiedosto polun vieressä
    ![create-branch](/images/create-branch.png)

4. In the field, name your branch `my-first-branch`. In this case, the name must be `my-first-branch` to trigger the course workflow.
5. Click **Create branch: my-first-branch** to create your branch.

   ![create-branch-button](/images/create-branch-button.png)

   The branch will automatically switch to the one you have just created.
   The **main** branch drop-down bar will reflect your new branch and display the new branch name.

6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 2: Commit a file

_You created a branch! :tada:_

Creating a branch allows you to edit your project without changing the `main` branch. Now that you have a branch, it’s time to create a file and make your first commit!

**What is a commit?**: A _[commit](https://docs.github.com/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits)_ is a set of changes to the files and folders in your project. A commit exists in a branch. For more information, see "[About commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits)".

### :keyboard: Activity: Your first commit

The following steps will guide you through the process of committing a change on GitHub. A commit records changes in renaming, changing content within, creating a new file, and any other changes made to your project. For this exercise, committing a change requires first adding a new file to your new branch.

> [!NOTE]
> `.md` is a file extension that creates a Markdown file. You can learn more about Markdown by visiting "[Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)" in our docs or by taking the "[Communicating using Markdown](https://github.com/skills/communicate-using-markdown)" Skills course.

1. On the **< > Code** tab in the header menu of your repository, make sure you're on your new branch `my-first-branch`.

2. Select the **Add file** drop-down and click **Create new file**.

   ![create new file option](/images/create-new-file.png)

3. In the **Name your file...** field, enter `PROFILE.md`.

4. In the **Enter file contents here** area, copy the following content to your file:

   ```
   Welcome to my GitHub profile!
   ```

   ![profile.md file screenshot](/images/my-profile-file.png)

5. Click **Commit changes...** in the upper right corner above the contents box. For commits, you can enter a short commit message that describes what changes you made. This message helps others know what's included in your commit. GitHub offers a simple default message, but let's change it slightly for practice. First, enter `Add PROFILE.md` in the first text-entry field titled "Commit message".

   ![screenshot of adding a new file with a commit message](/images/commit-full-screen.png)

6. In this lesson, we'll ignore the other fields and click **Commit changes**.
7. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

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

3. Luo seuraavaksi uusi haara eli branch nimeltä _my-first-branch_. Saat luotua branchin komennolla `git checkout -b my-first-branch`. Huom! on tärkeää, että käytät tismalleen samaa nimeä branchille, jotta tehtävä menee läpi.
   - `git checkout -b` komennossa git checkout kertoo tietokoneelle, että haluamme vaihtaa branchiä. -b taas kertoo, että olemme siirtymässä aivan uuteen branchiin. Tietokone siis ensin tekee uuden branchin ja sen jälkeen siirtyy sinne.
   - Saman voisi tehdä myös kahdella erillisellä komennolla: 1. `git branch my-new-branch` 2. `git checkout my-new-branch`
   - Branch, jossa olet, pitäisi näkyä tiedosto polun vieressä
    ![create-branch](/images/create-branch.png)

4. In the field, name your branch `my-first-branch`. In this case, the name must be `my-first-branch` to trigger the course workflow.
5. Click **Create branch: my-first-branch** to create your branch.

   ![create-branch-button](/images/create-branch-button.png)

   The branch will automatically switch to the one you have just created.
   The **main** branch drop-down bar will reflect your new branch and display the new branch name.

6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>
