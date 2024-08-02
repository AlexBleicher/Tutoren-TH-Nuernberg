# Informationen zum Git-Repository

Dieses Repository dient dem Austausch und der Verwaltung von Unterrichtsmaterialien. Jeder ist eingeladen, sich von den bereitgestellten Materialien inspirieren zu lassen und diese unter Angabe des Erstellers zu verwenden.

**WICHTIG**: Vermeidet es unbedingt, alte Klausuren oder urheberrechtlich geschützte Inhalte hochzuladen, die nicht von euch selbst erstellt wurden!

Bitte ladet eure Dateien in den entsprechenden Ordner eures Moduls (falls noch nicht vorhanden, erstellt diesen) unter eurem Namen/Acronym hoch.

# GIT GUIDE

Falls ihr noch nicht mit Git in Kontakt gekommen seid, keine Sorge. Hier ist ein kleiner Leitfaden für die Command-Line.

## Was ist Git und GitHub?

1. **Git**: Ein Versionskontrollsystem, das euch ermöglicht, den Verlauf eurer Dateien zu verfolgen und Änderungen rückgängig zu machen.

2. **GitHub**: Eine Plattform, um eure Git-Repositories online zu verwalten und mit anderen zu teilen. GitHub bietet viele zusätzliche Features, die für diesen Guide jedoch nicht relevant sind.

## Wie verbinde ich Git mit GitHub?

Um Git mit GitHub zu verbinden und eure lokalen Repositories online zu verwalten, befolgt diese Schritte:

1. **SSH-Schlüssel erstellen**:
   - Führt den Befehl `ssh-keygen -t ed25519` aus, um einen neuen SSH-Schlüssel zu erstellen.

2. **SSH-Schlüssel zu GitHub hinzufügen**:
   - Geht auf GitHub zu eurem Profil >> Settings >> SSH and GPG keys >> New SSH key.
   - **WICHTIG**: Ladet nur den **öffentlichen Schlüssel** (.pub-Datei) hoch.
   - Teilt niemals euren privaten Schlüssel!

3. **SSH-Agent starten und Schlüssel hinzufügen**:
   - Startet den SSH-Agenten mit `eval "$(ssh-agent -s)"`.
   - Fügt euren privaten Schlüssel mit `ssh-add [EUER PRIVATE KEY]` hinzu.

## Repository auf eure lokale Maschine klonen

1. **Fork des Repositories erstellen**:
   - Geht auf die GitHub-Seite des Repositories und klickt auf "Fork". Dadurch wird eine Kopie des Repositories in eurem eigenen GitHub-Konto erstellt.

2. **Lokales Repository klonen**:
   - Klont das Repository von eurem Fork mit `git clone git@github.com:[EUER_GITHUB_USERNAME]/Tutoren-TH-Nuernberg.git`.

3. **In das Verzeichnis wechseln**:
   - Wechselt in das Verzeichnis des geklonten Repositories mit `cd Tutoren-TH-Nuernberg`.

## Ihr seid soziale Menschen und wollt eure Materialien teilen?

1. **Pull von der Originalquelle**:
   - Bevor ihr Änderungen vornehmt, stellt sicher, dass euer Fork aktuell ist: `git pull origin main`.

2. **Änderungen vornehmen**:
   - Fügt eure Dateien hinzu mit `git add .`.
   - Committet eure Änderungen mit `git commit -m "Beschreibung der Änderungen"`.

3. **Änderungen in euren Fork pushen**:
   - Push die Änderungen zu eurem Fork mit `git push origin main`.

4. **Pull Request erstellen**:
   - Geht auf GitHub zu eurem Fork.
   - Klickt auf "Compare & pull request".
   - Fügt eine Beschreibung hinzu und klickt auf "Create pull request", um eure Änderungen zur Überprüfung einzureichen.

Jetzt sollten eure Änderungen in der Original-Repository zur Verfügung stehen, und die Maintainer können diese überprüfen und zusammenführen.
