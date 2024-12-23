# Projecte-A04-01
### Treball realitzat a les branques "albert" i "karolayn"
## 08/11/24

# Projecte-A04-01 
## Branca DAW - Albert Penadés Casajús

## Objectius:
#### L’objectiu principal del projecte és la creació d’un sistema de fitxatge per una institució on quedi registrat en quin moment entra i surt una persona en un espai determinat d’un edifici d’una organització (podria ser una empresa, un institut, etc...). 

#### A nivell tècnic caldrà realitzar la creació d'un dispositiu basat en Arduino que permeti la lectura de dades de targetes RFID i l'enviament d'aquestes a una base de dades centralitzada. S'hauran d'integrar diversos components d'infraestructura per a garantir la seguretat, l'escalabilitat i el correcte funcionament d'aquest sistema en un entorn simulat d'empresa.
#### Serà necessari el disseny d’una base de dades que contempli aquests requeriments, així com possibles ampliacions del projecte. Caldrà fer el disseny i planificació de la infraestructura de servidors, així com el seu desplegament en la infraestructura d’Isard. Des del servidor, caldrà recollir les lectures que s’envien des del dispositiu i guardar-les en la base de dades, a més de proporcionar un feedback al dispositiu, per a indicar un possible error.

## Descripció i requeriments tècnics (apartat només de DAW):
### 1. Infraestructura del sistema:
#### El sistema es basarà en una infraestructura composta per diversos servidors:
#### ■ Un servidor web configurat amb un nom de domini
#### ■ Un servidor de base de dades que gestionarà totes les dades generades pel sistema.

### 2. Programació i desplegament:
#### S'haurà de desenvolupar una aplicació web que permeti la gestió ivisualització de les dades de l’alumnat. Tindrem diferents rols:
#### ■ Alumne/a: haurà de poder accedir a la seva pròpia informació
#### ■ Administradors: tindran accés a totes les funcions.
#### ■ Professorat: podran passar llista, veure l’assistència dels seus grups, i afegir-se el seu horari, modificar l'assistència, etc.


## 3. Monitoratge i seguretat:
#### ■ Tots els servidors i dispositius han d'estar monitoritzats constantment, de manera que qualsevol canvi en els arxius o intents de connexió no autoritzada quedin registrats. S’utilitzarà un script amb cron, i avís per correu electrònic.

## Important:
### L' aplicació ha de permetre la gestió de marcatges, horaris i retards, organitzant la informació en funció de la estructura que tingui la organització (departament, pisos, aules, edificis, etc.). 

### El desplegament de l'aplicació web haurà de ser automàtic, connectant-se a un sistema de control de versions (com Git) per actualitzar l’aplicació.

# Documentació Wireframe DAW:
## Iniciar sessió
![Iniciar sessió](image-1.png)

## Crear compte
![Crear compte](image.png)
### Ens servirà per crear un compte nou

## Selecció d'ús del compte creada
![creació del compte](image-2.png)
### Sol podrà accedir com a alumne, més endavant podrà ser modificat per poder afegir els seus permisos.

# APARTAT D'ALUMNE
![Safata d'entrada](image-3.png)
### Podem veure dues imatges, l'única diferència que podem trobar és el menú desplegable, és sol per la visualització. Per cada framework hi ha dues imatges.

### En aquest apartat podem veure que disposa d'un llistat de notificacions al centre, aquest seria les alertes que envia el centre, molt semblant al gmail de google.
### Podem veure a la part superior a la dreta l'imatge del nostre usuari. Si presiona l'icona podem veure que:
![Tancar sessió](image-4.png)

## Enviar missatge
![Enviar misstage](image-5.png)
### Apartat on l'usuari podrà enviar un correu a qui vulgui. Podrà adjuntar fitxers si ell vol.

## Assistències mòduls
![Assistències mòduls](image-6.png)
### L'usuari podrà veure les seves assistències. Podem veure que primer estan separades per mòduls. Disposa d'una barra de búsqueda per facilitar l'ús de cerca.

## Assitències separades per RA's
![Assistències RA's](image-7.png)
### Podem veure que un cop el nostre alumne hagi entrar al mòdul dessitjat li aparaixen les RA's o resultats d'aprenentatges. Si ens hi fixem podem veure que hi ha una "ruta" just a sobre perquè l'alumne es pugui moure lliurement en aquest apartat.

## Assitències informació de les RA's
### Un cop seleccionada la RA que l'alumne decideix veure, tindrà un llistat de "missatges" conforme ja han passat llista. Aquests tindrà un missatge segons si ha estat present, ha arribat tard o si no ha vingut.
![Dins del missatge](image-8.png)

# APARTAT DE PROFESSOR
## Safata d'entrada
![Safata d'entrada](image-9.png)
### Disposa del mateix format que del alumne,

![Missatges enviats](image-10.png)
### Podra enviar correus a altres professors, i als seus alumnes.

## Assitències mòdul
![Assistències](image-11.png)
### Disposarà dels mòduls que ell dongui. Si fa clic dins del seu mòdul veurà que:
![RA's](image-12.png)
### Disposarà d'una taula o informació del horari que ell imparteix. També té un botó que servirà per poder editar les hores que ell dóna.

## Taula d'assistència
![Taula d'assistència](image-13.png)
### Podrà controlar el sistema d'assistència a classe. Podrà posar retards, absències, faltes...

# Apartat d'Administrador
## Admin
![Admin](image-14.png)
### Apartat on podrem veure tot i tenir accès a totes les funcions. Podrem veure els usuaris que s'han creat ja siguit alumnes o professors, podrem veure els horaris, els grups i un apartat de configuració

## Usuaris
![Usuaris](image-15.png)
### Secció on podrem veure tots els usuaris creats. Aquí podrem diferenciar els diferents rols d'alumne i professor. A la següent imatge podem veure que disposen de la mateixa estructura, separat per curs. L'únic que varia és el nom ens trobem situats.
![Alumnes i Professors](image-16.png)

## Llistat d'alumnes de 1r i 2n de DAW
![Llistat d'alumnes de 1r i 2n de DAW](image-17.png)
### Aquí podem veure tots els alumnes creats de DAW separats per any (1r i 2n). És el mateix per els altres cursos (DAM i ASIX). Si ens hi fixem podem veure a la part superior del wireframe 3 icones, aquests serviràn per editar un alumne, eliminar un alumne i per afegir un alumne.

## Llistat de professors
![Llistat de professors de 1r i 2n de DAW](image-18.png)
### Podem veure tots els professors de 1r i 2n de DAW. Per els altres cursos serà el mateix format. Així com els alumnes, els professors tindran les mateixes icones per poder editar, eliminar i afegir professor.

# Horaris
## Distribució dels horaris.
![Apartat d'horaris de les classes](image-19.png)
### Aquest apartat estarà dividit per dos botons principals que més endavant redirigirà als cursos d'aquell any.
### 1r any
![Horaris 1r](image-20.png)

### 2n any 
![Horaris de 2n](image-21.png)

### Un cop dins podem veure que cada curs tindrà els seus horaris establerts. Aquests podràn ser modificats.
#### Horaris de 1r
![Horaris de 1r DAW, DAM, ASIX](image-22.png)

#### Horaris de 2n
![Horaris de 2n DAW, DAM, ASIX](image-23.png)

# Grups
## En aquest apartat sol disposarà de 3 botons que redirigirà a les webs que ja han sigut anteriorment creades.
![Grups](image-24.png)

# Configuració
## Apartat dedicat a la configuració bàsica de la web. Aquí hi haurà informació bàsica, botons per cambiar d'hora, idioma, comptes, cofigurar tamany...
![Configuració](image-25.png)

## Secció del admin per veure tots els usuaris creats
![Veure tots els usuaris creats](image-27.png)

#### Estan dividits per: Alumne, Professor i Admin:
![Tipus d'usuaris](image-28.png)

# Base de dades - Model relacional
![BBDD Model relacional](image-26.png)