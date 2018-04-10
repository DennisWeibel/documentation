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
<p>Um weiter vorgehen zu können, war es nötig Bash + Git zu installieren. Mit den Angaben im Skript konnte ich es erfolgreich fertigstellen. Danach habe ich noch das Repository von GitHub Project geklont. So kann ich nun</p>
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
<h2 id="firewall--apache-anpassen">Firewall &amp; Apache anpassen</h2>
<p>Ich habe ausserdem noch mit Visual Studio Code die Default Page von Apache2 verändern können und noch automatisch eine Firewall hinzufügen können.<br>
Code:<br>
<img src="https://perrone.myqnapcloud.com:450/share.cgi/apachecode.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=apachecode.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></p>
<p><img src="https://perrone.myqnapcloud.com:450/share.cgi/apachecode1.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=apachecode1.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></p>
<h2 id="testen">Testen</h2>
<h3 id="vagrant-1">Vagrant</h3>
<ul>
<li>Zweck: 		                      	Virtelle Maschinen erzeugen</li>
<li>Erwartetes Resultat: 			VM wird erstellt</li>
<li>Tatächliches Resultat:		VM’s wurden erfolgreich erstellt</li>
<li>Bildbeweis<br>
<img src="https://perrone.myqnapcloud.com:450/share.cgi/Vagrant.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=Vagrant.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></li>
</ul>
<h3 id="github--gitlab">Github &amp; Gitlab</h3>
<ul>
<li>Zweck:									Funktionalität testen</li>
<li>Erwartetes Resultat:			Man kann sich einloggen und Verzeichnisse erstellen</li>
<li>Tatsächliches Resultat:		Das Login Funktioniert und man kann Github/Gitlab nach belieben verwenden.</li>
<li>Bildbeweis:<br>
<img src="https://perrone.myqnapcloud.com:450/share.cgi/Github.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=Github.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></li>
</ul>
<h3 id="bash--git">Bash &amp; Git</h3>
<ul>
<li>Zweck:								Bash und Git funktionieren</li>
<li>Erwartetes Resultat:			Befehle die man eingibt werden ausgeführt</li>
<li>Tatsächliches Resultat:		Repository können geklont werden</li>
<li>Bildbeweis:<br>
<img src="https://perrone.myqnapcloud.com:450/share.cgi/gitbash.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=gitbash.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></li>
</ul>
<h3 id="visual-studio-code-1">Visual Studio Code</h3>
<ul>
<li>Zweck:								Mit VS Code VM verändern die automatisch erzeugt wird</li>
<li>Erwartetes Resultat:			Die Maschine wird mit den Änderungen erstellt</li>
<li>Tatsächliches Resultat:		Die Änderungen sind in der VM zu sehen</li>
<li>Bildbeweis:<br>
<img src="https://perrone.myqnapcloud.com:450/share.cgi/VM_Modifiziert.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=VM_Modifiziert.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></li>
</ul>
<h3 id="firewall">Firewall</h3>
<ul>
<li>Zweck: Kann man sich mit ssh verbinden?</li>
<li>Erwartetes Ergebnis: Verbindung ist möglich</li>
<li>Tatsächliches Resultat: Man kann sich per ssh auf die VM verbinden</li>
<li>Bildbeweis:<br>
<img src="https://perrone.myqnapcloud.com:450/share.cgi/firewall.PNG?ssid=02YbC2K&amp;fid=02YbC2K&amp;path=/&amp;filename=firewall.PNG&amp;openfolder=normal&amp;ep=" alt="enter image description here"></li>
</ul>

