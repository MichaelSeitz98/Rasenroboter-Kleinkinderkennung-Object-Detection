## Erkennung von Kleinkindern bei Rasenmährobotern für mehr Sicherheit

Sie sind überall und nicht mehr wegzudenken aus Wohngebieten, Gartenanlagen, Fußballplätzen oder öffentlichen Rasenflächen - die Rasenmähroboter.
Im April 2020 testete Stiftung Warentest elf verschiedene Modelle und kommt zu einem besorgniseregendes Fazit: Die Sicherheit für Kleinkinder kann in keinem der getestete  Modelle gewährleistet werden. Kleinkinder, die sich auf dem Rasen befinden, werden durch die Roboter angefahren und im Fuß- und Armbereich verletzt. Alle  Robotermodelle haben zwar Sensoren verbaut, um Hindernisse zu erkennen, jedoch reagieren diese Sensoren im Fall von Kleinkindern erst nach einer gewissen Zeit bzw. einem gewissen Widerstand. In genau dieser Zeit können Verletzungen durch den Rasenmäher ausgelöst werden.

## Objekterkennung mit Tensorflow Object Detection API

Um diese Gefahr zu reduzieren, habe ich auf eine protoypische Objekterkennung entwickelt, die speziell Kleinkinder aus Perspektive des Rasenmährobotersobotors detektiert. Dafür habe ich verschiedene Modelle aus dem Tensorflow Modelzoo (https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md) verwendet und auf meinen Anwendungsanfall angepasst. Dafür habe ich die vier Modelle ausgewählt und auf den individuellen Anwendungsfall angepasst. 

<img src="./res/Vorauswahl_Modelle_Tensorflow_OD_API.png" width="620"/>


## Genauigkeit und Rechenzeiten


Bei den Rechenzeiten ergibt sich der folgende Vergleich
<img src="./res/Rechnenzeiten.png" width="620"/>

## Mobile Echtzeit-Anwendung unter Realbedingungen

Um einen möglichst realistischen Anwendung zu erhalten, habe ich das Modell in das TF-Lite Format exportiert. Dadurch lässt sich eine kamerabasierte Echtzeitanwendung erstellen, die einen Praxiseinsatz bei Rasenmähroboter realistisch simuliert.

<img src="./res/Einstellungsmöglichkeiten_und_Vollbild_App.png" width="620"/>
