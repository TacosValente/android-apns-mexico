# android-apns-mexico

Configuración de APNs para México (Android), incluye también las OMV más usadas.

### Operadores disponibles:

* **AT&T:** YO Mobile.
* **Altán:** Bait, CFE TEIT, Diri, izzi Móvil, Mega Móvil, NeWWW, Pillofon, Red TIC.
* **Movistar:** Simplii, Virgin Mobile, weex.
* **Telcel:** FreedomPop, Soriana Móvil, Oui Elektra, Redi Coppel.
* **Unefon/Iusacell**

---

### ¿Cómo usar este archivo?

#### 1. Quieres crear el perfil de datos para tu operadora:
Abre el archivo XML con cualquier editor de texto y busca a tu operador, solo vas a necesitar el nombre, APN, MCC y MNC.

**Pasos generales:**
1. Ve a **Ajustes** (o Configuración) de tu teléfono.
2. Entra en la sección de **Redes móviles** o **Conexiones**.
3. Busca la opción llamada **Nombres de puntos de acceso** (o APN).
4. Presiona el botón de **"+"** (Añadir) o el menú de tres puntos para seleccionar **"APN nuevo"**.
5. Ingresa los parámetros necesarios (Nombre, APN, MCC, MNC) basándote en la información de tu operador.
6. Una vez ingresados los campos, presiona el menú (los tres puntos verticales) y selecciona **Guardar**.
7. Asegúrate de que el nuevo APN esté seleccionado (debe aparecer un punto azul o una marca al lado).
8. **Reinicia** tu celular o activa/desactiva el **Modo Avión** para que el sistema detecte los cambios en la red.

#### 2. Vas a agregarlo al archivo `apns-config.xml` (Root):
Si andas manoseando los archivos de sistema de tu teléfono y te diste cuenta de que aún existe Nextel en la parte de México y AT&T/Unefon todavía tienen los datos de Iusacell: (Aquí considero que ya sabes dónde está el archivo y tienes un explorador con root).

1. Copia y pega los datos dentro de la sección de México (MX / MX CARRIERS / Mexico - "Carrier" / MCC 334 / etc).
2. Guarda el archivo y no olvides agregarle el permiso **644**:
   * **En terminal:** `chmod 644 /ruta/etc/apns-config.xml`
   * **En explorador root:** Selecciona: Propietario R/W, Grupo R, Otros R.
3. **Reinicia tu cel.**

#### 3. Estás trabajando en una ROM oficial/patito/modificada/port:
Decidiste buscar las APN de México porque nos quieres mucho o nomás quieres tener la lista completa:

1. Agrégalos a la sección de México en el `apns-config.xml`.
2. Lo guardas, no sé cómo o qué permisos ocupe, no hago ROMs.

---

**Nota:** No creo actualizar esta cosa así que, si sale algún operador virtual nuevo o pasa el cambio de infraestructura Movistar a Virgin puede que lo actualice, puede que no. Nextel no está, ya nadie lo usa pero igual luego lo pongo.
