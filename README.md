# Space Invaders 

Ziel dieser Übung ist es, ähnlich zu unserem Tetris einen Space Shooter in JavaFX zu programmieren. 
Im assets Ordner liegen einige Bilder und Töne die du verwenden kannst wenn du möchtest. 

Wie genau du das Spiel programmierst, ist dir überlassen, ein paar Schlüsselfunktionalitäten sollte es aber haben: 
* Das Spielfeld sollte 10 x 3 Dimensionen haben
* Zu Beginn des Spiels befindet sich der Spieler mittigs am unteren Spielfeldrand. 
* Mit den Tasten A und D kann sich der Spieler nach links bzw. rechts bewegen. 
* Zu Beginn des Spiels erscheint eine Armee von Space invaders (3 Zeilen á 10 Invaders) im oberen linken Eck des Spielfelds.
* Die Space Invaders bewegen sich von oben links nach rechts bis sie den Rand berühren, dann eine Zeile nach unten, dann nach links bis sie den Rand berühren dann eine Zeile nach unten und wieder nach rechts und so weiter
* Berührt ein Space Invader unseren Spieler ist das Spiel vorbei
* Mit einer beliebigen Taste (z.b. Space - bzw Ctrl+Space da JavaFX das Event sonst nicht aufnimmt) können laserstrahlen abgeschossen werden
* Ein laserstrahl bewegt sich von der Position des Spielers aus nach oben bis es entweder einen Alien oder den oberen Rand berührt
* Trifft ein Laserstrahl einen Space Invader so verschwindet dieser

## Nice to have 

* Verwende die beigelegten Grafiken zur Darstellung des Spielers bzw der Aliens 
* Bau die beigelegten Soundeffekte ein (Laser schuss, Alien movement, Game Over) 
```
AudioClip audioClip = new AudioClip(new File("my-sound.mp3").toURI().toString());
audioClip.play();
```
  Wenn du in JavaFX einen sound abspielen möchtest, musst du bei den VM arguments im "Edit Configuration" im IntelliJ ein weiteres Module hinzugefügt werden `--add-modules javafx.controls,javafx.fxml,javafx.media`
* Zeig einen coolen Game Over Screen an

## Recommendation 

Du darfst das Spiel natürlich implementieren wie du möchtest, könntest dich aber wenn dir kein Lösungsansatz einfällt an dem Tetris spiel orientieren. Dabei kannst du das Spielfeld wieder als TilePane darstellen und die Position der einzelnen Spielelemente (Spieler, Invader, Laser Strahl) mittels CSS Klassen steuern. 
