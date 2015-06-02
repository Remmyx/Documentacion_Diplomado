# Instalacion Debian 7 Wheezy 
## Soporte de virtualización
* Como la instalacion se realizará sobre un escenario virtual es importante verificar el soporte de virtualizacion del equipo (hardware - Bios).Ejecutar la siguiente instrución:
`grep vmx /proc/cpuinfo` 

remmy@remmy-pc:~$ sudo grep --color vmx /proc/cpuinfo 
[sudo] password for remmy: 
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm ida arat epb xsaveopt pln pts dtherm tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm ida arat epb xsaveopt pln pts dtherm tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm ida arat epb xsaveopt pln pts dtherm tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm ida arat epb xsaveopt pln pts dtherm tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms


## INSTALACION DEBIAN7.6.0 

1. Iniciar la instalación desde la unidad del DVD: Selecionar "Install". 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/00_pantalla_inicial.png)

2. Seleccón del idioma: "Español"
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/01_pantalla_idioma.png)

3. Selección de la Ubicacion: "Bolivia"
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/02_pantalla_ubicacion.png)

4. Selección de la distribución del teclado: "Latinoamericano" 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/03_pantalla_teclado.png)

5. Parametros para la configuración de Red: Nombre de Maquina 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/04_pantalla_nombre_maquina.png)

6. Parametros para la configuración de Red: Nombre de dominio 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/05_pantalla_nombre_dominio.png)

7. Parametros para la configuración de usuario: Clave de superusuario
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/06_pantalla_clave_root.png)

9. Parametros para configuracion de uauario: nombre de usuario 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/07_pantalla_Usuario.png)

10. Parametros para configuracion de uauario: nombre de usuario para la cuenta 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/07_pantalla_Usuario_01.png)

11. Parametros para configuracion de uauario: contraseña de usuario
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/07_pantalla_Usuario_02.png)

12. Inicio de la instalacion: avance 
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/08_pantalla_hora_red.png)

13. Particionado del Disco duro: Manual
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/09_pantalla_seleccion_hdd.png)

![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/09_pantalla_tipo_particionado.png)

13.1 Creamos una partición nueva primaria, considerar los siguientes puntos:
- Establecer tamaños de acuerdo a las recomendaciones del asistente
- El tipo de partición debe ser primero "primaria" y luego "Logica" 
- Elegir la ubicación de la nueva particion: principio o al final, dependiendo el tipo de funcionalidad al que se destine.

![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/10_pantalla_tipo_particion.png)
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/11_pantalla_particion_boot.png)
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/12_pantalla_particion_boot_lugar.png)
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/12_pantalla_particion_boot_lugar_01.png)

13.2 Tabla de particiones: una vez finalizado el particionamiento, muestra el estado. Posteriormente debemos continuar definiendo la particion de intercambio (swap), datos y raiz y por ultimo confirmamos los cambios realizados.
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/13_pantalla_otras_particiones.png)
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/14_pantalla_partiones_resumen.png)
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/15_pantalla_partiones_confirmaciones.png)

14.Instalacion del sistema base:
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/16_pantalla_proceso_instalacion.png)

14.1 Selección de Programas 
Seleccionar los programas a instalar:
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/21_pantalla_paquetees_a_instalar.png)
Elegimos "Debian Desktop enviroment", "SSH Server", "Laptop" y "Utilidades estandar del sistema" para montar un servidor con capacidad de administracion e instalación de maquinas virtuales.

Durante la instalacion el asistente preguntará si deseamos instalar el cargador de arranque GRUP en el registro principal de arranque, elegiremos la opción "Si" y finalemente la instalacion se completa yrecomienda extraer el disco de instalación para un reinicio del sistema.
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/23_pantalla_grub.png)
![Pantalla de Instalacion](Images/00_instalacion_Devian_Servidor/24_pantalla_finalizacion.png)


