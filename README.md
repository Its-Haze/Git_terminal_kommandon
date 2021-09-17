<h1 align="center">Börja rätt</h1>

1. Skapa en ny mapp på datorn med filerna du vill lägga ut på github


2. Skapa en fil som heter Readme.md och skriv vad programmet du skapar handlar om innuti readme.md filen


3. Öppna upp mappen via pycharm så ni har projektet öppet med alla filer


4. Gå ner till terminalen inuti Pycharm


<h2 align="center">Kommandon i terminalen ~ i ordning:</h2>

1. git init 
- Detta skapar en lokal Git repository till ditt projekt

2. git status
- Detta kontrollerar vilka filer som har ändrats och kommer förmodligen att ha röd text på den

3. git add .
- Punkten i slutet gör att ALLA filer som ändrats kommer att läggas til
Man kan skriva: git add (filnamnet.py) utan parenteser då. om man endast vill lägga upp 1 fil 

4. Skriv: git status
- Nu när du har gjort git add . så kommer du se att alla röda filer blev nu gröna. alltså e dem redo att bli skickade till github

5. Skapa en repo på github om du inte redan har det och kalla den vad du vill


6. Gå tillbaka till terminalen och skriv - git commit -m "text om vad som ändrats"


7. git branch -M main
- Detta skapar en Main branch

8. git remote add origin https://github.com/"your_repository_name.git
- Byt ut your_repository_name.git med vad din repository heter på github
- T.ex [https://github.com/Erik-Avakian/Git_terminal_kommandon.git]()

9. git push -u origin main
- Detta pushar filerna från din dator till github

10. Klar! kolla github om filerna har laddats upp


<h2 align="center">Nästa gång du ska uppdatera din kod och vill pusha den till Github:</h2>

1. git status
- Kolla vilka filer som ändrats.. dem är i röd text


2. git add (filnamnet)
- t.ex. git add .\README.md == Detta tar endast med README.md filen
- eller git add . == detta gör att alla filer som blev röda under "git status" kommer nu bli gröna och redo för uppladdning


4. git status
-Kolla så filerna blivit gröna nu så dem är redo att laddas upp


5. git commit -m "meddelande om ändringarna"


6. git push
- Om detta inte funkar. testa: git push origin. om inte det heller funkar så testa. git push origin main


<h2 align="center">EXTRA</h2>

Får du denna Error:
"Updates were rejected because the tip of your current branch is behind"
Skriv git push -f origin main
-f står för Force


<h1 align="center">Hur man byter/skapar branches</h1>

1. git checkout -b nyttBranchNamn
- Ersätt nyttBranchNamn med vad du vill döpa din nya branch till

2. git checkout nyttBranchNamn 
- Detta får dig att hoppa från Main branchen till nyttBranchNamn branchen


<h2 align="center">Byta mellan brancher:</h2>

1. git checkout nyttBranchNamn
- Byter från main till nyttBranchNamn 

2. git checkout main
- Återvänder till main branchen

<h2 align="center">Hur man pushar från olika brancher till github</h2> 

1. git checkout nyttBranchNamn

2. git push origin nyttBranchNamn 



<h1 align="center">Av Erik Avakian</h1>

