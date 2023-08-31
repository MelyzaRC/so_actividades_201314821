## Actividad 4

# Creación de un systemd unit de tipo servicio 

- Archivo ***actividad4.service***
```
[Unit]
Description=Actividad4
After=network.target

[Service]
Type=simple
ExecStart="/home/melyza/Escritorio/script.sh"

[Install]
WantedBy=default.target
```
  <img src="images/4.png" alt="drawing" width="1000">

El archivo se encuentra alojado en el siguiente directorio

``` /etc/systemd/system```

<img src="images/2.png" alt="drawing" width="1000">

- Script que ejecuta el servicio ***script.sh**

```
#!/bin/bash
echo "201314821"
echo "Fecha actual: $(date +%d/%m/%Y)"
```

<img src="images/5.png" alt="drawing" width="1000">

- Comandos utilizados

```
sudo systemctl daemon-reload

```

```
sudo systemctl enable actividad4.service

Salida:
Created symlink /etc/systemd/system/default.target.wants/actividad4.service → /etc/systemd/system/actividad4.service.

```

```
sudo systemctl start actividad4.service

```

- Verificando estado del servicio creado

Comando utilizado

```
sudo systemctl status actividad4.service

```

<img src="images/1.png" alt="drawing" width="1000">

- Verificando informaciòn de los servicios

```
sudo systemctl list-unit-files --type service --all

```

<img src="images/3.png" alt="drawing" width="1000">
