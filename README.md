# android-apns-mexico

Configuración de APNs para México (Android), incluye tambien las OMV mas usadas.

AT&T
- YO Mobile

Altán
- Bait
- CFE TEIT
- Diri
- izzi Movil
- Mega Movil
- NeWWW
- Pillofon
- Red TIC

Movistar
- Simplii
- Virgin Mobile
- weex

Telcel
- FreedomPop
- Soriana Movil
- Oui Elektra
- Redi Coppel

Unefon/Iusacell


Para usar este archivo tienes tres opciones:
- Quieres crear el perfil de datos para tu Operadora:
  Abre el archivo XML con cualquier editor de texto y busca a tu operador, solo vas a necesitar el nombre, apn, mcc y mnc.
  Pasos generales:
  1. Ve a Ajustes (o Configuración) de tu teléfono.
  2. Entra en la sección de Redes móviles o Conexiones.
  3. Busca la opción llamada Nombres de puntos de acceso (o APN).
  4. Presiona el botón de "+" (Añadir) o el menú de tres puntos para seleccionar "APN nuevo".
  5. Ingresa los parámetros necesarios (Nombre, APN, MCC, MNC) basándote en la información de tu operador.
  6. Una vez ingresados los campos, presiona el menú (los tres puntos verticales) y selecciona Guardar.
  7. Asegúrate de que el nuevo APN esté seleccionado (debe aparecer un punto azul o una marca al lado).
  8. Reinicia tu celular o activa/desactiva el Modo Avión para que el sistema detecte los cambios en la red.

- Vas a agregarlo al archivo apns-config.xml porque andas manoseando los archivos de sistema de tu telefono y te diste cuenta que aun existe nextel en la parte de mexico y AT&T/unefon todavia tienen los datos de iusacell: (Aqui considero que ya sabes donde esta el archivo y tienes un explorador con root)
  1. Copia y pega los datos dentro de la seccion de mexico (MX / MX CARRIERS / Mexico - "Carrier" / MCC 334 / etc), si estas en este paso, ya sabes como se hace.
  2. Guarda el archivo y no olvides agregarle el permiso 664 (En terminal: chmod 664 /ruta/etc/apns-config.xml, En explorador root: Habra algunas opciones, selecciona: Propietario R/W, Grupo R, Otros R)
  3. Reinica tu cel

 - Estas trabajando en una ROM oficial/patito/modificada/port/etc y decidiste buscar las apn de mexico pq nos quieres mucho o nomas quieres tener la lista completa
   1. Agregalos a la seccion de mexico en el apns-config.xml
   2. Lo guardas, no se como o que permisos ocupe, no hago roms. 

No creo actualizar esta cosa asi que, si sale algun operador virtual nuevo o pasa el cambio de infraestructura Movistar a Virgin puede que lo actualice, puede que no, nextel no esta, ya nadie lo usa pero igual luego lo pongo.
