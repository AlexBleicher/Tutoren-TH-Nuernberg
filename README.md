# Informationen zum Git-Repository
Dieses Repository hat den Zweck, damit ihr eure Unterrichtsmaterialiern miteinander teilen könnt. 
Achtet bitte darauf, dass eure Materialen das Copyright verlieren, sobald diese hier hochgeladen wurden. 
Es ist angedacht, dass jeder seine Materialien hochladen kann, sowie die Materialien der anderen benutzen kann.

**WICHTIG**: Ladet bitte um keine Umstände Altklausuren oder Copyright geschütze Inhalte hoch, die ihr nicht selbst erstellt habt!

# GIT GUIDE
Viele von euch werden vermutlich noch nicht mit git in Kontakt gekommen sein. Das ist kein Problem. Hier ein kleiner Guide für die Command-Line

## Das erste mal git/GitHub?

Ihr werdet in eurer Laufbahn als Informatiker früher oder später mit git in Kontakt kommen. Dazu solltet ihr den Umgang damit beherrschen. 
Falls du noch nie damit gearbeitet hast, ist das ein kleiner Leitfaden.

1. Was ist git?

-> Git ist ein Versionskontrollprogramm. Ihr könnt euch das so vorstellen: Statt einen Text nach jedem Paragraphen in einer Datei zu speichern, um eure Veränderungen im Blick zu haben, könnt ihr git nutzen. Git übernimmt den Prozess des Speicherns eurer Historie. Text=Code, kann aber auch normaler Plain Text o.ä. sein

2. Was ist GitHub?

-> GitHub ist eine Plattform, auf der ihr eure lokalen Repositories online verwalten könnt und den Zugang mit anderen Teilen könnt. Außerdem bietet die Plattform noch sehr viele weitere Features, die aber für den Gebrauch dieses Repositories irrelevant sind.

3. Wie verbinde ich git mit GitHub?

> Um git mit GitHub zu verbinden und eure lokalen Repositories verwalten zu können, müsst ihr folgendes tun:
1. ssh-keypair erstellen : ssh-keygen -t ed 25519
2. Auf GitHub oben Rechts auf euer Profil >> Settings >> SSH and GPG keys >> New SSH key
3. **GANZ WICHTIG**: hier ladet ihr euren **PUBLIC KEY** hoch. Das ist die Datei, die mit .pub endet.
4. Teilt unter keinen Umständen euren Private-Key mit jemand anderem!
5. Bindet euren ssh-key mit eurem ssh-agent ein.
- SSH-Agent starten. Unter Linux : ``eval "$(ssh-agent -s)"``
- ``ssh-add [EUER PRIVATE KEY]``
-> Eigentlich seid ihr ab hier schon fertig. Um eure lokalen Reposiories hochzuladen, findet ihr im folgenden noch eine Anleitung.

## Repository auf eure lokale Maschine laden

1. Initialisiert ein lokales Repository : ``git init .`` (Macht das in einem neuen Ordner)
2. Fügt das remote Repository eurer Maschine hinzu: ``git remote add origin git@github.com:Pand3ru/Tutoren-TH-Nuernberg.git``
3. Synchronisiert den Branch ``git branch -M main``
4. Zieht euch das Repository ``git pull``
5. ``git push -u origin main``

-> Jetzt solltet ihr in eurem Ordner den gesamten Inhalt des auf GitHub gehostetem git-Repository haben

## Ihr seid gute Menschen und wollt eure Materialien teilen?

1. Pulled nochmal, damit alles am ende gut läuft : ``git pull``
2. Fügt eure Datein hinzu : ``git add .`` (. bezieht sich auf den gesamten Inhalt des aktuellen Ordners. Stattdessen könnt ihr auch einfach Dateinamen schreiben)
3. ``git commit -m "Schreibt hier rein, was ihr hinzugefügt/verändert habt. Diese Nachricht ist ganz wichtig!"``
4. Ladet hoch: ``git push -u origin main`` oder ``git push``

-> Jetzt sollten alle eure Datein mit hochgeladen sein

