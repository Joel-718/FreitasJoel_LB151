# Projekt-Dokumentation

✍️ Ihr Nachname

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|       | 0.0.1   | ✍️ Jedes Mal, wenn Sie an dem Projekt arbeiten, fügen Sie hier eine neue Zeile ein und beschreiben in *einem* Satz, was Sie erreicht haben. |
|       | 0.0.2   |                                                              |
|       | 0.0.3   |                                                              |
|       | 0.0.4   |                                                              |
|       | 0.0.5   |                                                              |
|       | 0.0.6   |                                                              |
|       | 1.0.0   |                                                              |

# 0 Ihr Projekt

✍️ Beschreiben Sie Ihr Projekt in einem griffigen Satz.

# 1 Analyse

✍️ Beschreiben Sie, auf welchem Tier Sie die dynamischen Elemente der Anwendung unterbringen möchten:

* Tier 1 (Presentation):
* 
* Der Spieler versucht in einem Gitter Wörter oder Redewendungen zu erraten, indem er Buchstaben an der Rate-Wand ratet, wobei er bestrebt ist, möglichst hohe Geldbeträge zu gewinnen. Eine Kategorie wird vorab genannt und Satzzeichen und Ziffern sind bereits an der Rate-Wand vorhanden.

* Tier 2 (Webserver):
* 
* Im zweiten Teil des Spiels dreht der Spieler ein Glücksrad, um unterschiedliche Felder zu erhalten, die entweder Geldbeträge beinhalten, durch die der Spieler durch Raten von Konsonanten oder Kaufen von Vokalen Geld gewinnen kann, oder "Bankrott", bei dem der Spieler sein gesamtes Guthaben verliert und ein neues Spiel beginnen muss.
* 
* Tier 3 (Application Server):
* In dieser Aufgabe wird kein Tier 3 erwähnt. Es handelt sich um ein Rätselspiel, bei dem der Spieler versucht Wörter oder Redewendungen zu erraten, indem er Buchstaben an der Rate-Wand ratet, um möglichst hohe Geldbeträge zu erhalten. Der Spieler dreht auch ein Glücksrad, um unterschiedliche Felder zu erhalten, die entweder Geldbeträge oder "Bankrott" enthalten und wenn der Spieler einen ungültigen Buchstaben ratet, verliert er Lebenspunkte.
* 
* Tier 4 (Dataserver):

# 2 Technologie

✍️ Um dieses Rätselspiel mit ASP.NET zu entwickeln, könnten wir eine Web-Anwendung erstellen, die die Benutzeroberfläche des Spiels enthält. Dazu könnten wir ASP.NET Core verwenden und das Model-View-Controller (MVC) Designmuster anwenden, um die Benutzersteuerung, die Datenverarbeitung und die Darstellung der Benutzeroberfläche voneinander zu trennen. Eine Datenbank wie SQL Server könnte verwendet werden, um die Rätsel-Phrasen oder -Wörter, die Kategorien und die Leistung des Spielers sowie den aktuellen Spiel-Status zu speichern. ASP.NET Identity könnte verwendet werden, um die Anmeldung und Verwaltung von Benutzerkonten zu handhaben.

# 3 Datenbank

✍️ Mit ASP.NET könnte die Datenbank mit Entity Framework gesteuert werden, einem Object-Relational-Mapping-Framework, das es ermöglicht, mit der Datenbank mittels C#-Code zu interagieren, anstatt SQL-Statements zu verwenden. Das Interface der Anwendung könnte mit ASP.NET Core und Razor Pages oder MVC erstellt werden, um eine benutzerfreundliche und ansprechende Benutzeroberfläche zu erstellen. Es könnten Formulare verwendet werden, um dem Benutzer die Möglichkeit zu geben, Buchstaben zu raten und das Glücksrad zu drehen, sowie Tabellen und Grafiken, um die aktuelle Spiel-Status und Leistung des Benutzers anzuzeigen.

# 4.1 User Stories

✍️ Formulieren Sie klare Anforderungen in der Form von User Stories (*„als … möchte ich … damit …“*) und zu jeder Anforderung mindestens einen dazugehörigen Testfall (in Kapitel 4.2). 

✍️ Formulieren Sie weitere, eigene Anforderungen und Testfälle, wie Sie Ihre Applikation erweitern möchten. Geben Sie diesen statt einer Nummer einen Buchstaben (`A`, `B`, etc.)

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |Funktional       | Muss | Als Administrator möchte ich mich über einen Benutzernamen und Passwort authentifizieren können, um Zugang zu den administrativen                                     |Funktionen der Anwendung zu erhalten.
| 2    |Funktional       |Muss  |Als Administrator möchte ich in der Lage sein, Phrasen und Rätselwörter hinzuzufügen, zu bearbeiten und zu löschen, um das Angebot des                                 |Spiels zu verwalten.                
| 3    |Funktional       |Muss  |Als Administrator möchte ich Kategorien erstellen und Wörter und Fragen diesen Kategorien zuordnen können, um das Rätseln zu                                           |erleichtern.                        
| 4    |Funktional       |Muss  |Als Administrator möchte ich einzelne Einträge in der Highscore-Liste löschen können, um unerwünschte oder ungültige Einträge zu                                       |entfernen.                          
| 5    |Funktional       |Muss  |Als Spieler möchte ich über einen Webbrowser auf die Benutzeroberfläche des Spiels zugreifen können, um das Rätseln zu starten.                                       |                                                      
| 6    |Funktional       |Muss  |Als Spieler möchte ich meinen Namen eingeben können, damit er in der Highscore-Liste angezeigt wird.                                                                   |                                    
| 7    |Funktional       |Muss  |Als Spieler möchte ich meinen aktuellen Kontostand und die verbleibenden Lebenspunkte jederzeit einsehen können, um meinen Fortschritt                                 |im Spiel zu verfolgen.              
| 8    |Funktional       |Muss  |Als Spieler möchte ich erfahren, ob meine Antwort richtig oder falsch war, um mein Rätselverständnis zu verbessern.                                                   |                                    
| 9    |Funktional       |Muss  |Als Spieler möchte ich die Highscore-Liste ansehen können, um zu sehen, wie gut ich im Vergleich zu anderen abschneide.                                                                                    
| 10   |Funktional       |Muss  |Als Spieler möchte ich die Möglichkeit haben, jederzeit zu spielen oder das Spiel zu beenden und meinen Gewinn in die Highscore-Liste                                 |zu übernehmen.                      
| 11   |Funktional       |Muss  |Als Entwickler möchte ich sicherstellen, dass kein Rätselwort oder keine Phrase einem Spieler mehr als einmal gestellt wird, um die                                    Herausforderung des Spiels aufrechtzuerhalten.
| 12   |Funktional       |Kann  |Als Entwickler möchte ich ein Transaktionsmanagement implementieren, um die Integrität der Daten in der Datenbank zu gewährleisten.


✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc. oder Zahl), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). 

# 4.2 Testfälle

| TC-№ | Vorbereitung                                         | Eingabe     | Erwartete Ausgabe 
| ---- | ------------                                         | -------     | ----------------- 
| 1.1  |Benutzername und Passwort vorhanden                   | Anmeldung mit gültigem Benutzernamen und Passwort| Erfolgreiche anmeldung |
| 2.1  |Fügen Sie eine Phrase oder ein Rätselwort hinzu       | Ein Wort    | rfolgreich hinzugefügt wurde und im Angebot des Spiels erscheint.    |
| 3.1  |Erstellen Sie eine Kategorie|Kategorei erstellen      |erfolgreich erstellt und verfügbarbar|
| 4.1  |Löschen Sie einen Eintrag aus der Highscore-Liste     | Löschen     | Erfolgreich gelöst und auf der Liste nicht auffindbar|
| 5.1  |Browser öffnen und URL Anwebndung eingeben            |Keine|die Benutzeroberfläche des Spiels wird geladen und ist in der Lage das Rätseln zu starten.|
| 6.1  | Als Spieler möchte ich meinen Namen eingeben können, |
        damit er in der Highscore-Liste angezeigt wird.       |Name eingeben|Name wird in der Highscore-Liste angezeigt|
| 7.1  | Geben Sie einen gültigen Benutzernamen und Passwort  |Spiel starten| Aktueller Kontostand und die verbleibenden Lebenspunkte auf der Benutzeroberfläche                                                                                     wird angezeigt.
| 8.1  |Geben Sie eine Antwort für ein Rätselwort |Wort eingeben|Die Anwendung zeigt die richtige oder falsche Antworten |
| 9.1  | Öffnen Sie die Highscore-Liste |öffnen| Alle Spalten (Name des Spielers, Zeitpunkt des Spiels, Geldbetrag, Anzahl der Spielrunden) werden korrekt angezeigt
| 10.1 |Spiel starten und Spielen | Spielen| Möglichkeit besteht, das Spiel jederzeit zu beenden und Ihren Gewinn in die Highscore-Liste zu übernehmen.
| 11.1 |Spielen Sie das Spiel mehrmals| Speil spielen|  keine Phrase oder Rätselwort werden doppelt gestellt.

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.

# 5 Prototyp

✍️![image](https://user-images.githubusercontent.com/69576108/212012176-4f927782-46db-475d-96da-0df073499b09.png)


# 6 Implementation

✍️ Halten Sie fest, wann Sie welche User Story bearbeitet haben

| User Story | Datum | Beschreibung |
| ---------- | ----- | ------------ |
| ...        |       |              |

# 7 Projektdokumentation

| US-№ | Erledigt? | Entsprechende Code-Dateien oder Erklärung |
| ---- | --------- | ----------------------------------------- |
| 1    | ja / nein |                                           |
| ...  |           |                                           |

# 8 Testprotokoll

✍️ Fügen Sie hier den Link zu dem Video ein, welches den Testdurchlauf dokumentiert.

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

# 9 `README.md`

✍️ Beschreiben Sie ausführlich in einer README.md, wie Ihre Applikation gestartet und ausgeführt wird. Legen Sie eine geeignete Möglichkeit (Skript, Export, …) bei, Ihre Datenbank wiederherzustellen.

# 10 Allgemeines

- [ ] Ich habe die Rechtschreibung überprüft
- [ ] Ich habe überprüft, dass die Nummerierung von Testfällen und User Stories übereinstimmen
- [ ] Ich habe alle mit ✍️ markierten Teile ersetzt
