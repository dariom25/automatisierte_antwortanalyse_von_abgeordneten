# Klassifikation von Antworten der Abgeordneten

In diesem Projekt analysiere und klassifiziere ich die Antworten von Abgeordneten mit Daten von Abgeordnetenwatch.de mittels Supervised Learning. Ziel ist es herauszufinden, ob es bestimmte Fragetopics gibt, die die Abgeordneten besonders ungerne beantworten. Dabei steht nicht das Ignorieren von Fragen im Fokus, sondern das Antworten nur auf einzelne Fragen oder das Schreiben einer Antwort, die die konkrete Frage, aber nicht beantwortet.

## Daten
Als Datengrundlage für die Analyse dient ein selbst gesammelter Datensatz von Fragen, Antworten und weiteren Informationen. Die Daten wurden mittels Webscraping von der Seite Abgeordnetenwatch.de gesammelt. Die Daten wurden am 05.08.2024 gesammelt und umfassen alle Fragen, Antworten usw. der zu diesem Zeitpunkt gewählten Abgeordneten auf Bundes-, Länder- und EU-Ebene. Der Datensatz umfässt einen Zeitraum von Dezember 2004 bis August 2024, wobei die Daten vor ca. 2019 vergleichsweise dünn sind, da nur ein Teil der im Jahr 2024 gewählten Abgeordneten schon in früheren Legislaturperioden gewählt waren. In dem, um fehlende Antworten bereinigten, Datensatz sind 46 614 Fragen enthalten.

### Parteien
### Topics
Die Zahl der Topics habe ich von 98 auf 13 reduziert. Der größte Teil der Reduktion fand im Bereich Wahlen statt. Hier habe ich die Fragen zu den einzelnen Wahlen pro Legislatur pro Parlament zu einem einzigen Topic zusammengefasst. Für eine genauere Aufschlüsselung, wie die einzelnen Topics zusammengefasst wurden, siehe [pipeline_classification.ipnyb](pipeline_classification.ipnyb). 

Für die Verteilung der Fragen und Antworten auf die einzelnen Topics siehe **Abbildung X**.


### parlamente

2282 sind per Hand klassifiziert

## Vorgehen

## Ergebnisse
