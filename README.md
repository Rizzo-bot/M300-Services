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
`vagrant init ubuntu/xenial64` erzeugt das VagrantFile in ausgewähltem Verzeichnis\
`vagrant up` VM erstellen und starten\
`vagrant box` Commands to manage system boxes\
`vagrant destroy` Destroy the environment, deleting the created virtual machines\
`vagrant halt` Halt the running VMs in the environment\
`vagrant help [TASK]` Describe available tasks or one specific task\
`vagrant init [box_name]` Initializes the current folder for Vagrant usage\
`vagrant package` Package a Vagrant environment for distribution\
`vagrant provision` Rerun the provisioning scripts on a running VM\
`vagrant reload` Reload the environment, halting it then restarting it.\
`vagrant resume` Resume a suspended Vagrant environment.\
`vagrant ssh` SSH into the currently running Vagrant environment.\
`vagrant ssh_config` outputs ssh config valid syntax for connecting to this environment via ssh\
`vagrant suspend` Suspend a running Vagrant environment.\
`vagrant version` Prints the Vagrant version information\

Nachdem die Vagrant-VM gestartet wurde muss man sich per Git-Bash darauf anmelden mit folgendem Befehl: `vagrant ssh`.

![vagrant-ssh](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-ssh.PNG)

### Meine Infrastruktur 
So sieht meine Infrastruktur aus:

![Infrastruktur](https://github.com/Rizzo-bot/M300-Services/blob/main/Infrastruktur.PNG)

### Firewall eingerichtet insklusive Rules
In diesem Schritt wird eine lokale Firewall installiert und ebenfalls den Port 22. So kann man eine SSH-Verbindung herstellen.

![Vagrant-firewall](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-rule1.PNG)

### Reverse Proxy eingerichtet

Mit den folgenden Schritten habe ich den Reverse-Proxy aktiviert:

![Vagrant-rev1](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-rev1.PNG)

![Vagrant-rev2](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-rev2.PNG)

![Vagrant-rev3](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-rev3.PNG)

### Benutzer und Rechtevergabe ist eingerichtet

Hier habe ich jeweils zwei Users "Admin" und "Test" erstellt mit den entsprechenden Berechtigungen.

![Vagrant-rev3](https://github.com/Rizzo-bot/M300-Services/blob/main/vagrant-users.PNG)

### Persönliche Lernentwicklung: Vergleich Vorwissen - Wissenszuwachs

Im Vergleich zu jetzt habe ich vieles über Vagrant, Visual Studio Code und auch Virtualbox gelernt. Vorher konnte ich nur sagen was diese Programme sind, jedoch kann ich jetzt auch mit meinem neu erlerntem. Ich konnte eine VM mithilfe mit einem Vagrant-File erzeugen und so weiter. Jedoch fand ich es wirklich kompliziert von Visual Studio Code aus mit Hilfe von Markdown in die Dokumentation zu schreiben. Der erste Teil vom Modul war für mich eher anstrengend und auch recht frustrierend.

### Persönliche Lernentwicklung: Reflexion
Im erstem Teil des Moduls war es ziemlich ansztrengend für mich ich habe meistens Probleme mit dem Verstehen der Mechanismen, jedoch konnte ich dannach mithilfe verschiedener Leute einen besseren Einblick bekommen. Es gab Tage an dem ich gut für das Modul arbeiten konnte und einige Tage an denen ich schlechter daran arbeiten konnte. Leider konnte ich nicht sonderlich viel für die LB01 machen.
