---
layout: post
title: "FerenOS, das neue ZorinOS?"
tags: [Linux, Ersteindruck]
bootstrap: true
excerpt_separator: <!--more-->
---

Heute hab ich mir gedacht, dass ich mal ein Review zu einem Linux machen könnte, was ich schon seit längerer Zeit verfolge, [FerenOS](https://ferenos.weebly.com/).
Bei diesem Linux handelt es sich um eine Distribution die auf Linux Mint und Debian aufbaut. Zus&auml;tzlich handelt es sich sogar um eine [Rolling-Release](https://linux-einsteiger-wiki.de/title/Rolling_Distros)-Distribution, also ein echter Exot in der Debian/Ubuntu-Welt. <!--more-->

## Leicht zu installieren
Wie sehr viele Distributionen, die auf Ubuntu basieren, bringt auch diese Distribution einen grafischen Installer mit. Für Windows-Benutzer gibt es sogar ein Übertragungs-Tool mit dem man seine Daten wie Bilder, Dokumente, Musik, etc. sichern kann und auf Feren OS in den richtigen Ordnern wiederherstellen kann. Dieses ruft man von dem USB-Stick mit dem man das live Image von FerenOS startet. Im Tool wählt man die Platte aus, auf der Windows installiert ist und das Tool sichert automatisch die Ordner Dokumente, Bilder, Musik, etc. Sogar das aktuelle Hintergrundbild kann mit diesem Tool übernommen werden. Wenn man jedoch einen bestimmten Ordner nicht in FerenOS übernehmen will kann man einfach das entsprechende Kreuzchen entfernen. Nach der Installation kann man dann die gesicherten Daten mit demselbern Tool wiederherstellen. Auch hier kann man erneut auswählen, welche Ordner man in seinem Linux haben will.
![FerenOS Backup-Tool](/assets/img/blog/Jan2020/FerenBackup.png)<br>

## Das Windows unter Linux?
Also was den Übergang von Windows zu Linux angeht, scheint FerenOS dem bisherigen Topkandidaten für den Posten Windows-Klon ZorinOS den Rang abzulaufen. Denn nach dem Booten des live Images wurden mir gleich verschiedene Themes angeboten, die an die bekanntesten Betriebssysteme erinnern sollen. Aber die Entwickler haben sich am meisten Mühe dabei gegeben freundlich zu Windows Nutzern zu sein, denn hier gibt es gleich 2 Themes, Familiar und Redmond. Hier mal die Themes im Überblick:
<div id="demo" class="carousel slide" data-ride="carousel">

  <!-- Indicators -->
  <ul class="carousel-indicators">
    <li data-target="#demo" data-slide-to="0" class="active"></li>
    <li data-target="#demo" data-slide-to="1"></li>
    <li data-target="#demo" data-slide-to="2"></li>
    <li data-target="#demo" data-slide-to="3"></li>
    <li data-target="#demo" data-slide-to="4"></li>
    <li data-target="#demo" data-slide-to="5"></li>
    <li data-target="#demo" data-slide-to="6"></li>
    <li data-target="#demo" data-slide-to="7"></li>
  </ul>

  <!-- The slideshow -->
  <div class="carousel-inner">
    <div class="carousel-item active">
        <img src="/assets/img/blog/Jan2020/FerenDark.png" alt="FerenDark">
        <div class="carousel-caption">
            <p>Feren Dark</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenLight.png" alt="Feren Light">
        <div class="carousel-caption">
            <p>Feren Light</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenStandart.png" alt="Feren Standard">
        <div class="carousel-caption">
            <p>Standard</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenBrezzeDark.png" alt="BreezeDark">
        <div class="carousel-caption">
            <p>Breeze Dark</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenCupertino.png" alt="Cupertino">
        <div class="carousel-caption">
            <p>Cupertino</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenFamilar.png" alt="Familiar">
        <div class="carousel-caption">
            <p>Familiar</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenRedmond.png" alt="Redmond">
        <div class="carousel-caption">
            <p>Redmond</p>
        </div>
    </div>
    <div class="carousel-item">
        <img src="/assets/img/blog/Jan2020/FerenUnity02.png" alt="Unity">
        <div class="carousel-caption">
            <p>Unity</p>
        </div>
    </div>
  </div>

  <!-- Left and right controls -->
  <a class="carousel-control-prev" href="#demo" data-slide="prev">
    <i class="fa fa-caret-left" aria-hidden="true" style="font-size:50pt; color:black"></i>
  </a>
  <a class="carousel-control-next" href="#demo" data-slide="next">
    <i class="fa fa-caret-right" aria-hidden="true" style="font-size:50pt; color:black"></i>
  </a>

</div>
Ich finde es schon &auml;u&szlig;erst erstaunlich, wie gut, das Team von FerenOS es geschafft hat, die Live-Kacheln von Microsoft mit dem Familiar Theme zu kopieren. Wenn man dann noch ganz genau hinschaut sieht man auch, dass das Uhren-Layout unten rechts nahezu perfekt adptiert wurde und sogar die kleine rechteckige Fläche zum umschalten auf den Desktop ist vorhanden. Ich mag diese Detailverliebtheit, die man hier spürt.Es gibt meiner Meinung nach zur Zeit kein Linux, dass mehr nach unserem alten Bekannten aus Redmond aussieht.
Aber kommen wir nun mal zur Software, die Feren gleich zu Beginn mitbringt. Als Medienspieler ist VLC am Start und auch die altbekannte Bürosoftware LibreOffice ist in FerenOS gleich entahlten. Aber zu meiner Verwunderung kommt als Dateimanager nicht etwa Dolphin, der Standart Dateimanager des KDE Desktops zum Einsatz, sondern Nemo aus Cinnamon. Hier merkt man noch die Würzeln der Linux Distribution, den früher basierte FerenOS komplett auf Cinnamon. Es gibt aber auch noch eine Lite-Version von FerenOS die nach wie vor auf Cinnamon basiert. Um das installieren von verschiedenen Browsern zu vereinfachen, haben die Entwickler von FerenOS übrigens den Web Browser-Manager von ZorinOS einfach &uuml;bernommen. Der vorinstallierte Standard-Browser ist übrigens Vivaldi. Um das Thema noch genauer an seine Bedürfnisse anpassen zu können wurde der Kwantum-Manager implementiert. Timeshift für mögliche System-Backups ist auch gleich dabei. Sonst gibt es noch die KDE-typischen Tools wie KDE-Connect, Okular, die KDE-Einstellungen und so weiter.
Wer neue Software installieren will, dem steht neben einem Store in Form einer Eigenentwickung von FerenOS auch noch der Synaptic-Package-Manager zur Verfügung.

## Fazit
<br>
Wie die Entwicklung des neuen FerenOS-Updates wohl abgelaufen ist:
> Wie viel von Windows willst du kopieren?<br>
> JA!

Ich bin zwar nicht ganz so Fan von dem allgemeinem Aufbau von Windows, aber gerade weil das so gut umgesetzt wurde, dass es f&uuml;r mich fast schon nervig ist, ist Feren OS meiner Meinung nach zur Zeit die Distribution für alteingesessene Windows Benutzer, die auch mal Linux ausprobieren wollen. Einen gewaltgen Vorteil gegenüber Windows, der vielleicht den einen oder anderen &Uuml;berzeugen könnte w&auml;re, dass FerenOS im Idle nur eine RAM-Auslastung von knapp 800MB hat. Hier sieht man die gewaltige Verbesserung der Performance, die aber zugegebenerma&szlig;en aus dem Hause KDE kommt. 