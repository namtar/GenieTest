# Readme

## Julia Stuff
Im Workspace erzeuge ein neues Projekt mit
* Aufruf Julia Repl -> julia
* mkdir("genie_test")
* cd("genie_test")
* pwd() <-- der Linux PWD Befehl
* readdir() <-- zeigt den Inhalt des Verzeichnisses an
* print(read("Project.toml", String)) <-- liest eine Datei aus dem Verzeichnis und gibt den Inhalt aus.


### Activate
TODO: Erkläre was Activate macht

### Package
Im Repl in den Package Mode wechseln Taste: ]
Package Mode mit Backspace verlassen
* generate GenieTest
    * erzeugt ein neues Projekt das GenieTest heißt
    * legt eine Project.toml an
    * legt im src Unterordner eine GenieTest.jl Datei an.

### Dependencies zu Projekt hinzufügen
* Im Repl in den Package Mode wechseln. 
* Wichtig. Im Package Mode muss man das Projekt aktivieren, damit die Dependencies dem Projekt und nicht zu Julia Global hinzugefügt werden. Das geht mit dem Befehl **activate**.
* Der Befehl **status** zeigt an was aktiviert ist
* Eine Dependencies wird mit **add** z.B. **add Genie** hinzugefügt.

> Dependency Management https://pkgdocs.julialang.org/v1/managing-packages/

### Naming Conventions
> https://docs.julialang.org/en/v1/manual/variables/

* Projects
    * Anscheinend muss man Projekte mit Xyz.jl benennen. VS-Code erkennt das dann automatisch als Julia Projekt. Im Fall von Github habe ich das Projekt wie auch andere Julia Projekte benamt. https://github.com/namtar/GenieTest.jl.git
* Packages
    * CamelCase
* Modules
    * CamelCase
* Types
    * CamelCase
* Variables
    * Lowercase
* Functions and Macros
    * Lowercase without underscore
    * Funktionen die ihre Parameter verändern müsssen ein ! am Ende haben


