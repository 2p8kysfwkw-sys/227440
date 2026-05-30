**Pumpenanalyse – Strömungsmaschinen Zusatzaufgabe 22744**

**Projektbeschreibung**
Dieses Repository beinhaltet die Auswertung von Betriebsdaten einer industriellen Wasserpumpe mit einem 264 mm Laufrad. Das Verhalten der Anlage wird sowohl technisch als auch wirtschaftlich betrachtet.

**Enthaltene Dateien**
* volume_flow_data.csv: Die rohen Messdaten der Sensoren (Volumenstrom und Zeitstempel).

* etaline-etlz-200-200-250-ggsav66d303004-bksbie3_ar12649.pdf: Das Datenblatt des Pumpenherstellers.

* 22744.ipynb: Das Jupyter Notebook, welches die vollständige Berechnung, Datenbereinigung und grafische Auswertung enthält.

**Methodik und Berechnungen**
Das Skript führt vollautomatisch folgende Schritte durch:

* Datenaufbereitung mit Glättung: Da die Sensordaten Schwankungen enthalten, wurde ein gleitender Mittelwert berechnet. Durch diesen werden die Daten geglättet und der Betriebstrend zur Visualisierung besser sichtbar gemacht.

* Technische Auswertung: Basierend auf der Herstellerkennlinie werden für jeden Messpunkt die Förderhöhe und der Wirkungsgrad ermittelt. Daraus berechnet sich die elektrische Leistungsaufnahme, die hydraulische Nutzleistung und schließlich die ungenutzte Verlustenergie in Kilowattstunden (kWh).

* Wirtschaftliche Auswertung: Um die Ineffizienz zu verdeutlichen, werden die Energiewerte mit einem angenommenen Industriestrompreis (0,18€ / kWh) multipliziert. So wird exakt aufgeschlüsselt, welche Kosten durch tatsächliche Nutzung und welche durch Verluste entstehen.

**Grafische Auswertung**
* Zur besseren Nachvollziehbarkeit generiert der Code verschiedene Diagramme, darunter:

* Volumenstrom-Verlauf: Gegenüberstellung der rohen Sensordaten und des geglätteten Trends.

* H-Q-Kennfeld: Abgleich der real gemessenen Betriebspunkte mit der theoretischen Herstellerkennlinie.

* Leistungsvergleich: Visualisierung von Stromaufnahme, Nutzleistung und den dazwischenliegenden Verlusten über den Tag.

* Kostenverlauf: Darstellung der stündlichen Stromkosten, unterteilt in Nutz- und Verlustkosten.

**Ausführung des Codes**
Der Code wurde für die Nutzung in Google Colab optimiert:

* Die Datei 22744.ipynb herunterladen oder direkt in Google Colab öffnen.

* Die beiliegende Datei volume_flow_data.csv in das Dateiverzeichnis des Notebooks hochladen.

* Die Code-Zellen im Notebook nacheinander von oben nach unten ausführen.
