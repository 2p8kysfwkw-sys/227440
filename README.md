**Projekt: Pumpen-Performance-Analyse (22744)**

Dieses Repository enthält die automatisierte Auswertung der Betriebsdaten einer industriellen Wasserpumpe.
Im Rahmen der Zusatzaufgabe für das Modul "Strömungsmaschinen" wird das reale Betriebsverhalten einer Pumpe mit einem 269-mm-Laufrad technisch analysiert und wirtschaftlich bewertet.

**Aufgabenstellung**

Das Ziel dieses Projekts ist die Erstellung eines Jupyter Notebooks, das basierend auf bereitgestellten Sensordaten und dem Hersteller-Datenblatt folgende Analysen durchführt:
* Energieverbrauch: Berechnung der gesamten Leistungsaufnahme im betrachteten Zeitraum.  
* Effizienzbewertung: Ermittlung des durchschnittlichen Wirkungsgrades während des Pumpbetriebs.  
* Verlustanalyse: Quantifizierung der Energie, die im Betrieb nicht hydraulisch genutzt wurde (Verlustleistung).

**Repositorium-Struktur**

Das Projekt umfasst folgende Dateien zur Analyse:

* 22744.ipynb: Das Haupt-Notebook, welches die Datenbereinigung, die physikalischen Berechnungen sowie die grafische Auswertung bündelt.

* volume_flow_data.csv: Die CSV-Datei mit den zeitlich erfassten Volumenstrom-Messwerten des Sensors.  

* etaline-etlz-200-200-250-ggsav66d303004-bksbie3_ar12649.pdf: Das offizielle Datenblatt der Pumpe, welches die notwendigen Kennlinien für den Abgleich der Betriebspunkte bereitstellt.  

**Methodik**

Das Skript im Notebook vollzieht die Analyse in drei Schritten:

* Datenaufbereitung: Die Sensordaten des Volumenstroms werden eingelesen und für die weitere Verarbeitung vorbereitet.  

+ Physikalische Analyse: Abgleich der Betriebspunkte mit der Kennlinie des 269-mm-Laufrads. Bestimmung der Förderhöhe und hydraulischen Leistung.

* Auswertung: Berechnung der Energiebilanz und Identifikation von ineffizienten Betriebszuständen.

**Durchführung**

Das Skript wurde in Google Colab programmiert.
Um das Projekt auszuführen, folgen Sie diesen Schritten:

* Laden Sie das Notebook 22744.ipynb in Ihre bevorzugte Umgebung (z. B. Google Colab oder Jupyter Lab).

* Stellen Sie sicher, dass die Datei volume_flow_data.csv in das Dateiverzeichnis des Notebooks hochgeladen wurde.

* Führen Sie die Code-Zellen nacheinander aus. Die Grafiken und Ergebnisse werden automatisch generiert.
