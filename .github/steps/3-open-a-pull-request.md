<!--
  <<< Author notes: Step 3 >>>
  Just a historic note: the previous version of this step forced the learner
  to write a pull request description,
  checked that `main` was the receiving branch,
  and that the file was named correctly.
-->

## Tehtävä 3: Avaa pull request

Olet nyt tehnyt commitin, jonka pitäisi näkyä täällä Githubissa. Seuraavaksi tehdään pull request. Pull requestien idea on jakaa ehdottomasi muutokset muille kehittäjille, jotka voivat joko hyväksyä muutokset tai ehdottaa niihin muutoksia. Pull requesteja ei tarvitse käyttää, kun työskentelee yksin, mutta muiden kanssa työskennellessä niin sanotut koodi katselmoinnit (eng. code review) ovet tärkeä osa kehitysprosessia. Katselmoinnissa muut kehittäjät tarkistavat pull requestissa ehdotetun koodin. Lisätietoa: [About pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)".

### :keyboard: Tehtävä: Tee pull request

Saatat nähdä githubissa viestin, joka kertoo edellisessä kohdassa tekemästäsi git push:sta. Ilmoituksessa on nappi **Compare & pull request**.

![screenshot of message and button](/images/compare-and-pull-request.png)

Voit painaa tätä nappia, joka tekee pull requestin automaattisesti. Jos klikkaat nappia **Compare & pull request**, voit siirtyä suoraan tehtävän kohtaan 6. Jos et paina nappia, alla on ohjeet, miten tehdä pull request manuaalisesti.

1. Klikkaa **Pull requests** välilehteä github repositoriossasi (kannattaa avata repositorio toisessa välilehdessä ja pitää nämä ohjeet auki toisessa)
2. Klikkaa **New pull request**.
3. Valitse **base:** dropdownista **main** vaihtoehto
4. Valitse **compare:** dropdownista `my-first-branch`.

   ![screenshot showing both branch selections](/images/pull-request-branches.png)

5. Klikkaa **Create pull request**.
6. Valitse pull requestillesi otsikko. Oletusarvoisesti otsikko (title) on branchisi nimi. Vaihda otsikoksi teksti `Ensimmäinen tiedosto`.
7. Seuraavassa kentässä sinun tulee antaa kuvaus pull requestillesi. Kuvaukseen kirjoitetaan, mitä olet tehnyt kyseisessä pull requestissa. Tässä tehtävässä voi laittaa viestiksi esimerkiksi "lisäsin tiedoston"

   ![screenshot showing pull request](/images/Pull-request-description.png)

8. Klikkaa **Create pull request**. Sivu ohjautuu automaattisesti luomaasi pull requestiin.
9. Odota n. 20 sekuntia ja päivitä tämä ohje sivu [GitHub Actions](https://docs.github.com/en/actions) päivittää automaattisesti ohjeet seuraavaan tehtävään.