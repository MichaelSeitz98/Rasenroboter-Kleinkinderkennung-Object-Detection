### Erkennung von Kleinkindern bei Rasenmährobotern für mehr Sicherheit

Sie sind überall und nicht mehr wegzudenken aus Wohngebieten, Gartenanlagen, Fußballplätzen oder öffentlichen Rasenflächen - die Rasenmähroboter.
Im April 2020 testete Stiftung Warentest elf verschiedene Modelle und kommt zu einem besorgniseregendes Fazit: Die Sicherheit für Kleinkinder kann in keinem der getestete  Modelle gewährleistet werden. Keines der Geräte konnte eine bessere Note als 3,6 bezüglich der Sicherheit erzielen. Kleinkinder, die sich auf dem Rasen befinden,  werden durch die Roboter angefahren und im Fuß- und Armbereich verletzt. Alle  Robotermodelle haben zwar Sensoren verbaut, um 
Hindernisse zu erkennen, jedoch reagieren diese Sensoren im Fall von Kleinkindern erst nach einer gewissen Zeit bzw. einem gewissen Widerstand. In genau dieser Zeit können Verletzungen durch den Rasenmäher ausgelöst werden.

### Objekterkennung mit Tensorflow Object Detection API

Um diese Gefahr zu reduzieren, habe ich auf eine protoypische Objekterkennung entwickelt, die speziell Kleinkinder aus Perspektive des Rasenmährobotersobotors detektiert. Dafür habe ich verschiedene Modelle aus dem Tensorflow Modelzoo (https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md) verwendet und auf meinen Anwendungsanfall angepasst. Dafür habe ich verschiedene Modelle anhand ausgewählt. 

* EfficientDet D0
* EfficientDet D1
* Faster-R-CNN v1
* SSD MobileNet v2

### Mobile Echtzeit-Anwendung unter Realbedingungen für Android

<img src="./Einstellungsmöglichkeiten_und_Vollbild_App.png" width="620"/>
