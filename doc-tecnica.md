# DOCUMENTACIÓ TÈCNICA DE L'APLICACIÓ BAS SOLUTIONS

## 1. MENÚ
El menú consta de 7 opcions, les sis primeres són les eines i l'opció 7 és ficar una "q" i surt del menú.

![Menú](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/menu.jpg)

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/menu.py
```

## 2. SHODAN
**Entrada**


**Sortida**

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca1_shodan.py
```

## 2. THE HARVESTER
**Entrada**

**Sortida**

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca2_harvester.py
```

## 3. OSINT
**Entrada**

**Sortida**

Per a consultar el codi entreu a aquesta URL:
```
```

## 4. ESCANEIG
En aquesta eina quan entrem hi ha un menú amb diferents opcions:

![Menú escaneig](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/escm.png)

### Opció 1

**Entrada**

![Opció 1](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc1.png)

**Sortida**

![Opció 1](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc1-2.png)

### Opció 2

**Entrada**

![Opció 2](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esca2.png)

**Sortida**

![Opció 2](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc2-1.png)

### Opció 3

**Entrada**

![Opció 3](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc3.png)

**Sortida**

![Opció 3](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc3-1.png)

### Opció 4

**Entrada**

![Opció 4](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc4.png)

**Sortida**

![Opció 4](https://github.com/betlem96/Documentacio-Projecte/blob/main/imatges/esc4-1.png)

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca4_escaneig.py
```

## 5. SSH
**Entrada**

![Opció 5](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/ssh1.png)

**Sortida**

![Opció 5](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/ssh2.png)

![Opció 5](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/ssh2-1.png)

![Opció 5](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/ssh2-2.png)

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca5_ssh.py
```

## 6. ENUMERACIÓ
**Entrada**

![Opció 6](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/enu1.png)

**Sortida**

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca6_enumeracio.py
```

## 7. BOT DE TELEGRAM
**Imatges explicatives**
- Per a iniciar el bot

![Imatge d'iniciar el bot](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/t_1.png)

- Per a ficar un nou bot

Demanem un bot nou

![Demanar bot nou](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/t_2.png)

Definim un nom al bot

![Definir nom al bot nou](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/t_3.png)

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca_telegram.py
```

## 8. CONTENIDOR DOCKER PER AUDITORIES AUTOMATITZADES

**Instal·lació de GO**

Decarreguem la versió de Linux per a GO. Aquí està el link:
```
https://go.dev/dl/
```
![Descarregar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd1.png)
Descomprimim el .tar.gz
```
tar -xzvf go1.21.3.linux-amd64.tar.gz
```
![Descomprimir](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd2.png)
Exportem les variables de path
```
export GOROOT=/home/alumne/Documents/Programes/go
```
![Exportar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd3.png)
```
export GOPATH=/home/alumne/Documents/Programes/go/projectes
```
![Exportar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd4.png)
```
export PATH=/$PATH:$GOROOT/bin
```
![Exportar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd5.png)

**Configuració del proxy Tor**

Clonem el repositori del docker-image-generator
```
git clone https://github.com/tuxotron/docker-image-generator
```
![Clonar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd6.png)
Entrem dintre de la carpeta
```
cd docker-image-generator
```
![Entrar a carpeta](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd7.png)

Instal·lem el docker-image-generator
```
go build
```
![Instal·lar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd8.png)
Creem el docker
```
./doig -i bas_proxy -t anonsurf tinyproxy
```
![Crear docker](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd9.png)
![Entrem](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd10.png)
Entrem al docker
```
docker run -it --rm --privileged -p 8888:8888 bas_proxy
```
![Encendre](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd11.png)
Posem en marxa l'anonsurf
```
anonsurf start
```
![Executar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd12.png)
Executem el tinyproxy
```
tinyproxy
```
![Execució](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd13.png)
Cada vegada que vulguem posar en marxa el nostre proxy Tor haurem d'executar el contenidor i les dos comandes anteriors. Automatitzarem aquest procés:
```
./doig -d -t anonsurf tinyproxy > Dockerfile
```
![Automatic](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd14.png)
Entrem al Dockerfile
```
nano Dockerfile
```
![nano](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd15.png)

Li afegim la línia "CMD anonsurf start; tinyproxy -d" al final de l'arxiu. Això fa que Docker executi les dos comandes que necessitem al arrencar el contenidor. el -d fa que el tinyproxy s'executi al foreground.
![Afegir linea](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd16.png)
Construim la imatge
```
docker buildx build -t bas_proxy .
```
![Construir](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd17.png)
Executem el contenidor. L'opció -d fa que el contenidor s'executi en segon pla.
```
docker run -d -p 8888:8888 --privileged bas_proxy
```
![Execució](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd18.png)

El contenidor s'estarà executant en segon pla fins que el parem amb la comanda següent.
```
docker stop c1f1c6b591f9907184027d373e28ac1b348d443d2ef9f02c03b7232463b609e5
```
Per a comprovar si el contenidor s'està executant fem el següent.
```
docker ps
```
![Comprovar](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd19.png)

Crearem un compte per a poder pujar la imatge al següent link.
```
https://hub.docker.com
```
![Crear compte](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd20.png)

Fem login amb les coredencials corresponents.
```
docker login
```
![Login](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd21.png)

La imatge ha de tenir el tag usuari/imatge
```
docker tag bas_proxy sergiroig/bas_proxy
```
![Tag](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd22.png)

Pujem la imatge
```
docker push sergiroig/bas_proxy
```
![Pujar imatge](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/cd23.png)

Ara és possible executar el contenidor des de qualsevol màquina que tingui Docker. Podem veure el repositori a la web.

![Executar](/home/alumne/Documents/2on/Projecte/cd24.png)
Si entrem podem veure quina és la comanda per a fer pull de la imatge.

![Comanda](/home/alumne/Documents/2on/Projecte/cd25.png)
