<h1 align="center">Börja rätt</h1>

Om du inte har git installerat. Följ denna guiden --> [github.com/git/quickstart](https://docs.github.com/en/get-started/quickstart/set-up-git)  

När det är klart så kan du börja med att  :


1. Skapa en ny mapp på datorn med filerna du vill lägga ut på github


2. Skapa en fil som heter README.md och skriv vad programmet du skapar handlar om inuti readme.md filen


3. Öppna upp mappen via pycharm så ni har projektet öppet med alla filer


4. Gå ner till terminalen inuti Pycharm

---

<h2 align="center">Kommandon i terminalen ~ i ordning:</h2>

1. ```git init ```
- Detta skapar en lokal Git repository till ditt projekt

2. ```git status```
- Detta kontrollerar vilka filer som har ändrats och kommer förmodligen att ha röd text på den

3. ```git add .```
- Punkten i slutet gör att ALLA filer som ändrats kommer att läggas til
Man kan skriva: git add (filnamnet.py) utan parenteser då. om man endast vill lägga upp 1 fil 

4. ```git status```
- Nu när du har gjort git add . så kommer du se att alla röda filer blev nu gröna. alltså e dem redo att bli skickade till github

5. Skapa en repo på [github](https://github.com/new) om du inte redan har det och kalla den vad du vill. Klicka på länken ---> [github.com/new](https://github.com/new) om du inte hittar hur du ska göra

<h3 align="center">Återvänd till terminalen.</h3>

6. ```git commit -m "my first commit"```


7. ```git branch -M main```
- Detta skapar en Main branch

8. ```git remote add origin https://github.com/"your_repository_name.git```
- Byt ut your_repository_name.git med vad din repository heter på github
- T.ex [https://github.com/Erik-Avakian/Git_terminal_kommandon.git]()

9. ```git push -u origin main```
- Detta pushar filerna från din dator till github

10. Klar! kolla github om filerna har laddats upp

---

<h2 align="center">Nästa gång du ska uppdatera din kod och vill pusha den till Github:</h2>

1. ```git status```
- Kolla vilka filer som ändrats.. dem är i röd text


2. ```git add (filnamnet)```
- t.ex. git add .\README.md = Detta tar endast med README.md filen
- eller git add . == detta gör att alla filer som blev röda under "git status" kommer nu bli gröna och redo för uppladdning


4. ```git status```
-Kolla så filerna blivit gröna nu så dem är redo att laddas upp


5. ```git commit -m "meddelande om ändringarna"```


6. ```git push```
- Om detta inte funkar. testa: 


- ```git push origin```. 


- om inte det heller funkar så testa. 
- ```git push origin main```

---

<h2 align="center">Ta bort filer i din commit:</h2>

Om du gjort (git add .) med punkten i slutet kommer alla filer att läggas till i din nästa commit..
om du vill ta bort specefika filer så skriver du

`git restore --staged filnamnet.py`

Om du vill ta bort en specefik fil:

`git restore --staged '.\Vecka2\Uppgift 10.py'`

om du vill ta bort en hel mapp med alla filer i den:

`git restore --staged .\Vecka2\`

---

<h1 align="center">Hur man Forkar en repository</h1>

Gå in på repot du vill forka och klicka fork.

<img src="https://docs.github.com/assets/images/help/repository/fork_button.jpg"/> 

Sedan Klonar du din "Forkade repository"

---

<h1 align="center">Hur man Klonar ett repository</h1>

1. Gå till repot du vill Klona.  


2. Klicka på "Code" Knappen

<img  src="https://docs.github.com/assets/images/help/repository/code-button.png" />

3. Kopiera "Clone with HTTPS"

<img src="https://docs.github.com/assets/images/help/repository/https-url-clone-cli.png"/> 

4. Öppna pycharm


5. Skapa / Öppna en ny mapp där du vill att dem clonade filerna ska sparas i (Den nya mappen ska vara tom)


6. Skriv: `git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`
- Ersätt självklart denna länken med den du kopierade från Github


7. Klicka ENTER för att skapa din lokala "Clone" av repot från Github
```
$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
> Cloning into `Spoon-Knife`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.
```




<h2 align="center">ERRORS</h2>

---
##### Error message: "Updates were rejected because the tip of your current branch is behind"

### LÖSNING:
```git push -f origin main```
- -f står för Force
---

##### Error message: "Logon failed, use ctrl+c to cancel basic credential prompt "

### LÖSNING:
Om detta händer dig så är du inte på den senaste versionen av Git
Skriv in kommandot nedan i Terminalen baserat på ditt operativsystem.

Windows: `git update-git-for-windows`

Linux/Unix: 
```
#!/bin/bash
sudo add-apt-repository -y ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git -y
```

---


<h1 align="center">Hur man byter/skapar branches</h1>

1. `git checkout -b nyttBranchNamn`
- Ersätt nyttBranchNamn med vad du vill döpa din nya branch till

2. `git checkout nyttBranchNamn`
- Detta får dig att hoppa från Main branchen till nyttBranchNamn branchen

---

<h2 align="center">Byta mellan brancher:</h2>

1. `git checkout nyttBranchNamn`
- Byter från main till nyttBranchNamn 

2. `git checkout main`
- Återvänder till main branchen

---

<h2 align="center">Hur man pushar från olika brancher till github</h2> 

1. `git checkout nyttBranchNamn`

2. `git push origin nyttBranchNamn`

---

<h1 align="center">Av Erik Avakian</h1>

