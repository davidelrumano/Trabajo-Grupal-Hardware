# Sistema de Copias de Seguridad Automatizadas Multicapa

## 1\. Arquitectura General del Sistema

🔹 **Actividad**: Haz un esquema explicando los **tres niveles** del sistema de backups. Puedes incluir un diagrama en ASCII o hacer el digrama en https://excalidraw.com/

**Guía de investigación**:

* **¿Qué rol cumple cada nivel?**

**1\. Backup Primario / Locales \- Permite el acceso rápido y una recuperación de datos inmediata**

* Es el más común cuando se trata de pérdidas de datos accidentales.   
* Una de sus características es que permite restauraciones rápidas sin depender de la conectividad externa.   
* Es ideal en áreas de trabajo y para corregir errores de manera rápida. 

**2\. Backup Secundario / Externos \- Para respaldos contra desastres físicos y fallos graves**

* Este backup es común por proteger contra accidentes como incendios, robos o fallos en el sistema (hardware),   
* A su vez permite que los datos se recuperen en caso de que el almacenamiento primario falle.  
* Normalmente está cifrado y replicado para una mayor seguridad y respaldo contra amenazas. 

**3\. Backup Terciario / Fuera de línea \- Para una mayor seguridad y una recuperación de datos a largo plazo.** 

* Protege contra ataques como cibernéticos, corrupción de datos y ransomware.   
* Es idóneo para almacenar datos a largo plazo y cumplimiento de la normativa.   
* Por otro lado, es perfecto para datos críticos los cuales no deben de alterarse con frecuencia. 

—-------------------------------------------------------------------------------------------------------------------------

* **¿Qué tipo de dispositivos hay en cada uno?**

  Dispositivos Utilizados  
* Backup Primario / Locales:  
  * Discos duros internos y externos  
  * SSD  
  * Sistemas RAID / arrays de almacenamiento  
  * NAS locales  
* Backup Secundario / Externos:  
  * Servidores de respaldo remotos  
  * Sistemas NAS/SAN externos  
  * Soluciones en la nube  
* Backup Terciario / Fuera de línea:  
  * Cintas magnéticas  
  * Discos ópticos (DVD, Blu-ray)  
  * Dispositivos de almacenamiento externos que se mantienen desconectados

  [https://www.tecnozero.com/copia-de-seguridad/tipos-de-copias-de-seguridad-cual-elegimos/](https://www.tecnozero.com/copia-de-seguridad/tipos-de-copias-de-seguridad-cual-elegimos/)

  [https://www.purestorage.com/es/knowledge/primary-vs-secondary-storage.html](https://www.purestorage.com/es/knowledge/primary-vs-secondary-storage.html)

  [https://es.wikipedia.org/wiki/Tipos\_de\_almacenamientos\_primarios](https://es.wikipedia.org/wiki/Tipos_de_almacenamientos_primarios)


  

*(Explica brevemente la función de cada nivel. Puedes añadir un esquema o diagrama ASCII si lo deseas.)*

---

## 2\. Configuración del Nivel 1: PCs Individuales

### a. Selección de software

🔹 **Actividad**: Investiga y selecciona un software de backup para:

* Windows

* macOS

* Linux

* **¿Qué opciones gratuitas existen?**

* **¿Qué ventajas tiene cada una?**

\- A la hora de buscar los software de backups, para los sistemas nombrados, opte por hacer un tier list de cada uno de los SO y sus software de backups, agregando los gratis, y las ventajas que posee cada uno. 

**WINDOWS** 

**Tier S (Softwares más completos y seguros) :** 

* **Acronis Cyber Protect Home Office** \- Es perfecto contra ataques de ransomware, tenemos la posibilidad de almacenar en la nube y destaca por una recuperación de datos rápida.   
* **MacriumReflect** \- Tenemos la posibilidad de clonar discos, recuperación de datos rápida y opciones avanzadas a la hora de hacer los backups.   
* **Veeam Backup and Replication** \- Este software es perfecto para usarse en ámbitos de virtualización, y con alta eficiencia a la hora de recuperar datos. 

**Tier A (Muy buenas opciones, pero con algunas limitaciones) :** 

* **EaseUS Todo Backup** \- Tiene una interfaz muy intuitiva a la hora de usarse, tenemos la opción de respaldo de datos en la nube y es sencillo realizar la recuperación de datos.   
* **R-Drive Image** \- Es perfecto a la hora de realizar copias de seguridad completas, también a la hora de recuperación de datos contra desastres.   
* **Backblaze** \- Este software destaca ya que poseemos almacenamiento ilimitado en la nube sumándole que poseemos un respaldo automático. 

**Tier B (Buenas opciones, pero menos opciones avanzadas) :** 

* **AOMEI Backupper (Opción Gratuita)** \- Es uno de las mejores opciones gratuitas para Windows, es un software intuitivo y fácil de usar, el problema es que posee herramientas muy básicas.   
* **Cobian Backup (Opción Gratuita)** \- Es un software ligero y perfecto si queremos realizar backups programados, una de sus cosas destacables es que no requiere de un consumo excesivo de recursos.   
* **Carbonite** \- Puede realizar backups automáticos o en la nube con una recuperación sencilla y básica. 

**Tier C (Opciones muy básicas y con muchas limitaciones) :** 

* **Windows Backup** \- Se trata de la función que trae Windows integrada con el sistema dentro de la configuración de este, simple y no trae muchas opciones avanzadas.   
* **FBackup (Opción Gratuita)** \- Es un software de backups simple para realizar copias de seguridad automáticas. Es perfecta para usuarios que son nuevos o prefieren usar las funcionalidades básicas. 

\- En caso de Windows, las más recomendables de usar y que son gratuitas son AOMEI Backupper y Cobian Backup. Son sencillas de usar y muy intuitivas, lo malo es que no posee almacenamiento en la nube y puede que por las funciones básicas tengan sus limitaciones. 

[https://www.pcworld.com/article/407021/best-windows-backup-software.html](https://www.pcworld.com/article/407021/best-windows-backup-software.html)

[https://thectoclub.com/tools/best-backup-software/](https://thectoclub.com/tools/best-backup-software/)

[https://beebom.com/best-backup-software/](https://beebom.com/best-backup-software/)

[https://geekflare.com/es/best-backup-software/](https://geekflare.com/es/best-backup-software/)

[https://es.easeus.com/backup-recovery/mejores-programas-copia-de-seguridad-gratis.html](https://es.easeus.com/backup-recovery/mejores-programas-copia-de-seguridad-gratis.html)

[https://www.datanumen.com/es/Blogs/11-mejores-herramientas-de-software-de-respaldo-gratuitas/](https://www.datanumen.com/es/Blogs/11-mejores-herramientas-de-software-de-respaldo-gratuitas/)

—-------------------------------------------------------------------------------------------------------------------------

**MacOS**

**Tier S (Poseen muchas funciones y son los más completos y confiables) :** 

* **Time Machine (Opción Gratuita)** \- Es la opción que posee el sistema por defecto integrada en él, puede realizar copias automáticas y posee una recuperación de datos sencilla.   
* **Carbon Copy Cloner** \- Posee opciones como la clonación de discos y una recuperación de datos rápida y sencilla.   
* **ChronoSync** \- Además de agregar que posee una recuperación de datos rápida y sencilla, nos permite una sincronización avanzada y completa y tenemos la posibilidad de respaldar los datos en múltiples dispositivos. 

**Tier A (Muy buenos softwares, pero con menos opciones avanzadas) :** 

* **Get Backup Pro** \- Es perfecto si queremos hacer copias de seguridad incrementales, agregando que posee una encriptación de los datos avanzada y muy detallada.   
* **Acronis Cyber Protect Home Office** \- Esta opción sirve tanto como para sistemas Windows y MacOS. Como he mencionado es perfecto para la protección contra ransomware y el almacenamiento en la nube.   
* **SuperDuper\!** \- Lo más destacable de este software es que nos permite clonar discos de manera avanzada y a su vez posee opciones de automatización. 

**Tier B (Perfectos para realizar una funcion basica) :** 

* **EaseUS Todo Backup para Mac** \- Es un software sencillo de usar con opciones muy básicas y posee respaldo en la nube a la hora de realizar las copias de seguridad.   
* **Disk Drill (Opción Gratuita)** \- Es muy simple, intuitiva y con opciones muy básicas, lo más destacable, es que nos permite crear imágenes de disco para la recuperación de datos. 

\- En el caso de los sistemas MacOS, si buscamos una opción gratuita, las más recomendable es Time Machine, que es la que posee el sistema por defecto, es sencilla y posee muchas funciones. Si buscamos algo más avanzado lo mejor es Carbon Copy Cloner y ChronoSync, ya que ambas, aparte de que son sencillas de usar, poseen funciones como, la clonación de discos o la posibilidad de respaldar los datos en diferentes dispositivos. 

[https://www.easeus.com/mac-backup-recovery/best-backup-software-for-mac.html](https://www.easeus.com/mac-backup-recovery/best-backup-software-for-mac.html)

[https://www.igeeksblog.com/best-mac-backup-software/](https://www.igeeksblog.com/best-mac-backup-software/)

[https://news.macgasm.net/reviews/best-backup-software-mac/](https://news.macgasm.net/reviews/best-backup-software-mac/)

[https://www.softwarehow.com/best-mac-backup-software/](https://www.softwarehow.com/best-mac-backup-software/)

—-------------------------------------------------------------------------------------------------------------------------

**Linux** 

**Tier S (Los softwares más completos y con diferentes funcionalidades) :** 

* **BorgBackup (Opción Gratuita)** \- Software básico y con diferentes funcionalidades, como que posee duplicación y un buen cifrado de datos.   
* **Restic (Opción Gratuita)** \- Software rápido en cuanto a la recuperación de datos, muy seguro y es compatible con diferentes plataformas y sistemas operativos.  
* **Duplicati (Opción Gratuita)** \- Software de backup simple, pero posee diferentes funciones avanzadas de cifrado y posee un gran almacenamiento en la nube. 

**Tier A (Muy buenos, pero poseen limitaciones) :** 

* **Timeshift (Opción Gratuita)** \- Un software simple pero destaca en que es ideal para snapshots del sistema y posee una recuperación rápida.   
* **Amanda (Opción Gratuita)** \- De nuevo un software simple, solo que posee una función destacable la cual permite una solución rápida y avanzada para los backups en red.   
* **CloudBerry Backup** \- Otro software simple de backups, con una función más destacable que permite la compatibilidad con múltiples servicios en la nube, lo cual puede ser beneficioso para nosotros. 

**Tier B (Softwares simples y gratuitos) :** 

* **Deja Dup (Opción Gratuita) \-** Software simple y sencillo de usar, agregando a esto que posee una interfaz intuitiva y sencilla con integración en GNOME.   
* **UrBackup (Opción Gratuita) \-** De nuevo otro software simple con funcionalidades básicas, lo más destacable de este es que posee una restauración rápida de los backups en red.   
* **Kopia (Opción Gratuita) \-** Uno de los softwares gratis para realizar backups que posee almacenamiento en la nube, lo cual es algo destacable. Incluyendo que es sencillo de usar e intuitivo, para usuarios que son nuevos o tienen poca experiencia. 

\- En cuanto a las opciones gratuitas las mejores en mi opinión son BorgBackup y Restic, debido a las diferentes funcionalidades como la duplicación de datos o las opciones avanzadas en cuanto al cifrado, agregando que Restic es compatible en diferentes plataformas. En cuanto a algo más avanzado lo más recomendable es CloudBerry Backup, ya que aunque sea un software simple, la compatibilidad con múltiples servicios en la nube es algo que suma. 

[https://www.tecmint.com/linux-system-backup-tools/](https://www.tecmint.com/linux-system-backup-tools/)

*(Explica por qué has elegido cada uno.)*

—-------------------------------------------------------------------------------------------------------------------------

### b. Programación de copias

- ¿Cómo se configuran las copias incrementales diarias?  
- ¿Cómo se hacen las copias completas semanales?  
    
  **1\. Configuración de Copias Incrementales Diarias**

Las copias incrementales se encargan de respaldar únicamente los cambios realizados desde el último backup (ya sea completo o incremental). Para configurarlas:

* **Preparar una base sólida:** Antes de comenzar el ciclo incremental, realiza una copia completa (o respaldo total) que actuará como referencia. Esta copia base se realiza al inicio de la semana.

* **Automatización diaria:** Programa un trabajo (por ejemplo, mediante un cron job en Linux o el Programador de tareas en Windows, o usando un software especializado) para que, cada día, se ejecute un backup incremental.

  * El proceso detecta y respalda solo los archivos modificados, añadidos o eliminados desde el último backup.

  * Configura el horario en un periodo de baja actividad para minimizar el impacto en el rendimiento.

* **Ventajas de las incrementales:** Al copiar solo lo que ha cambiado, se reduce el tiempo de realización del backup y el espacio de almacenamiento necesario.

  **2\. Configuración de Copias Completas Semanales**

Las copias completas se realizan de forma periódica para capturar el estado íntegro de la información, reiniciando la cadena de incrementos. Para establecerlas:

* **Programación fija semanal:** Selecciona un día concreto de la semana (por ejemplo, el domingo o en un horario nocturno de fin de semana) para ejecutar el backup completo.

  * Este proceso copia todos los datos, independientemente de si han cambiado o no, creando un nuevo punto de partida para los backups incrementales de la siguiente semana.

* **Integración con las incrementales:** La copia completa actuará como base para las copias incrementales diarias posteriores. En caso de restauración, el proceso consistirá en aplicar primero el backup completo y luego las incrementales correspondientes para reconstruir el sistema hasta el día deseado.

* **Automatización:** De igual forma que las incrementales, se puede automatizar el backup completo usando las herramientas de backup del sistema o software especializado, programando para que se ejecute automáticamente en la franja horaria determinada.

  **Resumen del Proceso**

1. **Inicio de la semana:**

   * Ejecutar una copia completa, que servirá como base.

2. **Durante la semana:**

   * Cada día, ejecutar una copia incremental que almacene sólo los cambios desde el último respaldo (incremental o completo).

3. **Ciclo de respaldo:** 

   * Al llegar al día programado para la copia completa, se reinicia la cadena de backups, facilitando la restauración y evitando que se acumulen demasiados incrementales.

Esta estrategia ofrece un equilibrio entre eficiencia (menos tiempo y espacio para respaldos diarios con incrementales) y seguridad (al contar con copias completas periódicas que reinician la cadena de cambios).

[https://www.tecnozero.com/copia-de-seguridad/tipos-de-copias-de-seguridad-cual-elegimos/](https://www.tecnozero.com/copia-de-seguridad/tipos-de-copias-de-seguridad-cual-elegimos/)

[https://aodatacloud.es/blog/tipos-de-copias-de-seguridad/](https://aodatacloud.es/blog/tipos-de-copias-de-seguridad/)

[https://www.acronis.com/es-es/blog/posts/incremental-differential-backups/](https://www.acronis.com/es-es/blog/posts/incremental-differential-backups/)

### c. Destino de las copias  

- ¿Dónde se almacenan?  
- ¿Cómo se organizan las carpetas por PC?


Cuando se realiza una copia de seguridad en un PC, el destino puede variar dependiendo del método utilizado. Aquí tienes algunos escenarios comunes:

1. **Copias en almacenamiento local**  
     
   * Se pueden guardar en discos duros internos, externos o en unidades USB.  
       
   * Suelen almacenarse en carpetas específicas dentro del sistema, como "Documentos", "Imágenes" o una carpeta personalizada.  
       
2. **Copias en la nube**  
     
   * Servicios como OneDrive, Google Drive o Dropbox permiten almacenar archivos de forma segura.  
       
   * La organización depende del usuario; puedes crear carpetas personalizadas para clasificar tus copias.  
       
3. **Copias automáticas del sistema**  
     
   * Windows tiene herramientas como "Historial de archivos" o "Copia de seguridad y restauración", que guardan versiones periódicas de los archivos.  
       
   * Suelen ubicarse en la unidad de recuperación o en el disco configurado para la copia de seguridad.

### **Organización de las carpetas en un PC**

El sistema de archivos organiza carpetas siguiendo una jerarquía:

* **Disco principal (C: o D:)** → Carpetas raíz como "Usuarios", "Archivos de programa", "Windows".  
    
* **Carpeta de usuario** → Contiene "Escritorio", "Documentos", "Descargas", etc.  
    
* **Subcarpetas personalizadas** → Puedes crear categorías dentro de cada área según tus necesidades.  
    
  [https://support.microsoft.com/es-es/windows/realizar-copias-de-seguridad-y-restaurar-con-copias-de-seguridad-de-windows-87a81f8a-78fa-456e-b521-ac0560e32338](https://support.microsoft.com/es-es/windows/realizar-copias-de-seguridad-y-restaurar-con-copias-de-seguridad-de-windows-87a81f8a-78fa-456e-b521-ac0560e32338)   
    
  [https://www.xataka.com/basics/copias-seguridad-windows-11-que-sirven-que-tipos-hay-como-se-hacen](https://www.xataka.com/basics/copias-seguridad-windows-11-que-sirven-que-tipos-hay-como-se-hacen)   
    
  [https://www.kingston.com/es/blog/personal-storage/computer-backup-tips](https://www.kingston.com/es/blog/personal-storage/computer-backup-tips) 

---

## 3\. Configuración del Nivel 2: Servidor Local Primario

#### **a. Hardware**

🔹 **Actividad**: Elige una de estas opciones e investiga precios y características:

* NAS (marca/modelo)

* Ordenador con Linux/Windows

  **NAS** 

**\- ¿ Cuál es la función principal de un NAS ?** 

\- Un NAS es un dispositivo de almacenamiento conectado a la red, el cual nos permite guardar, compartir y acceder a los diversos archivos que tengamos guardados en él desde múltiples y diferentes dispositivos, sin la necesidad de tener que contratar o tener un servicio en la nube.

**\- Funciones principales de este :**  

**\- Almacenamiento centralizado :** El NAS actúa como servidor de archivos donde podemos acceder a él desde cualquier dispositivo o desde una red. 

**\- Copias de seguridad automáticas :** Tenemos la posibilidad de elaborar backups programados de los diferentes ordenadores u otros dispositivos de la empresa o compañía. 

**\- Nube privada :** Funciona como una similitud al almacenamiento en la nube, solo que aquí tenemos control total sobre los datos. 

**\- Servidor multimedia :** Con él podemos enviar fotos, videos, películas, etc … a dispositivos como móviles o televisores. 

**\- Acceso remoto :** De los más destacable de este es que podemos acceder a los archivos desde cualquier lugar, siempre y cuando tengamos conexión a internet. 

**\- Seguridad y privacidad :** Podemos gestionar las opciones para ver los accesos a este y tener la capacidad de cifrar los datos. 

**\- Lista comparativa entre precios/marcas/y calidad de estos.** 

**1\. Synology DiskStation DS224+**

**Precio** : 545 € 

**Características destacables** : 2 bahías, almacenamiento centralizado y herramientas de copias de seguridad avanzadas. 

**Opinión** : Es una opción ideal para la gente que lo quiere para el hogar, o directamente para empresas pequeñas, incluyendo que tiene una interfaz muy intuitiva. 

**2\. TERRAMASTERF8 NAS** 

**Precio** : Variable dependiendo de lo que queramos (hasta 64 TB)

**Características destacables** : 8 bahías SSD M.2 NvMe, procesador de 4 núcleos y protección contra ransomware. 

**Opinión** : Puede tener un almacenamiento muy grande y como se puede ver el propio NAS ofrece un rendimiento muy alto, considero que es de uso exclusivo para usuarios que sean avanzados. 

**3\. Synology DS223**

**Precio** : Aproximadamente 219 €

**Características destacables** : 2 bahías, procesador Realtek de 4 núcleos, capacidad de hasta 36 TB.

**Opinión** : En cuanto al NAS, es de lo mejor en cuanto a relación calidad \- precio, para un almacenamiento eficiente. 

**4\. TERRAMASTER NAS F2-424**

**Precio** : Variable segun lo que queramos 

**Características destacables** : 2 bahías, memoria DDR5 de 8 GB, procesador N95 de cuatro núcleos. 

**Opinión** : Ofrece un buen rendimiento y a su vez muchas opciones avanzadas en el ámbito de copias de seguridad. 

**5\. Netgear NAS RR3312G6-1000S**

**Precio** : De nuevo variable dependiendo de lo que elijamos (hasta 120 TB).

**Características destacables** : 12 bahías, procesador Intel Xeon y una protección continua de datos. 

**Opinión** : Es perfecto para empresas que necesitan almacenar grandes cantidades de datos y a su vez requieren de una gran seguridad. 

[**https://www.mejoraelige.es/servidor-nas/**](https://www.mejoraelige.es/servidor-nas/)

[**https://www.profesionalreview.com/mejores-nas-del-mercado/**](https://www.profesionalreview.com/mejores-nas-del-mercado/)

—-------------------------------------------------------------------------------------------------------------------------

### b. Tipo de RAID

- Elegido: RAID 1 / RAID 5 / RAID 10

- Justificación:


  ### **Opciones de RAID**

* **RAID 1:**

  * **Dispositivos:** Dos discos en espejo.

  * **Justificación:** Es la opción ideal para NAS de 2 bahías (como el Synology DS224+ o DS223). Duplica los datos entre ambos discos, ofreciendo alta redundancia y una recuperación rápida en caso de fallo de uno de ellos. La principal limitación es que se utiliza solo el 50% de la capacidad total de los discos.

* **RAID 5:**

  * **Dispositivos:** Mínimo tres discos, en los que los datos se distribuyen y se reserva el equivalente a un disco para la paridad.

  * **Justificación:** Es una excelente opción si se dispone de un NAS con más de dos bahías (por ejemplo, un dispositivo de 4 u 8 bahías). Ofrece un equilibrio entre seguridad y eficiencia en el uso de la capacidad, ya que solo se utiliza una parte del total para la paridad. La desventaja es que, si un disco falla, el proceso de reconstrucción puede ser más lento.

* **RAID 10:**

  * **Dispositivos:** Al menos cuatro discos, combinando la duplicación de RAID 1 con la distribución de datos de RAID 0\.

  * **Justificación:** Es la opción adecuada para entornos en los que se requiere alta velocidad en lectura y escritura sin sacrificar la redundancia. RAID 10 combina lo mejor del mirroring y del striping, pero supone una mayor inversión de hardware, ya que la capacidad efectiva es la mitad de la suma total de discos.

  ### **Conclusión y Elección**

La elección dependerá de la infraestructura y las necesidades del entorno:

* Si se cuenta con un NAS de 2 bahías, la solución natural es RAID 1, ya que garantiza una recuperación inmediata en caso de fallo con un costo moderado y sin requerir más hardware.

* Si se dispone de un NAS con 3 o más bahías y se busca un equilibrio entre capacidad y redundancia, RAID 5 es una opción eficaz, maximizando el espacio utilizable.

* Si además de la redundancia se requiere un rendimiento superior para operaciones intensivas, y se tiene la posibilidad de invertir en al menos 4 discos, RAID 10 ofrece la mejor combinación de velocidad y seguridad, aunque a costa de duplicar la inversión en almacenamiento.

  [https://ventajas.org/tipos-de-raid-ventajas-y-desventajas/](https://ventajas.org/tipos-de-raid-ventajas-y-desventajas/)

  [https://www.smythsys.es/11948/que-tipos-de-raid-hay-ventajas-y-desventajas/](https://www.smythsys.es/11948/que-tipos-de-raid-hay-ventajas-y-desventajas/)


  


### c. Software de gestión 

- Software elegido: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_  
- Función principal: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

### **Odoo: Software de Gestión Empresarial**

Odoo es un sistema de gestión empresarial (ERP) modular y de código abierto que permite a las empresas administrar todas sus operaciones desde un único lugar2. Fue creado en 2005 por Fabien Pinckaers y ha evolucionado hasta convertirse en una de las plataformas ERP más completas del mercado.

### **Función Principal**

Odoo integra múltiples áreas de gestión en una sola plataforma, permitiendo a las empresas optimizar sus procesos y mejorar la eficiencia operativa. Sus principales funciones incluyen:

* **Gestión de ventas:** Creación de cotizaciones, facturación y seguimiento de pedidos.  
    
* **Contabilidad y finanzas:** Control de ingresos, gastos y generación de informes financieros.  
    
* **Gestión de inventarios:** Seguimiento de existencias y optimización del almacén  
    
* **Recursos humanos:** Administración de empleados, nóminas y ausencias.  
    
* **Marketing:** Automatización de campañas y gestión de redes sociales.  
    
  [https://duonex.com/2023/03/27/para-que-sirve-odoo/](https://duonex.com/2023/03/27/para-que-sirve-odoo/)   
    
  [https://imaginaformacion.com/tutoriales/odoo-sistema-de-gestion-erp](https://imaginaformacion.com/tutoriales/odoo-sistema-de-gestion-erp)   
    
  [https://www.qubiq.es/blog/manuales-odoo-1/que-es-odoo-y-para-que-sirve-160](https://www.qubiq.es/blog/manuales-odoo-1/que-es-odoo-y-para-que-sirve-160) 

---

## 4\. Configuración del Nivel 3: Servidor Secundario Remoto

#### **a. Opción de servidor remoto**

🔹 **Actividad**: Elige una de estas opciones y justifica:

* NAS en otra ubicación

* Nube (Google Cloud, Azure, AWS)

* Ordenador remoto

\- Dependiendo de las prioridades que tengamos seleccionaremos una opción u otra, en casos de seguridad, accesibilidad y demás, la opción más cómoda y recomendable seria la nube. 

\- En cuanto a por qué elegir la nube algunas de las características más destacables son : 

* **Alta seguridad :** Protección con cifrado bastante avanzada, junto a la autenticación y redundancia de datos.   
* **Acceso remoto desde cualquier lugar :** No requieres de ningún equipo físico en una ubicación específica.   
* **Escalabilidad :** Puedes contratar o pagar por más almacenamiento en función del cuanto sea necesario.   
* **Menos mantenimiento :** No existe la necesidad de gestionar un mantenimiento en dispositivos físicos, por lo cual es más cómodo. 

\- Por lo cual elegiría el almacenamiento en la nube debido a la seguridad que nos proporcionan las grandes empresas y sin tener la necesidad de estar pendientes de si requiere un mantenimiento como pueden ser los dispositivos como los NAS. 

\- En cambio, si requieres de una privacidad extrema y un control total de toda la información es recomendable un NAS. En cambio un ordenador remoto es más económico que cualquiera de las otras opciones a largo plazo , pero menos fiable. 

—-------------------------------------------------------------------------------------------------------------------------

### b. Seguridad de la sincronización

- ¿Cómo se programa la sincronización?

- ¿Qué cifrado se usa?

- ¿Se puede activar doble autenticación?

**¿Cómo se programa la sincronización?** La sincronización se programa configurando tareas automáticas en el sistema. En los dispositivos NAS y servidores, se utilizan herramientas integradas como el programador de tareas (por ejemplo, mediante cron en sistemas Linux o el planificador en el sistema operativo del NAS, como DSM en Synology) para definir intervalos específicos (diario, semanal, etc.) en los que se inician las operaciones de sincronización. Esto permite que la transferencia y respaldo de datos se realice en momentos óptimos (normalmente en periodos de baja actividad) y de forma continua sin intervención manual.

**¿Qué cifrado se usa?** Generalmente, se emplea el cifrado AES (Advanced Encryption Standard), habitualmente en su versión de 256 bits. Este cifrado es robusto y se utiliza tanto para proteger los datos durante la transmisión (mediante protocolos seguros como SSL/TLS) como para cifrar la información almacenada en el dispositivo. Esto garantiza que los datos permanezcan seguros y protegidos ante accesos no autorizados.

**¿Se puede activar doble autenticación?** Sí, la mayoría de los sistemas modernos, especialmente en dispositivos NAS como Synology o QNAP, permiten habilitar la autenticación de dos factores (2FA). Esto añade una capa extra de seguridad, ya que para acceder a la configuración o a la interfaz de gestión del sistema se requiere, además del usuario y contraseña, un código temporal generado por una aplicación móvil (por ejemplo, Synology Secure SignIn o Google Authenticator). De esta forma, incluso si se comprometa la contraseña, se dificulta el acceso sin el segundo factor.

[https://kb.synology.com/es-es/DSM/help/DSM/SecureSignIn/2factor\_authentication](https://kb.synology.com/es-es/DSM/help/DSM/SecureSignIn/2factor_authentication)

---

## 5\. Automatización del Proceso

- Script de verificación: *(pega o enlaza un ejemplo)*  
    
  *\#\!/bin/bash*  
  *\# Script de verificación para el proceso de backup*  
    
  *\# Variables de configuración*  
  *SOURCE\_DIR="/home/usuario/datos"        \# Directorio que se va a respaldar*  
  *BACKUP\_DIR="/home/usuario/backups"        \# Directorio donde se guardarán los backups*  
  *LOG\_FILE="/home/usuario/backup.log"       \# Archivo de log para registrar el proceso*  
  *TIMESTAMP=$(date \+"%Y%m%d-%H%M%S")*  
  *BACKUP\_FILE="backup-${TIMESTAMP}.tar.gz"  \# Nombre del archivo de backup*  
    
  *\# Iniciar el proceso de backup*  
  *echo "\[$(date)\]: Iniciando el backup de ${SOURCE\_DIR}" \>\> "${LOG\_FILE}"*  
  *tar \-czf "${BACKUP\_DIR}/${BACKUP\_FILE}" "${SOURCE\_DIR}"*  
    
  *\# Verificar si el backup se realizó correctamente*  
  *if \[ $? \-eq 0 \]; then*  
      *echo "\[$(date)\]: Backup creado exitosamente: ${BACKUP\_FILE}" \>\> "${LOG\_FILE}"*  
      *\# Calcular y registrar el checksum (opcional)*  
      *CHECKSUM=$(sha256sum "${BACKUP\_DIR}/${BACKUP\_FILE}" | awk '{print $1}')*  
      *echo "\[$(date)\]: Checksum del backup: ${CHECKSUM}" \>\> "${LOG\_FILE}"*  
  *else*  
      *echo "\[$(date)\]: Error: Falló la creación del backup." \>\> "${LOG\_FILE}"*  
  *fi*  
    
  *echo "\[$(date)\]: Proceso de backup finalizado." \>\> "${LOG\_FILE}"*  
    
    
- Alerta por email: ¿Cómo se configura?  
    
  **Acceder al Panel de Control:** Inicia sesión en la interfaz de administración de tu NAS y dirígete al "Panel de control".  
  **Ir a la sección de Notificaciones:** Busca la opción “Notificación” o “Correo electrónico” en el menú. En Synology, por ejemplo, esto se encuentra en el Panel de Control, dentro de "Notificación".  
  **Configurar el Remitente del Correo:**  
* Selecciona o crea un perfil de correo electrónico, indicando la dirección desde la cual se enviarán las alertas.  
* Elige un proveedor preconfigurado (como Gmail, Outlook, etc.) o configura un servidor SMTP personalizado.  
* Introduce la dirección del servidor SMTP (p. ej. `smtp.gmail.com` para Gmail o `smtp-mail.outlook.com` para Outlook), el puerto (usualmente 587 para conexión segura), y activa la opción de usar SSL/TLS si es necesario.  
* Ingresa el nombre de usuario y la contraseña correspondientes a la cuenta de correo.  
  **Definir los Destinatarios y Reglas de Alerta:**  
* Especifica las direcciones de correo electrónico a las que deseas que se envíen las notificaciones.  
* Configura las reglas o eventos que activarán el envío de alertas (por ejemplo, fallos del sistema, advertencias de hardware, etc.).  
  **Realizar una Prueba:** Utiliza la opción de “Enviar un correo electrónico de prueba” para confirmar que la configuración es correcta y que los correos llegan a los destinatarios.  
  **Guardar la Configuración:** Una vez verificados los datos, guarda la configuración para que el sistema empiece a enviar alertas automáticamente.  
  [https://kb.synology.com/es-es/DSM/help/DSM/AdminCenter/system\_notification\_email](https://kb.synology.com/es-es/DSM/help/DSM/AdminCenter/system_notification_email)  
    
    
- Prueba de restauración: ¿Cada cuánto tiempo? ¿Cómo?  

**¿Cada cuánto tiempo?** Las pruebas de restauración son fundamentales para asegurarte de que tus copias de seguridad son confiables. La frecuencia recomendada depende de la criticidad de los datos y de los cambios en el entorno, pero en general se sugiere:

* **Ciclos regulares:** Realizar pruebas de restauración de manera programada, idealmente de manera mensual. En entornos menos críticos, puede aceptarse una prueba trimestral, pero en ambientes donde la pérdida de datos implica altos costos o riesgos, lo más seguro es hacerlo mensualmente o incluso tras cada backup completo importante.  
* **Tras cambios significativos:** Cada vez que se aplique una actualización importante en el sistema, se instalen nuevas aplicaciones o se modifiquen configuraciones relevantes, se recomienda efectuar una prueba de restauración para validar que la nueva configuración y los datos se pueden recuperar correctamente sin contratiempos.

**¿Cómo se realiza?** El proceso de prueba de restauración puede llevarse a cabo siguiendo estos pasos prácticos:

1. **Seleccionar un entorno de pruebas o “sandbox”:** Utiliza una máquina virtual o un servidor de ensayo que imite lo más fielmente posible el entorno de producción. Esto evita interferir con los sistemas en operación.  
2. **Escoger una copia de seguridad reciente:** Selecciona uno de tus backups completos o incrementales, según el plan establecido.  
3. **Ejecutar la restauración:** Utiliza el software o la herramienta de backup para iniciar el proceso de restauración en el entorno de pruebas. Asegúrate de seguir las mismas rutas y configuraciones que usarías en una restauración real.  
4. **Verificar la integridad de los datos:** Una vez finalizada la restauración, revisa que los archivos, bases de datos, y aplicaciones funcionen correctamente. Esto puede incluir la ejecución de scripts de validación o la verificación manual de la consistencia de la información.  
5. **Documentar y analizar:** Registra el tiempo que ha tardado el proceso de restauración, cualquier error o anomalía encontrada, y realiza un análisis para ajustar el proceso y optimizarlo en futuras pruebas.  
   [https://docs.aws.amazon.com/es\_es/aws-backup/latest/devguide/restore-testing.html](https://docs.aws.amazon.com/es_es/aws-backup/latest/devguide/restore-testing.html)  
   [https://www.baculasystems.com/es/el-blog/prueba-de-recuperacion-de-copias-de-seguridad/](https://www.baculasystems.com/es/el-blog/prueba-de-recuperacion-de-copias-de-seguridad/)  
   [https://www.datanumen.com/es/blogs/a-menudo-verifica-las-copias-de-seguridad-de-datos/](https://www.datanumen.com/es/blogs/a-menudo-verifica-las-copias-de-seguridad-de-datos/)  
   

---

## 6\. Justificación del uso de RAID

- ¿Por qué no sustituye al backup?  
- ¿Qué pasa si solo tenemos RAID?

**¿Por qué RAID no sustituye al backup?**

* **Protección limitada:** RAID (Redundant Array of Independent Disks) se diseña para ofrecer redundancia en el hardware, es decir, para minimizar el tiempo de inactividad tras fallos físicos de discos individuales. Sin embargo, no protege contra la corrupción de datos, errores humanos (como la eliminación accidental) o ataques cibernéticos, ya que estos errores se reproducen en todos los discos del arreglo .  
* **Falta de versiones históricas:** Un sistema RAID refleja en tiempo real el estado de los datos. Esto significa que si se sobreescribe o corrompen los archivos, la "redundancia" garantiza que todos los discos muestran el error. Por el contrario, una estrategia de backup permite almacenar versiones históricas, de modo que puedas restaurar datos en un estado anterior, aun cuando el origen se vea afectado.  
* **Protección ante desastres:** RAID se encuentra normalmente instalado en la misma ubicación física, por lo que en caso de desastres (incendios, inundaciones, robos) que afecten el centro de datos, todos los discos del RAID pueden resultar perdidos o dañados. Los backups, generalmente almacenados en sitios distintos o en la nube, están diseñados para recuperarse en estos escenarios.

**¿Qué pasa si solo tenemos RAID?**

Si en una infraestructura se utiliza únicamente RAID sin realizar copias de seguridad adicionales se expone a riesgos significativos:

* **Pérdida de datos críticos:** Un error o una acción no intencionada (como la eliminación o la sobrescritura de archivos) se replicará instantáneamente en todo el sistema RAID, resultando en la pérdida de información crítica sin posibilidad de recuperación.  
* **Impacto en la integridad de la información:** Aunque RAID puede manejar la falla de un disco físico, no puede restaurar datos si son afectados por un problema lógico (como la corrupción causada por malware o fallas en el software). La ausencia de versiones previas implica que no existen "copias históricas" para recuperar la versión correcta de los datos.  
* **Falta de resiliencia global:** Solo depender de RAID significa no cumplir con los principios de una buena estrategia de seguridad de datos, la cual debe incluir también backup externo, permitiendo restaurar el sistema tras incidentes que un RAID por sí solo no puede solventar.

[https://www.diskinternals.com/raid-recovery/raid-is-not-backup/](https://www.diskinternals.com/raid-recovery/raid-is-not-backup/)  
[https://www.langmeier-software.com/es/seiten/news/was-ist-der-unterschied-zwischen-raid-und-backup](https://www.langmeier-software.com/es/seiten/news/was-ist-der-unterschied-zwischen-raid-und-backup)  
[https://www.raidrecoveryservices.com/blog/raid-vs-backup/](https://www.raidrecoveryservices.com/blog/raid-vs-backup/)

---

## 7\. Resumen de Software Recomendado

| Función | Software Recomendado |
| :---- | :---- |
| Gestión centralizada | Microsoft ,SCCM,Ansible,Pupper |
| Sincronización entre servidores | Resilio Sync, Syncthing, Rsync |
| Monitorización | Zabbix, Nagios, Prometheus |



---

