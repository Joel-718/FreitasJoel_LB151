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

Um das Word Guesser-Spiel zu entwickeln, müssen verschiedene Technologien und Tools eingesetzt werden. JSF (JavaServer Faces) ist eine Java-Webanwendungs-Framework, die verwendet werden kann, um die Benutzeroberfläche des Spiels zu gestalten und zu verwalten. JSF bietet verschiedene Komponenten, mit denen Benutzeroberflächen erstellt werden können, z.B. Eingabefelder, Buttons, Labels und Dropdown-Listen. Mit JSF können Entwickler auch auf Ereignisse reagieren, die vom Benutzer ausgelöst werden, z.B. durch Klicken auf einen Button oder durch Eingabe von Text in ein Eingabefeld.

Eine weitere wichtige Technologie, die bei der Entwicklung des Word Guesser-Spiels eingesetzt werden kann, ist XAMPP. XAMPP ist ein kostenloses, plattformübergreifendes Tool, das eine komplette Entwicklungs- und Testumgebung für Webanwendungen bereitstellt. Es enthält Apache-Webserver, MySQL-Datenbank, PHP und Perl, die alle zur Erstellung von Webanwendungen erforderlich sind. Mit XAMPP können Entwickler eine lokale Umgebung einrichten, in der sie ihre Anwendung entwickeln, testen und debuggen können, bevor sie sie auf einem Live-Server bereitstellen.

In Bezug auf das Word Guesser-Spiel können JSF und XAMPP zusammen eingesetzt werden, um die Benutzeroberfläche zu gestalten und die Datenbank zu verwalten. Die Benutzeroberfläche kann mithilfe von JSF-Komponenten erstellt werden, z.B. Textfelder für die Eingabe von Buchstaben, Buttons zum Drehen des Glücksrads und Anzeigen von Hinweisen. Die Benutzeroberfläche kann auch dynamisch gestaltet werden, indem JSF verwendet wird, um Ereignisse zu verarbeiten, z.B. das Aktualisieren von Ergebnissen nach dem Drehen des Glücksrads.

Die Datenbank des Word Guesser-Spiels kann mit XAMPP verwaltet werden, indem MySQL verwendet wird, um die Spielergebnisse, Guthaben und die von den Spielern eingegebenen Buchstaben zu speichern. Die Datenbank kann auch verwendet werden, um Fragen und Kategorien zu speichern, die im Spiel verwendet werden können.

# 3 Datenbank

Um die Datenbank mit XAMPP und JSF zu steuern, muss zunächst eine Verbindung zwischen den beiden hergestellt werden. Dazu kann JDBC (Java Database Connectivity) verwendet werden, eine Java-API, die es ermöglicht, Datenbanken über Java-Anwendungen zu verwalten.

Sobald die Verbindung hergestellt ist, können verschiedene Operationen auf der Datenbank ausgeführt werden, z.B. das Abrufen von Daten, das Einfügen von Daten oder das Aktualisieren von Daten. In Bezug auf das Word Guesser-Spiel kann die Datenbank verwendet werden, um Spielergebnisse, Guthaben und eingegebene Buchstaben zu speichern. Die Datenbank kann auch dazu verwendet werden, Fragen und Kategorien zu speichern, die im Spiel verwendet werden.

Das Interface des Word Guesser-Spiels kann mithilfe von JSF erstellt werden. Die Benutzeroberfläche kann verschiedene Komponenten enthalten, wie z.B. Textfelder, Buttons, Labels und Dropdown-Listen. Diese Komponenten können verwendet werden, um den Spielern die Eingabe von Buchstaben, das Drehen des Glücksrads und das Anzeigen von Hinweisen zu ermöglichen.

Das Interface kann auch dynamisch gestaltet werden, indem Ereignisse verarbeitet werden, die vom Benutzer ausgelöst werden. Zum Beispiel kann JSF verwendet werden, um die Ergebnisse nach dem Drehen des Glücksrads automatisch zu aktualisieren oder dem Spieler eine Meldung anzuzeigen, wenn er einen ungültigen Buchstaben eingegeben hat.


# 4.1 User Stories

✍️ Formulieren Sie klare Anforderungen in der Form von User Stories (*„als … möchte ich … damit …“*) und zu jeder Anforderung mindestens einen dazugehörigen Testfall (in Kapitel 4.2). 

✍️ Formulieren Sie weitere, eigene Anforderungen und Testfälle, wie Sie Ihre Applikation erweitern möchten. Geben Sie diesen statt einer Nummer einen Buchstaben (`A`, `B`, etc.)

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |Funktional       | Muss | Als Administrator möchte ich mich über einen Benutzernamen und Passwort authentifizieren können, um Zugang zu den administrativen                                     |Funktionen der Anwendung zu erhalten.
| 2    |Funktional       |Muss  |Als Administrator möchte ich in der Lage sein, Phrasen und Rätselwörter hinzuzufügen, zu bearbeiten und zu löschen, um das Angebot des Spiels zu verwalten.|               
| 3    |Funktional       |Muss  |Als Administrator möchte ich Kategorien erstellen und Wörter und Fragen diesen Kategorien zuordnen können, um das Rätseln zu erleichtern.|                       
| 4    |Funktional       |Muss  |Als Administrator möchte ich einzelne Einträge in der Highscore-Liste löschen können, um unerwünschte oder ungültige Einträge zu entfernen.|                          
| 5    |Funktional       |Muss  |Als Spieler möchte ich über einen Webbrowser auf die Benutzeroberfläche des Spiels zugreifen können, um das Rätseln zu starten.|                                                                                         
| 6    |Funktional       |Muss  |Als Spieler möchte ich meinen Namen eingeben können, damit er in der Highscore-Liste angezeigt wird.|                                                                                                    
| 7    |Funktional       |Muss  |Als Spieler möchte ich meinen aktuellen Kontostand und die verbleibenden Lebenspunkte jederzeit einsehen können, um meinen Fortschritt im Spiel zu verfolgen.  |            
| 8    |Funktional       |Muss  |Als Spieler möchte ich erfahren, ob meine Antwort richtig oder falsch war, um mein Rätselverständnis zu verbessern. |                                
| 9    |Funktional       |Muss  |Als Spieler möchte ich die Highscore-Liste ansehen können, um zu sehen, wie gut ich im Vergleich zu anderen abschneide.|                                                                                  
| 10   |Funktional       |Muss  |Als Spieler möchte ich die Möglichkeit haben, jederzeit zu spielen oder das Spiel zu beenden und meinen Gewinn in die Highscore-Liste zu übernehmen.|                      
| 11   |Funktional       |Muss  |Als Entwickler möchte ich sicherstellen, dass kein Rätselwort oder keine Phrase einem Spieler mehr als einmal gestellt wird, um die Herausforderung des Spiels aufrechtzuerhalten.|
| 12   |Funktional       |Kann  |Als Entwickler möchte ich ein Transaktionsmanagement implementieren, um die Integrität der Daten in der Datenbank zu gewährleisten.|


✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc. oder Zahl), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). 

# 4.2 Testfälle

| TC-№ | Vorbereitung                                         | Eingabe     | Erwartete Ausgabe 
| ---- | ------------                                         | -------     | ----------------- 
| 1.1  |Benutzername und Passwort vorhanden                   | Anmeldung mit gültigem Benutzernamen und Passwort| Erfolgreiche Anmeldung, der Admin kann nun die Highscore liste und die Wörterliste bearbeiten
| 2.1  |Fügen Sie eine Phrase oder ein Rätselwort hinzu       | Ein x-beliebiges Wort| Wurde erfolgsreich hinzugefügt und erscheint per Zufall im Spiel|
| 3.1  |Erstellen Sie eine Kategorie|Kategorie erstellen      |Erfolgreich erstellt und wird, sobald das Wort dieser Kategorie erraten werden muss, erscheint die korrekte Kategorie|
| 4.1  |Löschen Sie einen Eintrag aus der Highscore-Liste     | Admin logt sich ein und löst ein Eintrag   | Erfolgreich gelöscht und auf der Liste nicht auffindbar|
| 5.1  |Browser öffnen und URL Anwendung eingeben            |Keine|die Benutzeroberfläche des Spiels wird geladen und ist in der Lage das Rätseln zu starten.|
| 6.1  | Als Spieler muss ich mein Name vor dem Spiel eingeben können, damit er in der Highscore-Liste angezeigt wird.|Name eingeben|Name wird in der Highscore-Liste angezeigt und wird beim Spiel mit dem richtigen Namen begrüsst|
| 7.1  | Der User muss vor dem Spiel sein Name eingeben |Spiel starten| Aktueller Kontostand und die verbleibenden Lebenspunkte auf der Benutzeroberfläche werden angezeigt.|
| 8.1  |Geben Sie eine Antwort für ein Rätselwort |Wort eingeben|Bei einer falschen Antwort geht dein Leben um eins runter, sobald es richtig ist, kommt eine Anzeige, dass du das Wort korrekt erraten hast und frag dich, ob du weiter spielen möchtest|
| 9.1  | Öffnen Sie die Highscore-Liste |Drücken Sie auf den Button "Highscore"| Alle Spalten (Name des Spielers, Zeitpunkt des Spiels, Geldbetrag, Anzahl der Spielrunden) werden korrekt angezeigt|
| 10.1 |Spiel starten und Spielen | Button drücken| Möglichkeit besteht, das Spiel jederzeit zu beenden und Ihren Gewinn in die Highscore-Liste zu übernehmen.|
| 11.1 |Spielen Sie das Spiel mehrmals| Spiel spielen|  keine Phrase oder Rätselwort werden doppelt gestellt.|


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
