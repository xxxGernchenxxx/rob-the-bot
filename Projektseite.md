Diese Seite ist meine Projektseite. Hier stelle ich mein fertiges Projekt vor und ziehe ein Fazit.

<h2> Inhalt </h2>
<ul style="list-stlye-type:none">
<li><a href="#kapitell">1. Einleitung</a></li>
<li><a href="#kapitel2">2. Arduino und Sketch</a></li>
<li><a href="#kapitel3">3. Projektentwicklung</a></li>
<li><a href="#kapitel4">4. Vorstellung des Projekts</a></li>
<li><a href="#kapitel5">5. Der Sketch</a></li>
<li><a href="#kapitel6">6. Der Farbsensor TCS3200</a></li>
<li><a href="#kapitel7">7. Reflexion und Fazit</a></li>
<li><a href="#kapitel8">8. Eigenständigkeitserklärung</a></li>
<br>
<h2 id="kapitell">1. Einleitung</h2>
  Auch wenn es skuril erscheinen mag, gibt es viele Menschen, die die Unordnung in Schokolinsen-Verpackungen bezüglich der Farbe nervt. Dann könnte man sie natürlich mit der Hand sortieren, aber eine automatisierte Maschine wäre in dem Fall einfacher und bestimmt auch cooler. Mit einer solchen Maschine lassen sich dann auch im größeren Stile Schokolinsen sortieren, um sie zum Beispiel auf Feiern anzubieten.<br>
  
<h2 id="kapitel2">2. Arduino und Sketch</h2>
  Der Arduino ist eine Physical-Computing-Platform, die aus Hard- und Software besteht. Der Arduino besteht aus einer Platine, einem darauf montierten Mikrocontroller und verschiedenen Anschlüssen. So gibt es digitale und analoge Pins, die je nach Anwendung mit Lampen, Mikromotoren, Sensoren oder anderer Hardware verbunden werden können. Bei den digitalen Pins gibt es noch eine zusätzliche Unterscheidung in Pins, bei denen eine ständig gleichbleibende Spannung anliegt und in jene, die mit eine Welle (~) gekennzeichnet sind. Diese Welle steht für die Abkürzung PWM. Pulse Width Modulation (PWM) heißt, dass die am Pin anliegende Spannung geändert werden kann und dies vor allem für dimmbare LEDs bzw. RGB-LEDs nützlich ist. Zudem hat der Arduino noch eine USB-Schnittstelle und einen weiteren Anschluss, um Netzteile oder Batterien mit einem Adapter anstecken zu können. Falls bei einem Projekt die Stromversorgung über das USB-Kabel mit dem Computer nicht ausreicht, kann dieser Anschluss für eine weitere externe Stromquelle genutzt werden.
Mit den Pins lassen sich die genannten Verbraucher entweder direkt anschließen oder mittels eines E/A-Boards mit Widerständen versehen. Damit ist unter anderem eine bessere Übersichtlichkeit der angeschlossenen Module gegeben.<br>
  Von dem Arduino gibt es verschiedene Modelle. Bei diesem Projekt wurde ein Arduino R3 verwendet, der über fünf analoge und dreizehn digitale Pins verfügt. Zudem hat er wie jeder Mikrocontroller Minus-(GND) und Pluspole (3,5V / 5V). Neben diesen "Standardanschlüssen" gibt es noch einige weitere, die aber im Verlauf des Projektes nicht genutzt wurden.<br>
 
<h2 id="kapitel3">3. Projektentwicklung</h2>
  Nachdem das letzte Projekt abgeschlossen war, habe ich mir einige Gedanken gemacht, was ich als nächstes bauen bzw. programmieren möchte. Da kam mir zum einen ein Roboter in den Sinn, der auf Ketten oder Rädern selbst gesteuert fährt und Hindernisse mit Sensoren erkennt und umfahren kann. Bei diesem Roboter hätten sowohl verschiedene Motoren, als auch Sensoren zum Einsatz kommen können. Nach einiger Planung ist mir jedoch bewusst geworden, dass ein selbstfahrender Roboter eine Nummer zu groß ist. Deshalb habe ich im Internet nach Projektvorschlägen für den Arduino gesucht und eine Idee gefunden, die eine Sortiermaschine vorsieht. Diese Idee für Schokolinsen fand ich sofort sehr interessant und witzig in der Umsetzung. Doch auch hier habe ich mich nach einiger Planung auf eine etwas einfachere Umsetzung beschränkt, da meine eigene Weiterentwicklung der Idee zu einer Sortiermaschine für Legosteine wahrscheinliche große mechanische Schwierigkeiten gemacht hätte.<br>
  Auf diese Weise bin ich dann schlussendlich bei dem Vorschlag aus dem Internet für eine Sortiermaschine für Schokolinsen gelandet. Hierzu habe ich mir dann anschließend tiefergehende Planungen gemacht. Zum einen galt es einen passenden Farbsensor zu finden, aber auch einen geeigneten Aufbau zu entwerfen. Mit der Zeit bin ich von Ideen, die eine Förderband beinhalteten abgekommen und habe mich auf Ideen mit Rutschen beschränkt, die die Schwerkraft ausnutzen. Damit bin ich dann auch zu einem geplanten Aufbau gelangt, der folgendermaßen aussieht: 
  
  
  
  
  
<h2 id="kapitel4">4. Vorstellung des Projekts</h2>
  
  
<h2 id="kapitel5">5. Der Sketch</h2>
  Den Sketch habe ich selbst zusammengestellt. Den Teil, der für das Auslesen und Ansteuern des Farbsensors notwendig ist, habe ich aus dem Internet von einem YouTube-Video übernommen und den Rest habe ich mir selbst überlegt und aufgeschrieben. Das bedeutet, dass ich die Motorsteuerung und die Ansteuerung der LEDs in den Sketch selbst eingebunden habe genauso wie ich die if-Schleifen eigenstädnig entworfen habe. 
  Im Folgenden möchte ich den Sketch in den drei Teilen Definitionen von Variablen, Void Setup und Void Loop vorstellen:<br>
  Definitionen von Variablen:<br>
  
  ![Definitionen von Variablen](https://user-images.githubusercontent.com/88386279/163358696-6ab67091-155b-47dd-a396-9b1aa59da58f.PNG)
  
  In diesem Abschnitt habe ich die Variablen definiert. Das bedeutet ich habe den spezifischen Bezeichnungen besser verstädnliche Bezeichnungen verpasst oder sie erst definiert, damit in den späteren Schritten der Sketch überhaupt funktioniert. Hier kann man sehen, dass ich zu allererst die "Servo.h-Bibliothek" eingebunden habe und anschließend beide verwendeten Servo-Motoren benannt habe, damit ich zu jeder Zeit weiß, welcher Servo, wo sitzt und sich wann bewegt. Anschlißend habe ich die Pins des Farbsensors TCS32000 definiert und dann die RGB-Werte aus dem Kalibrierungs-Sketch für den Farbsensor übertragen. Anschließend habe ich noch weitere Variablen für den Farbsensor niedergeschrieben und abschließend die Pins für die drei LEDs definiert und benannt.<br>
  
  Void Setup:
  
  ![Void Setup](https://user-images.githubusercontent.com/88386279/163359887-777abc22-766a-4cce-ac20-da09e3c9398c.PNG)

  In diesem nächsten Abschnitt werden dann die Pins des Arduinos als Output oder Input versehen. Zudem wird eine Skalierung des Farbsensors vorgenommen und der Serial Monitor wird auf 9600 gesetzt. Das bedeutet, dass die Baudrate auf 9600 definiert wird und damit die Kommunikation zwischen dem Arduino und dem Serial Monitor ermöglicht wird. Im Prinzip dient dann der Serial Monitor, ein Fenster auf dem PC, als Anzeigeplattform für die vom Arduino gesammelten Informationen via Sensoren.
  Zudem habe ich im Void Setup noch die Steuerpins der Motoren und die Pins der LEDs als Output definiert.<br> 
  Im Gegensatz zur Void Loop wird das Void Setup nur einmal vom Arduino abgelesen. Das heißt, dass dieser die Anweisungen nur einmal befolgt und dann für die Schritte in der Loop immer umsetzt.<br>
  
  Void Loop:
  
  ![Void Loop 1](https://user-images.githubusercontent.com/88386279/163361416-96389016-bdd4-48c0-9da1-a93269d270cf.PNG)


  
<h2 id="kapitel6">6. Der Farbsensor TCS3200</h2>
  
  
<h2 id="kapitel7">7. Reflexion und Fazit</h2>
  
  
<h2 id="kapitel8">8. Eigenständigkeitserklärung</h2>
  
  
