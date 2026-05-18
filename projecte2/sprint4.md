---
layout: default
title: "Sprint 4.Configuració del Programari de Base i Sistemes d’Emmagatzematge en Windows"
permalink: projecte2/sprint4/
---

## RAIDs a Windows server

### Preparacio inicial

Avans d'inciar la mv afegim 3 discs extra, en el meu cas de 5gb cadascun

<img width="412" height="269" alt="image" src="https://github.com/user-attachments/assets/b4ec2199-fa1a-4ac4-9f50-285f8f92e9a8" />


Iniciem la maquina i desde administracio de discos els iniciem en format MBR

<img width="598" height="441" alt="image" src="https://github.com/user-attachments/assets/9da6de14-92ea-499b-8508-30d77c6a1f21" />

<img width="654" height="316" alt="image" src="https://github.com/user-attachments/assets/a0a22dcc-f5e4-405d-b3f9-95b33b0148b9" />


Sense formatarlos ni crear particions, seleccionarem "nou volum raid 5" des de un dels disc 

<img width="808" height="264" alt="image" src="https://github.com/user-attachments/assets/b0c92a50-a9cb-426b-8d18-6b02274096f6" />


Des del assistent que s'obre afegim els altres dos

<img width="520" height="426" alt="image" src="https://github.com/user-attachments/assets/ecfb3767-d640-4c6a-891e-a7f8e3d1da8e" />


Assignem una lletra d'acces "D:"

<img width="520" height="426" alt="image" src="https://github.com/user-attachments/assets/8801754b-d434-4f0c-8cc3-8b27020f1705" />


Assignem format d'arxius ntfs i un nom "raid5-test"

<img width="520" height="426" alt="image" src="https://github.com/user-attachments/assets/81317ffd-44fb-4662-8640-bb48ed227d7d" />


Acceptem la configuracio i deixem que es formati correctament

<img width="618" height="321" alt="image" src="https://github.com/user-attachments/assets/ed98a95b-99fd-4e55-b518-7316e194b308" />


S'ha creat un unic volum per els tres discos

<img width="704" height="172" alt="image" src="https://github.com/user-attachments/assets/ae168666-02ed-45a6-b995-9159fb369239" />


## Proves

Creem o copiem un par de documents tambe una carpeta i comprovem que son accessibles

<img width="620" height="176" alt="Captura de pantalla de 2026-05-14 14-17-03" src="https://github.com/user-attachments/assets/3def62ca-f773-4343-9749-3dd4c9287128" />

<img width="882" height="591" alt="Captura de pantalla de 2026-05-14 14-17-23" src="https://github.com/user-attachments/assets/53fdfac9-3616-43cb-aa38-5ceaa417ef89" />


