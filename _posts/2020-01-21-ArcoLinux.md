---
layout: post
title: "Linux für die, die mehr Wissen wollen"
tags: [Linux]
---

Habt ihr schon etwas Erfahrung im Umgang mit Linux und wolltet mal etwas mehr dar&uuml; wissen wie ein Linux Betiebssystem eigentlich aufgebaut ist? Dann schaut euch mal Arco Linux an. Der Lernpfad dieser Distribution zeigt euch Schritt f&uuml;r Schritt, aus welchen Programmen ein Linux-Betriebssystem besteht und am Ende seid ihr sogar in der Lage eure eigene, auf Arch-Linux basierende Distribution zu bauen<!--more-->

## Was ist eigentlich ArcoLinux?
![ArcoLinux](/assets/img/blog/Jan2020/arcolinux-one-liner.jpg)<br>
Warscheinlich habt ihr noch nichts von dieser Distriution gehört, aber dennoch ist diese Distribution genial, wenn du mehr dra&uuml;ber wissen willst wie Linux funktioniert. Denn das gute an ArcoLinux ist, dass sich die Distro an Leute wendet, die mehr &uuml;ber Linux wissen wollen. In dieser Distribution gibt es nämlich einen eingebauten Lernpfad, der dir beibringt, deine eigene Distro zu bauen.Doch wie sieht der Lernpfad von ArcoLinux aus?<br>
Um hier schnell einen schnellen Überblick zu haben gibt es diese Übersicht, aber ich werde euch auch noch mal jeden Schritt etwas detaillierter und auf deutsch erkl&auml;ren.
![LearnigPath](/assets/img/blog/Jan2020/ArcoLinux-learning-path.png)<br><br>

## Phase 1: ArcoLinux installieren

In der ersten Phase installierst du erstmal die ganz "normale" ArcoLinux ISO, die du [hier](https://sourceforge.net/projects/arcolinux/files/ArcoLinux/) herunterladen kannst. Die Installation ist da (noch) ganz einfach und wie bei Ubuntu, denn man muss einfach nur das Live-Image mit einer Software wie [Etcher](https://www.balena.io/etcher/) auf den USB-Stick schreiben und diesen beim Booten im Bootmenu auswählen. Danach kann man das System mit dem Calamaris-Installer, der dem Installer, der bei Ubuntu benutzt wird, sehr &auml;hnlet, installieren.<br>
Und nach einem Neustart hat man schon ein voll funktionsfähiges, auf Arch-Linux basierendes System installiert. In dieser ISO von Arch-Linux sind desweitern drei verschiedene [Grafische Oberfl&auml;chen](https://linux-einsteiger-wiki.de/title/Grafische_Oberflächen) installiert:
<ul>
    <li><b>XFCE</b> f&uuml;r den kompletten Einstieg.</li>
    <li><b>OpenBox</b> f&uuml;r alle die einen etwas komplexeren Desktop ausprobieren wollen.</li>
    <li><b>i3</b>, der komplexeste, aber auch am besten anpassungsfähigste Desktop unter diesen drei. (Und nein, das ist kein Intel-Prozessor)</li>
</ul>
Diese Phase ist dazu da um erstmal, <b>komplett grundlegenden Umgang mit Linux</b> zu lernen. Aber damit man auch gleich mit dem Benutzen des Systems loslegen kann, haben die Entwickler von ArcoLinux gleich sehr viele Programme in das ISO gepackt. Also tobt euch hier aus und lernt Linux kennen. Einer der gr&ouml;&szlig;ten Unterschiede zu der normalerweise für Anf&auml;nger empfohlenen Distros ist zu Beginn der andere [Paket-Manager](https://linux-einsteiger-wiki.de/title/Paketverwaltungen) Pacman. Damit ihr euch damit zurechtfindet hier mal die grundlegende Syntax von Pacman:<br>
<b>sudo pacman</b>
<ul>
    <li><b>-S</b> zum Programme installieren</li>
    <li><b>-R</b> zum Programme deinstallieren</li>
    <li><b>-Ss</b> zum suchen von Paketen</li>
    <li><b>-Syu</b> zum installieren der neusten Updates</li>
</ul><br>
Also w&auml;re z.B. der Befehl um Audacity zu installieren:
```bash
    sudo pacman -S audacity
```
Wenn ihr eure Programme jedoch lieber &uuml;ber eine grafische Oberfläche installiert, steht euch dafür Pamac zur verf&uuml;gung. Alle Programme, die ihr mit Pacman im Terminal finden k&ouml;nnt, gibt es auch in Pamac.

## Phase 2: ArcoLinuxD mit XFCE, OpenBox und i3
Wenn ihr jetzt schon so etwas ge&uuml;bt im Umgang mit Linux seit, könnt ihr euch ArcoLinux heruterladen, das gibt's [hier](https://sourceforge.net/projects/arcolinux/files/ArcoLinuxD/). Der Unterschied zum "normalen" ArcoLinux ist, dass ArcoLinuxD nur ein ganz minimales System ist, ohne grafische Oberfl&auml;che. Also quasi so wie eine frische Installation von Arch-Linux. Allerdings ist die Installation dieses Grundsystems nicht so schwer wie bei Arch Linux, weil sie wieder &uuml;ber Calamaris erfolgt, wie bei Phase 1.<br>
Die Herausforderung besteht hier darin, sich seinen Desktop und alles n&ouml;tige selber zu installieren. Aber das ist auch nicht sonderlich schwer, da die Entwickler von ArcoLinux daf&uuml;r extra Skripte vorbereitet haben, um alles n&ouml;tige für den jeweiligen Desktop zu installieren. Ihr m&uuml;sst also nicht selber nach allen Paketen suchen. In der Phase 2 wird empfohlen erstmal die Desktops zu istallieren, die auch in Phase 1 zum Einsatz kamen, <b>XFCE, OpenBox und i3</b>.<br>
Die Skripte dafür gibt es auf der offiziellen [ArcoLinuxD-Website](https://arcolinuxd.com). Und hier w&auml;ren gleich die Tutorialseiten zu:
<ul>
    <li><a href="https://arcolinuxd.com/1-installation-of-arcolinuxd-xfce/">XFCE</a></li>
    <li><a href="https://arcolinuxd.com/1-installation-of-arcolinuxd-openbox/">OpenBox</a></li>
    <li><a href="https://arcolinuxd.com/1-installation-of-arcolinuxd-i3/">i3</a></li>
</ul>
Und hier zeigt sich die gro&szlig;e Stärke von ArcoLinux. Alles wird mit leicht verst&auml;ndlichen Tutorials erk&auml;rt und oft ist sogar ein Video dabei. Wenn man jetzt die drei grafischen Oberfl&auml;chen installiert hat, sollte das System ca. so aussehen wie die normale ArcoLinux-Installation aus Phase 1 aussehen. Nur mit dem Unterschied, dass ihr jetzt wisst welche Bestandteile ein Linux-Betriebssystem braucht, um zu funktionieren.

## Phase 3: ArcoLinuxD mit einer beliebigen grafischen Oberfl&auml;che
Wenn ihr jetzt mal eine andere grafische Oberfl&auml;che wie XFCE, OpenBox oder i3 nutzen wollt, dann kommt ihr in Phase 3 des Lernpfads von ArcoLinux an. Und keine Sorge, hier ist die Installation fast genauso einfach wie bei Phase 2. Sucht euch einfach auf der [ArcoLinuxD-Website](https://arcolinuxd.com) einen aus den insgesamt 12 verschiedenen Deskops aus, klone das jeweilige GitHub-Repository auf deinen PC und führe die entsprechenden Skripte aus. Zur Verf&uuml;gung stehen relativ bekannte Oberfl&auml;chen wie Gnome oder KDE Plasma, aber auch weniger bekannte, wie z.B. Herbstluftwm werden von den Entwicklern zur Verf&uuml;gung gestellt. Ob ihr hier die neuen Desktops auf eurem schon vorhandenem System aus Phase 2 installiet oder ob ihr nochmal mit einer frischen ArcoLinuxD-Istallation neustartet, bleibt ganz euch &uuml;berlassen.

## Phase 4: BYOI
In dieser Phase erstellt ihr eure erste eigene Linux ISO. Ihr bestimmt, welche Programme auf dem System landen und welcher Desktop standardm&auml;&szlig;ig genutzt wird. Auch das ist dank den vorgefertigten Skripten der ArcoLinux-Entwickler auch nicht sonderlich schwer. Hier sucht ihr einfach auf der [ArcoLinuxB-Website](https://arcolinuxb.com/category/byoi/arcolinuxb-iso/) nach der Oberf&auml;che eurer Wahl und klont das in dem Artikel angegebene Discord-Repository auf euren Rechner. In dem geklonten Repository befindet sich ein Ordner mit dem Namen "archiso" mit der Datei "packages.x86_64". Dort findet ihr eine Liste von Programmen. Ihr könnt einfach die Programme auskommentieren (ein "#" an den Anfang der jeweiligen Zeile). An den Programmen, die ihr haben wollt enfernt ihr entweder das "#" wenn schon eins da ist. Eigentlich ganz einfach. Die Programme, die ein "#" am Anfang der Zeile haben, werden nicht installiert, die ohne schon. Schreibt aber keine Programme, die &uuml;berhaupt nicht in der Liste stehen einfach dazu, das funktioniert leider nicht.<br>
Wenn ihr jetzt die Programme ausgew&auml;hlt habt, müsst ihr nur noch das "30-build-the-iso-the-first-time.sh" Skript aus dem Ordner "installation-scripts" aus und die ISO-Datei, wird mit den von euch ausgew&auml;hlten Programmen generiert. Wenn das auch geschafft ist, m&uuml;sst ihr nur noch das erzeugte Abbild, das sich in eurem Home-Verzeichnis in dem "ArcoLinuxB-Out" befindet, mit Etcher auf einen USB-Stick brennen. Jetzt k&ouml;nnt ihr dieses erstellte Image in eurem Bootmenu ausw&auml;hlen und booten. Und keine Sorge, wenn euch beim Starten vom USB-Stick die XFCE-Oberfl&auml;che angezeigt wird und nicht die, die ihr ausgew&auml;hlt habt. Das liegt daran, dass ArcoLinux immer den XFCE-Desktop nutzt um das Betriebssystem an euren Rechner "auszuliefern". Wenn ihr das System dann mit Calamares installiert habt, m&uuml;sst ihr nur noch euren PC neustarten und ihr werdet von eurem selber gebauten Betriebssystem mit der Oberfl&auml;che eurer Wahl begr&uuml;&szlig;t.

## Phase 5: Arch-Linux installieren
So, jetzt geht's langsam an's Eingemachte. In diesem Schritt wird n&auml;lich Arch-Linux komplett ohne zus&auml;zliche Skripte. Aber eins im Vorraus, ich habe schon selber oft Arch-Linux installiert und es ist echt nicht so schwer, wie viele behaupten. Folgt einfach dem Tutorial auf der Seite von ArcoLinux und es kann gar nicht viel schief gehen. Benutzt einfach:
<ul>
    <li><a href="https://arcolinuxd.com/5-the-actual-installation-of-arch-linux-phase-1-bios/">Dieses Tutorial,</a> wenn ihr noch ein <b>BIOS</b> habt</li>
    <li><a href="https://arcolinuxd.com/5-the-actual-installation-of-arch-linux-phase-1-uefi/">Dieses Tutorial,</a> wenn ihr schon <b>UEFI</b> habt</li>
</ul>
Ihr werdet sehen, mit dem Wissen aus den vorherigen Phasen und den Tutorials auf der Website, werdet ihr schon verstehen, was die Phylosophie hinter Arch-Linux ist.

## Phase 6: CARLI
Kommen wir nun zur letzen Phase. Und die ist so im Prinzip nocheimal die Phase 4, in der ja eine eigene ISO generiert wurde, nur mit dem Unterschied, dass wir hier keine Tools von ArcoLinux nutzen sondern auf "archiso" zur&uuml;ckgreifen. Ein Tool um selber bootbare Images von Arch-Linux zu erstellen. Das ganze wird von den Arco-Linux Entwicklern als "<b>C</b>ustomized <b>AR</b>ch <b>L</b>inux <b>I</b>so", also kurz <b>CARLI</b> bezeichnet.<br>
Klar, das ist etwas komplierter wie das "BYOI" aus Phase 4, aber dafür seid ihr durch "archiso" in der Lage, eure komplett eigene Arch-Linux-Distribution zu entwickeln. Wenn ihr damit anfangen wollt, startet am besten mit <a href="https://arcolinuxiso.com/1-installing-and-learning-about-archiso/">diesem Tutorial</a>.

## Zusammenfassung
Arco Linux ist meiner Meinung nach keine Distro, die nur aus der dem Betriebssystem besteht. Viel wichtiger als das Betriebssystem sind die Tutorials auf den ArcoLinux Websites. Desweiteren empfehle ich euch auch den <a href="https://discord.gg/R2amEEz">Discord-Server</a> oder die <a href="https://t.me/arcolinux_d_b">Telegram-Gruppe</a>. DIe Community dort ist sehr hilfbereit, wenn bei dem Lernpfad irgendwelche Probleme auftreten sollten.<br>
Der einzige Negatvpunkt ist meiner Meinung nach, dass die Tutorials nur auf Englisch verf&uuml;gbar sind. Wenn ich euch zu irgendeinem Schritt mal ein deutsches Tutorial machen soll, dann schreibt mir das ganz einfach als Kommentar unter den Ank&uuml;ndigungstweet dieses Artikels.
<blockquote class="twitter-tweet" data-lang="de"><p lang="de" dir="ltr">So habe den Artikel jetzt überarbeitet und er ist wieder online. Schaut vorbei<a href="https://t.co/dg46acn6L0">https://t.co/dg46acn6L0</a></p>&mdash; ニクラス (@NikurasuYT) <a href="https://twitter.com/NikurasuYT/status/1219756146854170624?ref_src=twsrc%5Etfw">21. Januar 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
