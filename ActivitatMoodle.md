# ACTIVITAT INSTAL·LACIÓ MOODLE

Primer anem a moodle i a "Downloads" hem de descarregar l'arxiu més recent en zip.

![image](https://user-images.githubusercontent.com/114162341/203819036-fe6f6304-1033-4016-94d6-b7e2ef0e64a1.png)

Ara fem clic dret al text amb un enllaç i li donem a "Copia l'adreça de l'enllaç".

![image](https://user-images.githubusercontent.com/114162341/203819381-34f82b98-9ca4-4dc7-ae1b-b19037d01398.png)

Ara posem aquesta comanda a la terminal que tenim connectada amb ssh a la màquina virtual d'ubuntu server.

![image](https://user-images.githubusercontent.com/114162341/203820233-819662d2-5a17-4610-ab3d-1456a3d7d148.png)

Ara fem un update.

![image](https://user-images.githubusercontent.com/114162341/203821545-3efc2d2c-c068-4703-a4ff-b03205e520d3.png)

Ara instal·lem el apache2.

![image](https://user-images.githubusercontent.com/114162341/203821636-a0732a78-bb36-4780-b12a-b1aff3679ace.png)

Ara instal·lem el mariadb-server.

![image](https://user-images.githubusercontent.com/114162341/203821771-f1ded828-8045-4d7c-8d5c-c7af6f7430bc.png)

Ara executem la comanda de seguretat.

![image](https://user-images.githubusercontent.com/114162341/203822072-fcdfc212-a2c1-4c56-8def-fda41de8e067.png)

I amb aquesta comanda iniciem com a root amb mariaDB amb un usuari extern.

![image](https://user-images.githubusercontent.com/114162341/203823313-8cfd5f19-5560-4c42-8d1c-ca47fd18c592.png)

I ara instal·lem el PHP.



Ara posem aquesta comanda per a accedir a aquest arxiu de configuració.

![image](https://user-images.githubusercontent.com/114162341/203825235-54e37e4d-6fef-4143-8bbb-6379ce38bd93.png)

Ara posem el "index.php" al principi de tots els index.

![image](https://user-images.githubusercontent.com/114162341/203825635-fe464caf-df1c-4e40-aa23-51afafe85301.png)

Ara instal·lem el php7.3 amb aquesta comanda.

``He fet servir aquesta guia: https://www.tecno-tips.com/php/instalar-php-7-3-7-2-7-1-7-0-5-6-ubuntu-20-04/ ``

![image](https://user-images.githubusercontent.com/114162341/203826739-72320b48-507e-46c9-a642-5e9d8d641440.png)

Ara reiniciem el apache2.

![image](https://user-images.githubusercontent.com/114162341/203827036-819f9706-265d-4966-bbea-38078bb9fb5d.png)

Ara fem un status per a veure que funciona.

![image](https://user-images.githubusercontent.com/114162341/203827140-de2473ad-69f8-42d9-b71a-920421171409.png)

Ara crearem aquest arxiu.

![image](https://user-images.githubusercontent.com/114162341/203827357-bc382bb6-f9d0-4cf9-a6a0-99346a4c683a.png)

Ara simplement escrivim aquesta linia i guardem.

``<?php phpinfo(); ?>``

![image](https://user-images.githubusercontent.com/114162341/203827653-20db0698-ebe5-4700-be94-754958208ef1.png)

I finalment eliminem aquest arxiu ja que exposem informació de la nostra versió i configuració d'aquest fitxer a les persones externes.

![image](https://user-images.githubusercontent.com/114162341/203827862-651ae641-d983-4014-9466-847ebabe490c.png)

I ara ja podem continuar la instal·lació del moodle, fem un unzip del arxiu instal·lat anteriorment.

![image](https://user-images.githubusercontent.com/114162341/203828486-36e62738-400d-4d4f-b125-d95b89b43703.png)

Ara canviem el propietari del arxiu.

![image](https://user-images.githubusercontent.com/114162341/203828972-002998c7-deb3-451c-9e55-f606e1e9161d.png)

Ara creem el directori de fitxers i li donem propietari amb les següents comandes.

![image](https://user-images.githubusercontent.com/114162341/203829690-f18a8db9-cc48-4776-9b5e-f5b945984ef3.png)

Ara accedim dins de la base de dades per a configurar-la.

![image](https://user-images.githubusercontent.com/114162341/203830527-37824971-d2a9-499b-985a-c5bd185ab00c.png)

Creem un usuari en el meu cas l'he deixat com a la guia "moodlemanager".

![image](https://user-images.githubusercontent.com/114162341/203831177-9b458d33-04b3-44e7-8b86-ed2ae166c81f.png)

Ara creem la base de dades per a moodle.

![image](https://user-images.githubusercontent.com/114162341/203831252-23985600-83ee-488e-a481-90043edb26d3.png)

I li donem permissos al usuari creat.

![image](https://user-images.githubusercontent.com/114162341/203831414-ffa0f549-2fa5-4647-bb5d-ed333e0831ae.png)

I finalment si posem la ip de la màquina i la direcció ja ens sortirà la pàgina.

![image](https://user-images.githubusercontent.com/114162341/203832103-8e037480-9419-4bc3-8fb5-68f88adef5b7.png)

Ara configurarem el moodle, el primer que hem de fer és triar el idioma, en el nostre cas el català.

![image](https://user-images.githubusercontent.com/114162341/205075604-6e0a247d-ae28-4063-bb6f-d5343e98fc8d.png)

Ara ens dirà que necessitem la extensió zip del PHP.

![image](https://user-images.githubusercontent.com/114162341/205076106-3a657bb7-1fef-4e43-a910-ab1867a93732.png)

Per a solucionar-ho hem d'anar a la terminal i posar aquesta comanda.

![image](https://user-images.githubusercontent.com/114162341/205076513-3a746f53-214f-4ca4-bba4-a735fc0f0520.png)

Ara fem un grep per a buscar el zip.

![image](https://user-images.githubusercontent.com/114162341/205078759-a6076b2d-863e-4aa5-b41b-caa3445e528c.png)

Ara instal·lem el paquet.

![image](https://user-images.githubusercontent.com/114162341/205079355-89441481-7642-4a01-b97d-a646894bf51b.png)

I ara recarguem el servei apache2.

![image](https://user-images.githubusercontent.com/114162341/205079748-9c27d21c-6491-49c1-8276-d1a4625e8f97.png)

Ara ens demana un directori de dades, posarem l'adreça que haviem creat anteriorment.

![image](https://user-images.githubusercontent.com/114162341/205080218-7ff89b44-6e0b-4851-9d75-ac938b4e4927.png)

Seguidament triem el controlador de dades que haguesem instal·lat, en el meu cas el MariaDB.

![image](https://user-images.githubusercontent.com/114162341/205080595-849c91f3-d9cb-4cc6-8974-e60fc884c362.png)

Ara ens pregunta els paràmetres de la base de dades, posarem l'adreça localhost, el usuari moodlemanager i la contrasenya managermoodle, la resta ho deixem tal qual.

![image](https://user-images.githubusercontent.com/114162341/205086940-2761f778-18d8-4010-b5db-3090f55d0a24.png)

Ara ens sortirà aquest problema.

![image](https://user-images.githubusercontent.com/114162341/205087084-5eea1758-0b6f-4911-bf4f-799522e07a54.png)

Per a solucionar-ho simplement instal·lem el paquet.

![image](https://user-images.githubusercontent.com/114162341/205087436-c04c558d-9b98-485a-a44e-65df6f36ff77.png)

I ara reiniciem l'apache.

![image](https://user-images.githubusercontent.com/114162341/205087521-f45712b4-37f9-4a18-976e-89076c9bc7eb.png)

Per últim ens dirà que s'ha realitzat la instal·lació correctament.

![image](https://user-images.githubusercontent.com/114162341/205087762-7e426747-35b9-4aa8-b34a-c63f9284bc76.png)

Ara moodle comprova que tot està ok i si hem de revisar alguna cosa, en el meu cas he de revisar 2 coses.

![image](https://user-images.githubusercontent.com/114162341/205089280-27d40bf1-8ed5-4bbc-8feb-a28a66c1425b.png)

Per a fer-ho anem a la terminal i posem aquesta comanda per a instal·lar els paquets necessaris.

![image](https://user-images.githubusercontent.com/114162341/205089580-8591ab63-47f9-41e3-9c81-d6e71231b72f.png)

I fem un reload.

![image](https://user-images.githubusercontent.com/114162341/205089902-96da24fd-d4a0-4658-a760-a777d305e31b.png)

Ara veiem que els principals problemes s'han arreglat però encara en tenim un parell.

![image](https://user-images.githubusercontent.com/114162341/205090080-b46b934c-66c1-42f5-a695-224c51a7febe.png)

Però com és una instal·lació local no hi farem cas a aquestes comprovacions.

![image](https://user-images.githubusercontent.com/114162341/205090161-bd2e6b01-d7a6-45e3-84a7-57e3f37d08d4.png)

Ara moodle realitzarà una serie d'accions que ens dirà que ha sortit exitosament.

![image](https://user-images.githubusercontent.com/114162341/205093145-5185d69d-a176-4ea6-b409-047eae84fc2f.png)

Ara moodle ens demana que configuresem un compte d'administrador.

![image](https://user-images.githubusercontent.com/114162341/205094239-ef4a71ef-0d8d-4649-b72f-180c5e33c8a2.png)

Ara fem una petita configuració de la nostra pagina de moodle.

![image](https://user-images.githubusercontent.com/114162341/205095065-62da629e-ed1f-4262-9d51-7e0bf9154343.png)

Ara també ens demana canviar aquests paràmetres.

![image](https://user-images.githubusercontent.com/114162341/205095937-d7f78ebe-afff-4a02-8700-4eeadae375bf.png)

![image](https://user-images.githubusercontent.com/114162341/205096745-f22d02e6-aaec-4b1a-8a88-57750010d3ab.png)

I ja estarem dins de la zona d'administració de moodle.

![image](https://user-images.githubusercontent.com/114162341/205096863-4b31b230-46b0-4472-8f3d-6d0336718d74.png)

## SOLUCIÓ D'ERRORS

### PROBLEMA

Ara ens sortirà aquest problema.

![image](https://user-images.githubusercontent.com/114162341/205087084-5eea1758-0b6f-4911-bf4f-799522e07a54.png)

Per a solucionar-ho simplement instal·lem el paquet.

![image](https://user-images.githubusercontent.com/114162341/205087436-c04c558d-9b98-485a-a44e-65df6f36ff77.png)

I ara reiniciem l'apache.

![image](https://user-images.githubusercontent.com/114162341/205087521-f45712b4-37f9-4a18-976e-89076c9bc7eb.png)

### PROBLEMA

Ara moodle comprova que tot està ok i si hem de revisar alguna cosa, en el meu cas he de revisar 2 coses.

![image](https://user-images.githubusercontent.com/114162341/205089280-27d40bf1-8ed5-4bbc-8feb-a28a66c1425b.png)

Per a fer-ho anem a la terminal i posem aquesta comanda per a instal·lar els paquets necessaris.

![image](https://user-images.githubusercontent.com/114162341/205089580-8591ab63-47f9-41e3-9c81-d6e71231b72f.png)

I fem un reload.

![image](https://user-images.githubusercontent.com/114162341/205089902-96da24fd-d4a0-4658-a760-a777d305e31b.png)
