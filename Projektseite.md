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
  **Definitionen von Variablen:**
  
  
<h2 id="kapitel6">6. Der Farbsensor TCS3200</h2>
  
  
<h2 id="kapitel7">7. Reflexion und Fazit</h2>
  
  
<h2 id="kapitel8">8. Eigenständigkeitserklärung</h2>
  
  
