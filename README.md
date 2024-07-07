# Logistic-Regression

**Anleitung zum ausführen des Notebooks:**
1. Klicken Sie auf das MyBinder Batch ↓
2. Warten Sie bis sich das Notebook geöffnet hat (bis zu 15min)
3. Das Notebook wird direkt aufgerufen und kann durch verwenden des Play-Button schrittweise ausgeführt werden

**Update:**
Ausführen in Google Colab ebenfalls möglich & performatnter:
1. Klicken Sie auf den Google Colab Batch ↓
2. Warten Sie bis sich das Notebook geöffnet hat (maximal 10sek)
3. Das Notebook wird direkt aufgerufen und kann durch verwenden des Play-Button schrittweise ausgeführt werden

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MichaelFranLu/Logistic-Regression/master?labpath=3-Logistische_Regression_Projekt-Loesung.ipynb)

<a target="_blank" href="https://colab.research.google.com/github/MichaelFranLu/Logistic-Regression/blob/main/3-Logistische_Regression_Projekt-Loesung.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>




**Dokumentation - Logistische Regression**

In dieser Aufgabe wird ein logistisches Regressionsmodell erstellt, um zu ermitteln, ob ein Anwender auf eine Werbung auf einer Internetseite geklickt hat oder nicht. Die Vorhersage stützt sich auf Anwenderinformationen, die in einer Datensammlung gespeichert sind. Diese Sammlung umfasst die folgenden Attribute:
- 'Daily Time Spent on Site': Zeit auf der Webseite in Minuten
- 'Age': Alter in Jahren
- 'Area Income': Durchschnittliches Einkommen der Region des Nutzers
- 'Daily Internet Usage': Durchschnittliche Minutenzahl die der Nutzer täglich im Internet ist
- 'Ad Topic Line': Überschrift der Werbung
- 'City': Stadt des Nutzers
- 'Male': Ob der Nutzer männlich ist (1) oder nicht (0)
- 'Country': Land des Nutzers
- 'Timestamp': Zeit zu der der Nutzer auf die Werbung geklickt oder das Fenster geschlossen hat
- 'Clicked on Ad': Ob der Nutzer gelickt hat (1) oder nicht (0)


**Benötigte Libraries instalieren**
- pandas
- numpy
- matplotlib
- seaborn

**Daten einlesen "ad_data.csv"**


**Explorative Datensanalyse**

In diesem Teil wird die explorative Datenanalyse unter Verwendung der Seaborn-Bibliothek ausgeführt. Es werden unterschiedliche Diagramme generiert, um Zusammenhänge und Muster zu entdecken:
- Grafik: Alter (Age): Verteilung der Altersgruppen
- Jointplot: Darstellung Beziehung "Area Income" mit "Age"
- Jointplot: Darstellung Beziehung "Daily Time Spent on Site" gegen "Age"
- Jointplot: Darstellung Beziehung "Daily Time Spent On Site" gegen "Daily Internet Usage"
- Pairplot: "Clicked on Ad" als Hue um die Aspekte des Plots basierend auf den Werten einer spezifischen Variable zu färben.


**Logistische Regression**

In diesem Teil werden die Daten in Trainings- und Testsets aufgeteilt, um das logistisches Regressionsmodell zu trainieren. Die ausgewählten Merkmale sind "Daily Time Spent on Site", "Age", "Area Income", "Daily Internet Usage" und "Male". Zielvariable ist "Clicked on Ad".
- Mit der Methode "train_test_split" werdem die Daten aufgeteilt.
- Erstellen eines logistisches Regressionsmodell und auf das Trainingssatz angepasst.

**Vorhersagen und Auswertung**

Das Hauptziel dieses Projekts besteht darin, ein Modell zu erstellen, das auf der Grundlage von Nutzereigenschaften vorhersagen kann, ob ein Benutzer auf eine Werbeanzeige klicken wird oder nicht. 
Der Klassifizierungsbericht am Ende gibt Aufschluss über die Effizienz des Modells.
