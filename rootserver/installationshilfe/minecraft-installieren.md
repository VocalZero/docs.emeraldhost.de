# Minecraft installieren

1. Aktualisiere dein System und installiere notwendige Programme

```
apt update && upgrade -y
```

```
apt install screen default-jre
```

2. Lege einen Subuser für den Server an und melde dich an

```
adduser minecraft --disabled-login
```

```
su minecraft -l
```

3. Versionsauswahl (beispielsweise mit Spigot 1.19.3)
   * [Spigot Download](https://getbukkit.org/download/spigot)
   * &#x20;[Craftbukkit Download](https://getbukkit.org/download/craftbukkit)

```
wget https://download.getbukkit.org/spigot/spigot-1.19.3.jar
```

4. Startdatei erstellen

<pre><code>echo "screen -AmdS minecraft java -Xms1G -Xmx<a data-footnote-ref href="#user-content-fn-1">1</a>G -jar spigot-1.19.3.jar" > start.sh
</code></pre>

{% hint style="warning" %}
ändere bei -Xmx1G die 1 auf die anzahl deines Ram's z.B. 10 (Server mit 10 Gigabyte Ram)
{% endhint %}

5. Lizenzen aktzeptieren und dateirechte vergeben

```
echo "eula = true" > eula.txt
```

```
chmod +x start.sh
```

6. Server starten

```
./start.sh
```

{% hint style="info" %}
Die Console kann mit STRG + C geschlossen werden.
{% endhint %}

7. Wieder öffnen der Console

```
screen -r minecraft
```

[^1]: 
