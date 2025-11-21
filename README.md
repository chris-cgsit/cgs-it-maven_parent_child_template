# Maven Beispielstruktur Parent Child Template

Dieses Repository dient als zentrale Vorlage für einfache Projekte mit Parent Child Strutkru
Zum Beispiel für Übungen und Trainings 
Es verwendet Maven als Build-Tool und JUnit 5 für Tests.

## Struktur

*   `pom.xml`: Die zentrale Parent-POM-Datei. Hier sind globale Einstellungen (Java Version, JUnit Version) definiert.
*   `hello_world_dummy_module`: Ein Beispiel-Modul, das zeigt, wie ein Unterprojekt strukturiert ist.

## Starten eines neuen Projekts

Um eine neue Übung mittels maven sub-Modul zu starten, 
erstellen Sie einfach ein neues Maven-Modul in Ihrer IDE (IntelliJ, Eclipse):

1.  Klicken Sie in IntelliJ im Maven-Fenster auf das Plus-Zeichen (**+ Add Maven Project**) oder Rechtsklick auf den Root-Ordner im Projektbaum (**New** -> **Module**).
2.  Wählen Sie **Maven** aus.
3.  Geben Sie eine `ArtifactId` für Ihr neues Modul an (z.B. `java_03_schleifen`).
4.  Maven fügt das neue Modul automatisch zur Root-`pom.xml` hinzu.

## Testen

JUnit 5 ist bereits global im `dependencyManagement` konfiguriert. 
Sie können direkt Testabhängigkeiten in Ihren Submodulen hinzufügen (siehe `hello_world_dummy_module/pom.xml`).
