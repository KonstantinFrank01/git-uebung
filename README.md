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

### Dateien aus dem remote-repo entfernen

## Status des Git-Working-Directories ansehen

```
git status

```

## Pretty Printing für Git-Logs

## Zweige (Branches) für eigene Features erstellen

### Branch wechseln

### Branch mergen

## Pull requests durchführen

## Commits taggen

## Einen Release-Eintrag im Github erstellen (inkl. Doku)

## Verwerfen der lokalen Änderungen

### Was bedeutet ```stash```