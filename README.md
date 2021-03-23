# M300-Services

### Wissenstand pre-Modul
Ich habe keine Ahnung was Vagrant ist, weder die verschiedenen Funktionen von GitHub, noch was IaC ist etc. Vorwissen bereits über SSH, Ubuntu, VSC.

### Neu erlerntes
In dieser Dokumentation, werden jenste Begriffe, Prozesse beschrieben, wo von ich noch keine Ahnung hatte und interessant waren. Ebenso wird dokumentiert, was ich in diesem Modul gemacht habe, welche auf das Raster LB01 basieren.

## 10 Toolumgebung aufsetzen
### GitHub und GitBash
Wichtige Befehle:\
`git config --global user.name "username" | Standard Benutzername`\
`git config --global user.email "E-Mail" | Standard E-Mail Adresse`\
`git clone "URL vom Repository" | Repository klonen`\
`git pull | Repository auf aktuellem Stand beziehen`\
`git status | Status des Repositories abfragen`\
`git add - A "Filename" | Datei dem Repository hinzufügen`\
`git commit -m Kommentar (falls gewünscht) | Kommentar zu den Änderungen`\
`git push | Änderungen übernehmen`\

### Virtualbox
Virtualbox ist eine Software um seine virtuellen Maschinen zu verwalten und steuern.

Nach Anleitung wurden die virtuellen Maschinen erstellt. Meine Virtualbox sieht folgt aus:

![Virtualbox](https://github.com/Rizzo-bot/M300-Services/blob/main/Virtualbox-menu.PNG)

### Visualstudio Code
Visualstudio Code ist eine Software um verschiedene Codierungen zu schreiben. verschiedene Erweiterungen können ebenfalls heruntergeladen werden. Es ist auch bekannt als ein Quelltext-Editor. Es hat auch Funktionen wie Debugging, Autovervollständigung etc.

Folgend kommen wie angegeben die Konfigurationen für Visualstudiocode:

![Visualstudiocode1](https://github.com/Rizzo-bot/M300-Services/blob/main/visualstudiocode-1.PNG)

Filesexclude:

![Visualstudiocode2](https://github.com/Rizzo-bot/M300-Services/blob/main/visualstudiocode-filesexclude.PNG)

installierte Erweiterungen:

![Visualstudiocode3](https://github.com/Rizzo-bot/M300-Services/blob/main/visualstudiocode-installed.PNG)

### Vagrant
Mit Vagrant kann man Vm's schneller installieren und den langen Prozess überspringen.

Wichtige Befehle:\
`cd` choose Direcotry, wählt den Standort des Verzeichnisses aus.
`mkdir` erstellt einen Ordner\
`vagrant init ubuntu/xenial64` erzeigt das VagrantFile in ausgewähltem Verzeichnis\
`vagrant up` VM erstellen und starten\

Nachdem die Vagrant-VM gestartet wurde muss man sich per Git-Bash darauf anmelden mit folgendem Befehl: `vagrant ssh`.

![vagrant-ssh](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-ssh.PNG)

### Meine Infrastruktur 
So sieht meine Infrastruktur aus:

![Infrastruktur](https://github.com/Rizzo-bot/M300-Services/blob/main/Infrastruktur.PNG)


