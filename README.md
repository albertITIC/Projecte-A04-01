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
