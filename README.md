# git-uebung

## Erstellen eines Projektes

```
echo "# git-uebung" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/KonstantinFrank01/git-uebung.git
git push -u origin master

```

## Ein Projekt aus dem Repo downloaden (clonen)

```
git clone https://github.com/KonstantinFrank01/git-uebung.git

```

## Neue und/oder geänderte Dateien ins das Repo einpflegen

### Dateien in die Staging Area einpflegen

Eine bestimmte Datei in die Staging Area einpflegen

```
git add <file>
git add README.md

```
Ein ganzes Verzeichnis in die Staging Area einpflegen

```
git add <directory>
git add git-uebung

```

Alle Änderungen in die Staging Area einpflegen

```
git add .

```

### Dateien aus der Staging Area entfernen

Eine Datei aus der Staging Area entfernen ohne die Modifizierung rückgängig zu machen.

```
git reset HEAD <file>
git reset HEAD README.md

```

### Dateien in das local-repo einpflegen

```
git commit -m "commit message"

```

### Dateien aus dem local-repo entfernen

Die Datei aus dem lokalen Repo entfernen und auch vom File-System löschen.

```
git rm <file>
git rm README.md

```

Die Datei aus dem lokalen Repo entfernen und NICHT vom File-System löschen

```
git rm --cached <file>
git rm --cached README.md

```

### Dateien in das remote-repo einpflegen

Eine Datei vom lokalen Repository ins Remote-Repository "pushen"

```
git push <remote> <branch>
git push origin master
git push origin feature2

```

### Dateien aus dem remote-repo entfernen

## Status des Git-Working-Directories ansehen

Den aktuellen Status des Working-Trees anzeigen lassen

```
git status

```

## Pretty Printing für Git-Logs

<https://stackoverflow.com/questions/1057564/pretty-git-branch-graphs>

## Zweige (Branches) für eigene Features erstellen

Branch erstellen

```
git branch <feature_branch>

```
In den Branch wechseln

```
git checkout <feature_branch>

```

Änderungen in dem Branch stagen/committen

```
(git add .
git commit -m "adding a change from the feature branch")

```
Wieder in den Master-Branch zurück wechseln

```
git checkout master

```

Die Änderungen des feature_branch ins remote repo pushen

```
git push origin <feature_branch>

```

### Branch wechseln

```
git checkout <branch_name>

```

Checkout bei einem Remote Branch

```
git fetch 
git checkout <remote_branch>

```

### Branch mergen

In den Branch wechseln in den gemerged werden soll (Bei einem Feature z.B. Master-Branch)

```
git checkout master

``` 

Jetzt den gewünschten Branch in den Master (hinein-)mergen

```
git merge <branch_name>

```

## Pull requests durchführen

## Commits taggen

## Einen Release-Eintrag im Github erstellen (inkl. Doku)

## Verwerfen der lokalen Änderungen

### Was bedeutet ```stash```