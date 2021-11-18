
# Tehtävä 3 

## z)Lue ja tiivistä
Luin artikkelin [Markdown references](https://commonmark.org/help/). Artikkeli käsittelee Markdownin yleisimpiä syntakseja.

* Heading: `# "Heading"`
* Heading2: `## "Heading"`
* List: `* "listattava asia"`
* Kuva: `![image]("url")`


## a)Kirjoita raportti MarkDownina
Tässä se tulee tehtyä.

## b)Pull first
Tein muutoksia __Readme.md__ ja kans __MarkDown.md__ tiedostoihin. Tämän jälkeen ajoin muutaman komennon:

      git add --all
      git pull
      git commit
      git push
![image](/pics/bkohta.PNG)

Githubista näin että asiat olivat menneet läpi

## c)Kaikki kirjataan
Komennolla `git log --pretty=oneline` näkee kaikki commitit ja niiden SHA avaimet

![image](/pics/Ckuva1.PNG)

Komennolla `git diff` näyttää muutokset, jotka on tehty viimeisen commitin jälkeen.

![image](/pics/ckohta.PNG)

Toimii ennen kun on tehnyt `git add` tai sitten `git diff --cache` ennen kun on tehnyt git commitin.

Komennolla `git blame <file name>` nähdään milloin tiedoston rivit on lisätty.

![image](/pics/blame.PNG)

## d)Jotain tyhmää

Tein __Readme.md__ tiedostoon tyhmiä muutoksia, jonka jälkeen poistin ne ja tarkistin että ne olivat poistuneet.

Muutosten jälkeen ajoin komennot:

        git add Readme.md
        git reset --hard

![image](/pics/Tyh.PNG)
![image](/pics/Korjattu.PNG)

## d)Formula

Loin init.sls tiedoston h3d nimiseen hakemistoon ja laitoin sinne seuraavat komennot:

![image](/pics/dkohtaa.PNG)

Tämän jälkeen vaan ajoin komennon `sudo salt-call --local -l info state.apply h3d` ja sain seuraavan vastauksen.

![image](/pics/dkohdankuva.PNG)

En ole ihan satavarma että ymmärsinkö tehtävän oikein.
