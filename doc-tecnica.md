# DOCUMENTACIÓ TÈCNICA DE L'APLICACIÓ BAS SOLUTIONS

## 1. MENÚ
El menú consta de 7 opcions, les sis primeres són les eines i l'opció 7 és ficar una "q" i surt del menú.
![Menú](https://github.com/betlem96/Documentacio-Projecte/tree/main/imatges/menu.png)

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

![Menú escaneig](/home/alumne/Documents/2on/Projecte/escm.png)

### Opció 1

**Entrada**

![Opció 1](/home/alumne/Documents/2on/Projecte/esc1.png)

**Sortida**

![Opció 1](/home/alumne/Documents/2on/Projecte/esc1-2.png)

### Opció 2

**Entrada**

![Opció 2](/home/alumne/Documents/2on/Projecte/esca2.png)

**Sortida**

![Opció 2](/home/alumne/Documents/2on/Projecte/esc2-1.png)

### Opció 3

**Entrada**

![Opció 3](/home/alumne/Documents/2on/Projecte/esc3.png)

**Sortida**

![Opció 3](/home/alumne/Documents/2on/Projecte/esc3-1.png)

### Opció 4

**Entrada**

![Opció 4](/home/alumne/Documents/2on/Projecte/esc4.png)

**Sortida**

![Opció 4](/home/alumne/Documents/2on/Projecte/esc4-1.png)

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca4_escaneig.py
```

## 5. SSH
**Entrada**

![Opció 5](/home/alumne/Documents/2on/Projecte/ssh1.png)

**Sortida**

![Opció 5](/home/alumne/Documents/2on/Projecte/ssh2.png)

![Opció 5](/home/alumne/Documents/2on/Projecte/ssh2-1.png)

![Opció 5](/home/alumne/Documents/2on/Projecte/ssh2-2.png)

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca5_ssh.py
```

## 6. ENUMERACIÓ
**Entrada**

![Opció 6](/home/alumne/Documents/2on/Projecte/enu1.png)

**Sortida**

Per a consultar el codi entreu a aquesta URL:
```
https://github.com/SergiRoigSanchez/BAS-Solutions/blob/main/tasca6_enumeracio.py
```

## 7. BOT DE TELEGRAM
**Imatges explicatives**
- Per a iniciar el bot

![Imatge d'iniciar el bot](/home/alumne/Documents/2on/Projecte/t_1.png)

- Per a ficar un nou bot

Demanem un bot nou

![Demanar bot nou](/home/alumne/Documents/2on/Projecte/t_2.png)

Definim un nom al bot

![Definir nom al bot nou](/home/alumne/Documents/2on/Projecte/t_3.png)

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
![Descarregar](/home/alumne/Documents/2on/Projecte/cd1.png)
Descomprimim el .tar.gz
```
tar -xzvf go1.21.3.linux-amd64.tar.gz
```
![Descomprimir](/home/alumne/Documents/2on/Projecte/cd2.png)
Exportem les variables de path
```
export GOROOT=/home/alumne/Documents/Programes/go
```
![Exportar](/home/alumne/Documents/2on/Projecte/cd3.png)
```
export GOPATH=/home/alumne/Documents/Programes/go/projectes
```
![Exportar](/home/alumne/Documents/2on/Projecte/cd4.png)
```
export PATH=/$PATH:$GOROOT/bin
```
![Exportar](/home/alumne/Documents/2on/Projecte/cd5.png)

**Configuració del proxy Tor**

Clonem el repositori del docker-image-generator
```
git clone https://github.com/tuxotron/docker-image-generator
```
![Clonar](/home/alumne/Documents/2on/Projecte/cd6.png)
Entrem dintre de la carpeta
```
cd docker-image-generator
```
![Entrar a carpeta](/home/alumne/Documents/2on/Projecte/cd7.png)

Instal·lem el docker-image-generator
```
go build
```
![Instal·lar](/home/alumne/Documents/2on/Projecte/cd8.png)
Creem el docker
```
./doig -i bas_proxy -t anonsurf tinyproxy
```
![Crear docker](/home/alumne/Documents/2on/Projecte/cd9.png)
![Entrem](/home/alumne/Documents/2on/Projecte/cd10.png)
Entrem al docker
```
docker run -it --rm --privileged -p 8888:8888 bas_proxy
```
![Encendre](/home/alumne/Documents/2on/Projecte/cd11.png)
Posem en marxa l'anonsurf
```
anonsurf start
```
![Executar](/home/alumne/Documents/2on/Projecte/cd12.png)
Executem el tinyproxy
```
tinyproxy
```
![Execució](/home/alumne/Documents/2on/Projecte/cd13.png)
Cada vegada que vulguem posar en marxa el nostre proxy Tor haurem d'executar el contenidor i les dos comandes anteriors. Automatitzarem aquest procés:
```
./doig -d -t anonsurf tinyproxy > Dockerfile
```
![Automatic](/home/alumne/Documents/2on/Projecte/cd14.png)
Entrem al Dockerfile
```
nano Dockerfile
```
![nano](/home/alumne/Documents/2on/Projecte/cd15.png)

Li afegim la línia "CMD anonsurf start; tinyproxy -d" al final de l'arxiu. Això fa que Docker executi les dos comandes que necessitem al arrencar el contenidor. el -d fa que el tinyproxy s'executi al foreground.
![Afegir linea](/home/alumne/Documents/2on/Projecte/cd16.png)
Construim la imatge
```
docker buildx build -t bas_proxy .
```
![Construir](/home/alumne/Documents/2on/Projecte/cd17.png)
Executem el contenidor. L'opció -d fa que el contenidor s'executi en segon pla.
```
docker run -d -p 8888:8888 --privileged bas_proxy
```
![Execució](/home/alumne/Documents/2on/Projecte/cd18.png)

El contenidor s'estarà executant en segon pla fins que el parem amb la comanda següent.
```
docker stop c1f1c6b591f9907184027d373e28ac1b348d443d2ef9f02c03b7232463b609e5
```
Per a comprovar si el contenidor s'està executant fem el següent.
```
docker ps
```
![Comprovar](/home/alumne/Documents/2on/Projecte/cd19.png)

Crearem un compte per a poder pujar la imatge al següent link.
```
https://hub.docker.com
```
![Crear compte](/home/alumne/Documents/2on/Projecte/cd20.png)

Fem login amb les coredencials corresponents.
```
docker login
```
![Login](/home/alumne/Documents/2on/Projecte/cd21.png)

La imatge ha de tenir el tag usuari/imatge
```
docker tag bas_proxy sergiroig/bas_proxy
```
![Tag](/home/alumne/Documents/2on/Projecte/cd22.png)

Pujem la imatge
```
docker push sergiroig/bas_proxy
```
![Pujar imatge](/home/alumne/Documents/2on/Projecte/cd23.png)

Ara és possible executar el contenidor des de qualsevol màquina que tingui Docker. Podem veure el repositori a la web.

![Executar](/home/alumne/Documents/2on/Projecte/cd24.png)
Si entrem podem veure quina és la comanda per a fer pull de la imatge.

![Comanda](/home/alumne/Documents/2on/Projecte/cd25.png)
