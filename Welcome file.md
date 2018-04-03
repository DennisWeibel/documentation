---


---

<h1 id="dokumentation">Dokumentation</h1>
<h2 id="einleitung">Einleitung</h2>
<p>In diesem Modul geht es darum, eine Umgebung aufzubauen, bei der man VMs klonen kann und weitere Funktionen. Dabei müssen wir die Anweisungen eines Skripts befolgen.</p>
<h2 id="virtualbox">VirtualBox</h2>
<p>Um diese Umgebung aufbauen zu können muss man Virtuelle Maschinen erstellen können. Dazu verwende ich VirtualBox. Nach der Installation, musste ich noch die Funktionsfähigkeit testen. Um Das zu bewerkstelligen habe ich einen Ubuntu-Server aufgesetzt und so konnte ich sehen, dass alles korrekt lief.</p>
<h2 id="gitlab">GitLab</h2>
<p>Eine der Aufgaben, war etwas zu haben auf dem man seinen Code/Dokumentation hochladen kann. Hier kamen GitLab und GitHub in Frage. Ich habe mich für GitLab entschieden. Dazu habe ich den Test-Ubuntu Server genommen und auf ihm GitLab installiert. Ich habe folgende VM-Einstellungen verwendet:</p>
<ul>
<li>
<p>1 CPU</p>
</li>
<li>
<p>4 GB RAM</p>
</li>
<li>
<p>10 GB Harddisk</p>
</li>
<li>
<p>Netzwerk -&gt; NAT</p>
</li>
<li>
<p>Portweiterleitung -&gt; / Protokoll: TCP / Host-Port: 8080 / Gast-IP 127.0.0.1 / Gast-Port: 80</p>
</li>
</ul>
<p>Bei der Installation habe ich auf einen <a href="https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-gitlab-on-ubuntu-16-04">Guide</a> von DigitalOcean zurückgegriffen. Nachdem die Installation abgeschlossen war, konnte ich über 127.0.0.1:8080 auf GitLab zugreifen.</p>
<p>Benutzerdaten:</p>
<ul>
<li>
<p>Benutzername: root</p>
</li>
<li>
<p>Passwort: Sommer2017!</p>
</li>
</ul>
<h2 id="github">GitHub</h2>
<p>Weil GitLab nicht von Anfang an funktioniert hat, habe ich noch zusätzlich GitHub eingerichtet. Dort habe ich ein <a href="https://github.com/DennisWeibel">Konto</a> erstellt, mitsamt einer einfachen Ordner-Struktur. So kann ich nun Verzeichnisse erstellen und von dort aus committen.</p>
<p>GitHub und GitLab werden zur Versionierung verwendet.</p>
<h2 id="markdown">MarkDown</h2>
<p>Um dieses Modul zu dokumentieren, verwende ich MarkDown. Mit diesem Tool kann ich Text schreiben umso meine Fortschritte und Vorgehen festzuhalten. Ich habe MarkDown mit meinem GitHub verbunden und einem Repository zugewiesen. Das heisst meine Dokumentation ist in GitHub sichtbar.</p>
<h2 id="apache2">Apache2</h2>
<p>Eine weitere Aufgabe war, einen Apache-Server aufzusetzen, den man im späteren Verlauf verwenden muss. Dafür habe ich einen Ubuntu-Server mit den gleichen Spezifikationen, wie der GitLab-Server aufgesetzt. Anschliessend habe ich Apache2 installiert, dabei habe ich ein <a href="https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-ubuntu-16-04">Guide</a> von DigitalOcean verwendet.</p>
<h2 id="bash-und-git">Bash und Git</h2>
<p>Um weiter vorgehen zu können, war es nötig Bash + Git zu installieren. Mit den Angaben im Skript konnte ich es erfolgreich fertigstellen. Danach habe ich noch das Repository von GitHub Project geklont.</p>
<h2 id="vagrant">Vagrant</h2>
<p>Diese Anwendung wird für das automatisierte Erstellen vom VMs verwendet. Als erstes habe ich Vagrant heruntergeladen. Danach installierte ich Vagrant in Bash. -&gt; Anleitung Skript</p>
<p>Um Vagrant zu testen, musste ich einen Apache-Server automatisch aufsetzten. Ich gab die nötigen Befehle ein und der Apache-Server wurde automatisch erfolgreich erstellt.</p>
<h2 id="visual-studio-code">Visual Studio Code</h2>
<p>Eine weitere Komponente die Installiert werden musste war Visual Studio Code. Das wichtigste hierbei war, nach der Installation bei den Einstellungen noch einen Code reinzukopieren. Mit Visual Studio kann man die Konfiguration des Vagrantfiles ändern.</p>
<h2 id="linux">Linux</h2>
<p>Nun habe ich noch ein Linux Desktop installiert, über dem man später verschiedene Sachen durchführen kann.</p>
<p>Hardware Einstellungen:</p>
<ul>
<li>
<p>1 GB RAM</p>
</li>
<li>
<p>1 CPU</p>
</li>
<li>
<p>10 GB Speicher</p>
</li>
<li>
<p>Netzwerk -&gt; NAT</p>
</li>
</ul>
<h2 id="vagrant-file-abändern">Vagrant-File abändern</h2>
<p>Vagrant-File in Visual Studio Code öffnen.</p>
<p>Änderungen an SSH-File:</p>
<ul>
<li>Name des Servers -&gt; SHH_Srv</li>
<li>IP-Adresse -&gt; 192.168.0.15</li>
<li>Rechte der Benutzer -&gt; chmod 777</li>
<li>Name der Benutzer Gruppe -&gt; myadmins</li>
<li>Name der Benutzer -&gt; Dennis, Frank</li>
<li>Passwort der Benutzer -&gt; Sommer2017!</li>
<li>Einen 3ten Benutzer hinzugefügt -&gt; Thomas</li>
</ul>
<h2 id="testen">Testen</h2>

