# DNS Einträge

## Was sind DNS-Einträge?

Die einzelnen DNS-Einträge **beeinflussen den Betrieb der Domain-Dienste**. Sie bestimmen was angezeigt werden soll, wenn die Domain in die Adresszeile des **Browsers eingegeben** wird und legen fest wo Ihre E-Mails ankommen werden.

Durch das Anlegen oder die Löschung eines **A-Eintrags**, "schalten" Sie Ihre **Webseiten** online oder offline oder aktivieren eventuell eine **Domain der 3. Ebene** (Subdomain).

Jeder Eintrag kann auf einen anderen Dienstanbieter verweisen. Ihre Hauptseite kann z.B. unter der Internetadresse **domain.xy** laufen, während Ihr Onlineshop unter der Subdomain **eshop.domena.xy** läuft.

## Welche Arten von DNS Einträgen gibt es?

#### A-Records: <a href="#a-records" id="a-records"></a>

A-Records stehen für einen Hosteintrag z.B. www. und verweisen auf eine IP Adresse eines Servers z.B. Webserver.

**Beispiel:** Für die Domain deinedomain.com ist ein A-Record gesetzt, der auf die IP Adresse 77.244.243.2 zeigt.

#### AAAA: <a href="#aaaa" id="aaaa"></a>

AAAA steht für die gleiche Art von Eintrag wie für den „normalen“ „A“ Record, dieser Eintrag ist jedoch für die Verwendung von IPv6 Adressen vorgesehen. Bei Verwendung von IPv6 hat dieser Eintrag gegenüber dem normalen "A" Eintrag Priorität.

**Beispiel:** Für die Domain deinedomain.com ist ein AAAA-Record gesetzt, der auf die IPv6 Adresse f3b0:1:cb3a:b4b0:7872:5ef9:93bb:e7a2 zeigt.

#### CNAME: <a href="#cname" id="cname"></a>

Dieser DNS Eintrag wird eingesetzt, wenn statt einer IP-Adresse auf den Hostname verwiesen werden soll. CNAME Einträge können im Gegensatz zu ALIAS/ANAME Einträgen nur mit Subdomains verwendet werden.

**Beispiel:** Für die Subdomain test.deinedomain.com ist ein CNAME-Record gesetzt, der auf den Hostname www.deinedomain.com zeigt.

#### MX Record: <a href="#mx-record" id="mx-record"></a>

MX Records sind dafür zuständig einer Domain einen oder mehrere Mailserver mit Priorität (10, 20, 30 etc.) anzugeben. Der niedrigste Wert steht für den ersten zu verwendenden Mailserver.

**Beispiel:** Für die Domain deinedomain.com ist ein MX Eintrag gesetzt, der auf den easyname Mailserver mx01.easyname.eu zeigt.

#### NS-Records: <a href="#ns-records" id="ns-records"></a>

NS-Records werden verwendet, um Nameserver für eine Domain festzulegen

**Beispiel:** Für die Domain deinedomain.com ist ein NS Eintrag gesetzt, der auf den easyname Nameserver ns1.easyname.eu zeigt.

#### SRV-Records: <a href="#srv-records" id="srv-records"></a>

SRV-Records ermöglichen die Definition zur Verfügbarkeit von unter einer Domain angebotenen IP-basierter Dienste und werden für die Verwendung bestimmter Dienste und Anwendungen wie beispielsweise SIP/VoIP oder XMPP (Office 365, Jabber, Instant Messaging, etc) benötigt. Du kannst über einen SRV Eintrag bei uns auch den Port sowie das Protokoll angeben.

**Beispiel:** Für \_sip.\_tls.deinedomain.com ist ein SRV Eintrag gesetzt um den SIP Dienst zu verwenden mit dem TLS Protokoll. Dieser Eintrag zeigt auf den Hostname 443 sipdir.online.lync.com.

#### TXT-Records: <a href="#txt-records" id="txt-records"></a>

TXT-Records enthalten frei wählbaren Text. Auf einigen Systemen dient der Inhalt dazu, Verwaltungsdaten zu kodieren. TXT-Records werden auch benutzt um einen [SPF Eintrag](https://www.easyname.at/de/support/email/184-was-ist-spf-spamschutz) zu erstellen.

**Beispiel:** Für die Domain deinedomain.com ist ein TXT Eintrag gesetzt mit folgendem Inhalt: "v=spf1 include:spf.easyname.com -all"
