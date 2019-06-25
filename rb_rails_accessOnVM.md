## **So kann man seinen lokalen Rails Server auf einer Virtualbox VM starten, zum Beispiel für cross browser testing:**

### Auf Host:


```
$ rails s -b 0.0.0.0 -p 3000
```

In VirtualBox folgende Konfigurationen vornehmen:

```

File -> Host Network Manager -> create

Dort dann DHCP aktivieren. Configure Adapter Manually sollte ausgewählt sein und alle IP Adressen, Masks und Prefix ausgefüllt.
```


### Danach in die Settings der VM:

```

Network -> Adapter 1: Host-only Adapter & vboxnet0 (das vorhin erstellte)

Adapter 2: enabled & NAT
```

### Auf dem Guest:


```
Den Browser öffnen -> die IP des Hosts im vboxnet0 (ifconfig auf Host) mit Port 3000 ansteuern
```
