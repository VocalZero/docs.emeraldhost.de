# Minecraft installieren

1. Aktualisiere dein System und installiere notwendige Programme

```
apt update && upgrade -y
```

<details>

<summary>Debian 10</summary>

```
apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 73C3DB2A
```

```
echo "deb http://ppa.launchpad.net/linuxuprising/java/ubuntu focal main" | tee /etc/apt/sources.list.d/java.list
```

```
apt update
```

```
apt install oracle-java17-installer -y
```

</details>

<details>

<summary>Debian 11</summary>

```
apt install screen openjdk-17-jre-headless -y 
```

</details>

<details>

<summary>Ubuntu</summary>

```
apt install software-properties-common -y
```

```
add-apt-repository ppa:linuxuprising/java
```

```
apt update
```

```
apt install oracle-java17-installer -y
```

</details>

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

5. Lizenzen akzeptieren und dateirechte vergeben

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
Die Konsole kann mit "screen -r minecraft" geöffnet werden.
{% endhint %}

7.

[^1]: 
