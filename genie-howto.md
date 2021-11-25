# Howto Genie
Cheatsheet zur Benutzung für Anfänger wie mich.

## Vorgehensweise

Zuerst will ich eine Genie App erzeugen, da wir via VSCode und nicht ständig via REPL arbeiten wollen. Außerdem möchte ich den Code in Gihub einchecken.

### Webservice
Wollte ich einen Webservice via Genie erzeugen würde ich den entsprechenden Genie Generator (auszuführen im Julia REPL) benutzen.

```julia
# Quelle: https://genieframework.github.io/Genie.jl/dev/tutorials/4--Developing_Web_Services.html
using Genie
Genie.newapp_webservice("MyGenieApp")
```
Dadurch wird eine entsprechende App Struktur erzeugt.
Den Server startet man über das entsprechende Script das sich im **bin** Ordner befindet. Es handelt sich dabei um ein Shellscript, welches ich auf dem Mac folgendermaßen starte.

```zsh
. ./server
```

In meinem Fall nutze ich den "." als [Source](https://ss64.com/bash/source.html) Operator damit der in dem **server** Script vorhandene Julia Befehl ausgeführt werden kann.

Das mache ich, da die Standard Shell auf dem Mac nicht mehr die Bash sondern ZSH ist. Damit ich dort den Julia Befehl ausführen kann habe ich die Julia App nicht der Path Variable hinzugefügt sondern einen Alias definiert.

**.zshrc**
```zsh
alias julia='/Applications/Julia-1.6.app/Contents/Resources/julia/bin/julia'
```

### MVC Web-Anwendung
Um eine Genie MVC Web-Anwendung zu erzeugen gibt es ebenfalls einen passenden Generator (auszuführen im Julia REPL).

```julia
# Quelle: https://genieframework.github.io/Genie.jl/dev/tutorials/4-1--Developing_MVC_Web_Apps.html
using Genie
Genie.newapp_mvc("GenieTest")
```

Bei der Gelegenheit wird auch gleich SearchLight mit eingerichtet und eine zu verwendende Datenbank abgefragt.




