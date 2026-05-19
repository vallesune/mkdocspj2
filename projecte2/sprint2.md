---
layout: default
title: "Sprint 2.Instal·lació, Configuració de Programari de Base i Gestió de Fitxers"
permalink: projecte2/sprint2/
---

## Preparació del Sistema

Afegirem un disc nou a la mv tancada

<img width="510" height="289" alt="Captura de pantalla de 2026-04-16 10-33-21" src="https://github.com/user-attachments/assets/ded2e464-e430-498e-812e-bb7e9be4a351" />


Obriem el windows, el administrador de discs i ja ens avisa que tenim un disc per iniciar, ho fem i es iniciara un asistent

<img width="753" height="476" alt="Captura de pantalla de 2026-04-16 10-34-56" src="https://github.com/user-attachments/assets/215e322b-2696-47e9-b7d7-08efae811d36" />

<img width="581" height="437" alt="Captura de pantalla de 2026-04-16 10-42-44" src="https://github.com/user-attachments/assets/d424e6e5-35b5-41b3-abdc-3a22091b359c" />


Creem la primera particio utilitzant aproximadament la mitad del disc

<img width="581" height="437" alt="Captura de pantalla de 2026-04-16 10-43-49" src="https://github.com/user-attachments/assets/be1a99bb-1f42-4121-a651-625e957c8ce4" />


Li assignem una lletra

<img width="581" height="437" alt="Captura de pantalla de 2026-04-16 10-44-16" src="https://github.com/user-attachments/assets/0822030c-a685-4d0c-abb9-00fbf9f0eaef" />


Li assignem el nom "portable" i de tipo de fitxers fat32

<img width="581" height="437" alt="Captura de pantalla de 2026-04-16 11-39-08" src="https://github.com/user-attachments/assets/e583a76e-a6d6-429a-86f5-c7fec589233d" />


Comprovem, acceptem i es crea

<img width="581" height="437" alt="Captura de pantalla de 2026-04-16 11-39-29" src="https://github.com/user-attachments/assets/261080b9-8594-4eaa-8d7c-bac43615ffb1" />

<img width="688" height="131" alt="Captura de pantalla de 2026-04-16 11-40-06" src="https://github.com/user-attachments/assets/96a1f146-6f2a-4f25-b9bd-eb1db60448d5" />


Repetim el proces en l'altra mitad del disc

<img width="502" height="395" alt="Captura de pantalla de 2026-04-16 11-41-11" src="https://github.com/user-attachments/assets/bf2ec1be-30a3-4ba1-ba6a-30e29a7f2dff" />


Li assignem el tipo NTFS i el nom Dades

<img width="502" height="395" alt="Captura de pantalla de 2026-04-16 11-41-27" src="https://github.com/user-attachments/assets/8c4cbfa9-0a02-4770-82e7-145d052b46eb" />


S'ha creat correcte

<img width="667" height="126" alt="Captura de pantalla de 2026-04-16 11-41-57" src="https://github.com/user-attachments/assets/d863cd7a-ab4c-460f-a139-0d32f5c1d7a1" />

Des de la cmd disposem de "diskpart" i podem executar list disk per comprovar els discs que tenim i list volume per comprovar les particions i podem comprovar que coincideix en la informacio del administrador de discs

<img width="688" height="271" alt="Captura de pantalla de 2026-04-16 11-43-38" src="https://github.com/user-attachments/assets/b6a73a62-f99e-47d8-8be6-607c30ffb474" />




## Quotes de disc i usuari

Activem les quotes de disc per la particio Dades i li assignem de limit 300mb 

<img width="386" height="500" alt="Captura de pantalla de 2026-04-23 10-44-36" src="https://github.com/user-attachments/assets/711845c2-2111-4e37-b9c1-339bc4846a31" />

<img width="384" height="131" alt="Captura de pantalla de 2026-04-23 10-45-19" src="https://github.com/user-attachments/assets/87979481-480d-4e15-a5e1-494eeed78a7a" />


Des de administracio d'equips, usuaris i grups, usuaris, podem afegir dos usuaris a nivell local

<img width="671" height="347" alt="image" src="https://github.com/user-attachments/assets/263a219d-37de-451d-bee2-a6307c4c3ea6" />

<img width="430" height="387" alt="image" src="https://github.com/user-attachments/assets/6d24f3c1-38b4-410e-82ac-488aa08897b9" />

<img width="430" height="387" alt="image" src="https://github.com/user-attachments/assets/ad9156d4-6682-4cf3-82a5-d3f46ad60100" />

<img width="755" height="336" alt="image" src="https://github.com/user-attachments/assets/f15b1477-aae4-445f-90bf-cdeb9ab83826" />


Igualment des de administracio d'equips, creem un grup nou anomenat Limitats i afegim els dos users que acabem de crear

<img width="755" height="336" alt="image" src="https://github.com/user-attachments/assets/8db08690-69c8-437f-9b9e-64359802562d" />

<img width="437" height="400" alt="image" src="https://github.com/user-attachments/assets/c73efe18-cabc-4a44-97c6-60a5a2c937ba" />


Veiem que s'ha creat i des de propietats veiem que formen part els dos users

<img width="938" height="544" alt="image" src="https://github.com/user-attachments/assets/0081761f-b02e-4bc8-a94c-a85c8592660a" />

<img width="538" height="529" alt="image" src="https://github.com/user-attachments/assets/0188440a-1b55-49ac-abc3-0ffba2c69d1a" />


Comprovem que els limits de cuota funcionen afegint fitxers de prova a dades
capt


## Scripts de còpia i automatització

Afegim un nou disc a la mv

<img width="781" height="390" alt="image" src="https://github.com/user-attachments/assets/4bda8e13-20df-4eea-91d0-154223e99e2c" />


El formatem igual que anteriorment en NTFS i en nom "Backups"

<img width="631" height="112" alt="image" src="https://github.com/user-attachments/assets/3c32b731-a206-4296-a9e8-29cfaa034121" />

<img width="519" height="416" alt="image" src="https://github.com/user-attachments/assets/00c891a6-7aa5-40eb-a1af-20e6cc48f72b" />

<img width="485" height="103" alt="image" src="https://github.com/user-attachments/assets/1fb4f9af-7fd9-4e91-a452-7352c2efa39f" />


Dins de backups creem la carpeta "CopiesUsuaris"

<img width="573" height="391" alt="image" src="https://github.com/user-attachments/assets/cf89728c-e02d-4fa2-b59a-cd6d3588730d" />

<img width="545" height="122" alt="image" src="https://github.com/user-attachments/assets/bb267ffe-68cf-4436-a092-dafcf234539b" />


Creem un script .bat per copiar els Users del disc C, l'original, a la carpeta copies del disc F que acabem de crear 

<img width="546" height="253" alt="image" src="https://github.com/user-attachments/assets/c8b0f15b-9a90-4987-a27f-ccc57a94fdd1" />



Obrim gpedit.msc, l'editor de directives de grup local i a configuracio d'usuari, configuracio de windows,scripts modificarem el d'inici de sessio

<img width="670" height="293" alt="image" src="https://github.com/user-attachments/assets/b2d4a985-be3d-4a6b-94d3-3be0e08788a1" />


Afegim un parametre nou

<img width="593" height="507" alt="image" src="https://github.com/user-attachments/assets/68983909-45a9-44a3-bf4f-f01b84a03854" />


Busquem l'script que acabem de crear i l'afegim per que s'execute sempre al iniciar sessio

<img width="450" height="306" alt="image" src="https://github.com/user-attachments/assets/31be7c7f-9ca8-40ea-9b33-fd63d906a68b" />






## Gestio de processos i serveis

### Llistar procesos actius

Iniciem sessio com alumne1 local i des d'una terminal cmd executem "tasklist" que ens permet mostrar els processos que estan actius al moment

<img width="672" height="606" alt="image" src="https://github.com/user-attachments/assets/36c8ada7-db38-4679-95e1-03c0b045909e" />


Pasem el mateix resultat a un fitxer redireccionant en un " > /directori/fitxer.txt"

<img width="545" height="53" alt="image" src="https://github.com/user-attachments/assets/92ecb48b-409b-4cec-8cbe-e43cdef17e32" />


Si l'obrim i l'analitzem podem reconeixer alguns processos tipics de Windows com l'explorer, el One drive o altres

<img width="736" height="533" alt="image" src="https://github.com/user-attachments/assets/639379e7-c432-41cd-8ebe-2898c2688a10" />


### Identifiquem processos precindibles

Alguns dels processos que hi ha funcionant son programes com one drive, teams, skype que no son prescindibles per que el sistema funcioni i podem eliminiarlos, pero primer els mostrarem en una taula amb la justificacio que correspon



