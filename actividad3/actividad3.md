### Actividad 3

# Parte 1: Gestión de Usuarios
- **Creación de Usuarios**
  
```
sudo useradd -m usuario1
```

```
sudo useradd -m usuario2
``` 
```
sudo useradd -m usuario3
``` 
<img src="images/1.png" alt="drawing" width="500">

- **Asignación de Contraseñas**

```
sudo passwd usuario1
```

```
sudo passwd usuario2
```

```
sudo passwd usuario3
```
<img src="images/3.png" alt="drawing" width="500">

- **Información de Usuarios**

```
sudo passwd usuario1
```

<img src="images/5.png" alt="drawing" width="500">

- **Eliminación de Usuarios**

```
sudo userdel usuario3
```

<img src="images/7.png" alt="drawing" width="500">

# Parte 2: Gestión de Grupos

- **Creación de Grupos**

```
groupadd grupo1
```

```
groupadd grupo2
```

<img src="images/8.png" alt="drawing" width="500">

<img src="images/9.png" alt="drawing" width="500">

- **Agregar Usuarios a Grupos**

```
usermod -a -G grupo1 usuario1
```

```
usermod -a -G grupo2 usuario2
```
<img src="images/10.png" alt="drawing" width="500">

<img src="images/11.png" alt="drawing" width="500">

- **Verificar Membresía**
```
groups usuario1
```
```
groups usuario2
```

<img src="images/10.png" alt="drawing" width="500">

<img src="images/12.png" alt="drawing" width="500">

- **Eliminar Grupo**

```
groupdel grupo2
```

<img src="images/13.png" alt="drawing" width="500">
<img src="images/14.png" alt="drawing" width="500">
<img src="images/15.png" alt="drawing" width="500">

