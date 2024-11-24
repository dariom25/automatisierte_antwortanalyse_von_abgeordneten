# Klassifikation von Antworten der Abgeordneten

In diesem Projekt analysiere und klassifiziere ich die Antworten von Abgeordneten mit Daten von Abgeordnetenwatch.de mittels Supervised Learning. Ziel ist es herauszufinden, ob es bestimmte Fragetopics gibt, die die Abgeordneten besonders ungerne beantworten. Dabei steht nicht das Ignorieren von Fragen im Fokus, sondern das Antworten nur auf einzelne Fragen oder das Schreiben einer Antwort, die die konkrete Frage, aber nicht beantwortet.

## Daten
Als Datengrundlage für die Analyse dient ein selbst gesammelter Datensatz von Fragen, Antworten und weiteren Informationen. Die Daten wurden mittels Webscraping von der Seite Abgeordnetenwatch.de gesammelt. Die Daten wurden am 05.08.2024 gesammelt und umfassen alle Fragen, Antworten usw. der zu diesem Zeitpunkt gewählten Abgeordneten auf Bundes-, Länder- und EU-Ebene. Der Datensatz umfässt einen Zeitraum von Dezember 2004 bis August 2024, wobei die Daten vor ca. 2019 vergleichsweise dünn sind, da nur ein Teil der im Jahr 2024 gewählten Abgeordneten schon in früheren Legislaturperioden gewählt waren. In dem, um fehlende Antworten bereinigten, Datensatz sind 46614 Fragen enthalten.

### Parteien
![Balkendiagramm mit Zahl der Antworten nach Partei](images/bar_party_count.png)
Das Balkendiagram zeigt die Zahl der beantworteten Fragen nach Partei. Die SPD hat mit 13332 Fragen die meisten Fragen gestellt und beantwortet, gefolgt von Bündnis90/Die Grünen mit 10635 Fragen. Die wenigsten Fragen gestellt und beantworten haben die EU-Parteien Bürger in Wut und FAMILIEN-PARTEI. Bei den Parteien ist zu beachten, dass einige nur auf EU-Ebene antreten und knapp zwei Monate bevor die Daten erhoben wurden die Europawahl 2024 durchgeführt wurde. Daher sind für diese Parteien die Zahlen der beantworteten Fragen sehr niedrig. Auf der anderen Seite ist auch zu sehen, dass die Regierungsparteien mit deutlichem Abstand am Meisten Fragen auf Abgeordnetenwatch.de erhalten und beantwortet haben.

### Topics
Die Zahl der Topics habe ich von 98 auf 13 reduziert. Der größte Teil der Reduktion fand im Bereich Wahlen statt. Hier habe ich die Fragen zu den einzelnen Wahlen pro Legislatur pro Parlament zu einem einzigen Topic zusammengefasst. Für eine genauere Aufschlüsselung, wie die einzelnen Topics zusammengefasst wurden, siehe [exploratory_data_analysis.ipynb](exploratory_data_analysis.ipynb). 

![Balkendiagramm mit Zahl der Antworten nach Topics](images/bar_topic_count.png)
Das Balkendiagramm zeigt die Zahl der beantworteten Fragen nach Topics. Am häufigsten wurden Fragen zu den Topics "Politik und Parteien" mit 7095 Fragen und "Energie und Umwelt" mit 6773 Fragen gestellt und beantwortet. Die wenigsten Fragen wurden zu den Topics "Bildungs und Forschung" mit 860 Fragen und "Sport, Kultur, Tourismus" mit 424 Fragen gestellt und beantwortet.

### Parlamente
Die Zahl der Legislaturperioden der Parlamente habe ich auf die Bundes-, Landes- und EU-Parlamente reduziert, so dass nur noch 18 Parlamente existieren. Für einen genaueren Überblick siehe: [exploratory_data_analysis.ipynb](exploratory_data_analysis.ipynb)

![Balkendiagramm mit Zahl der Antworten nach Parlament](images/bar_parliament_count.png)
Das Balkendiagramm zeigt die Zahl beantworteten Fragen nach Parlamenten. Mit weitem Abstand die meisten Fragen wurden im Bundestag gestellt und beantwortet mit 40255 Fragen, gefolgt von Hamburg mit 884 Fragen. Die wenigsten Fragen wurden in Bremen mit 83 Fragen und Mecklenburg-Vorpommern mit 72 Fragen gestellt und beantwortet.

2282 sind per Hand klassifiziert

## Vorgehen

## Ergebnisse
