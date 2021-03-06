<p align="center">
<img src ="https://raw.githubusercontent.com/primitivorm/latino/master/logo/banner-300x.png" /><br>http://lenguaje-latino.org/
</p>
<img src ="doc/mac.png" />

## Dependencias 

Antes de instalar latino, vamos a instalar todos paquetes necesarios: 

```
sudo apt-get update && apt-get install bison flex cmake gcc g++ libjansson-dev libcurl4-openssl-dev libhiredis-dev redis-server curl libgtk-3-dev libreadline-dev libpthread-stubs0-dev
```

## INSTALAR


```bash
 git clone --recursive https://github.com/primitivorm/latino
 cd latino
 git submodule update --init --recursive
 cmake .
 make
 sudo make install
```

###Documentacion (borrador)
1. https://robincoello.gitbooks.io/latino/content/inicio.html
2. http://lenguaje-latino.org/doc/index.php


### COMPILAR

---

|Requiere               | Versión
| :---------------------|--------:
| bison                 |  3.04
| flex                  |  2.5.39
| cmake                 |  3.3.1
| gcc                   |  4.9.3
| g++                   |  4.9.3
| libjansson-dev        |  2.9 
| libcurl4-openssl-dev  |  *
| libhiredis-dev        |  *
| redis-server          |  *
| curl                  |  7.47.0
| libgtk-3-dev          |  3.0-2
| libreadline-dev       |  7.0-2
| libpthread-stubs0-dev |  0.3-4

--

### DESINSTALAR

#### 1- Opción
```bash
# Si instalaste con `sudo make install`:
sudo ./uninstall.sh
```

#### 2- Opción

Puedes ver un video de como proceder aca https://youtu.be/Q5xGm_Bp22k

Pirmero debes saber donde esta instalado

 ```bash
 whereis latino
 ```

 Te dará algo parecido a esto:

 ```bash
 latino: /usr/local/bin/latino

 ```

 Ahora que sabemos dónde está solamente lo borramos:
 ```bash
 sudo rm /usr/local/bin/latino

 ```

#### 3- Opción

 **Sólo debian/ubuntu. si instalaste paquete deb
 ```bash
 # Ubuntu 16.x.x en adelante
 sudo apt remove latino
 # Ubuntu 14.x.x hacía atrás
 sudo apt-get remove latino
 

## Ayuda en nuestro foro 

http://lenguaje-latino.org/foro/mac/


####Cualquier aportación o sugerencia es bienvenida.
