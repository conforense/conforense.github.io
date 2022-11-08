---
title: "Ponencias 1 Day Con Forense 2022"
date: 2022-11-02T22:04:20+02:00
showSummary: false
featured: true
tags: ["ponentes", "CON Forense"]
draft: false
---


## Cómo preparar la ratificación judicial de una pericial informática

La idea es hablar primero de la preparación y acciones previas a la ratificación: revisión de tu informe, preparación de las preguntas con el letrado, etc...
Posteriormente, hablar el día de la ratificación: Planificación del viaje, control del estrés previo a la ratificación.

Seguidamente, afrontaríamos la declaración en sí: Orden de intervención en el juicio, orden de las preguntas de los letrados, tratamiento a cada persona, forma de responder a las preguntas y posiciónamiento del perito respecto a preguntas de la parte contraria.
Terminaríamos ya brevemente, con el seguimiento al caso tras la ratificación. 

La charla llevará 0% contenido técnico.

Por [Peritotec]({{< ref "/blog/ponentes-1-day-con-forense-2022#Peritotec" >}})

## Mi proveedor ha sido hackeado ¿Seguro?

Se trata de la presentación de un caso real. Un cliente nos llama porque un proveedor les reclama unos pagos que ellos ya han realizado. Quieren demostrar que un proveedor ha sido victima de un ataque informático, y que certifiquemos que las transferencias realizadas a dicho proveedor son correctas. Que son ellos los que tienen el problema. Nos aportan una serie de correos electrónicos, facturas y comprobantes bancarios.

Tras analizar las cabeceras de dichos correos se detecta una suplantación de cuentas de correo (mail spoofing), sufrida no por el proveedor sino por nuestro cliente. El caso se convierte en una variante de la Estafa del CEO. Mediante la suplantación de la cuenta de correo del proveedor se ha conseguido que se realicen una serie de transferencias bancarias (decenas de miles de euros) a cuentas controladas por el atacante. Tras demostrar lo sucedido y descargar de responsablidad al proveedor, comienza una investigación para analizar cómo se ha producido la suplantación.

Debido a las deficiencias técnológicas de nuestro cliente, sólo disponemos de logs de tráfico web posteriores a los hechos investigados (aparentemente sin interés para nuestra investigación). No disponemos de logs del servidor de correo ni de ningún tipo de log de las fechas relevantes. Aún con estas limitaciones y trás un análisis profundo de los logs disponibles. Se descubre que las comunicaciones por correo electrónico del cliente siguen siendo interceptadas por el atacante, aúnque las contraseñas de correo fueron cambiadas. Y que no sólo se intercepta la cuenta de correo usada para los pagos, sino todas las cuentas de correo del dominio de la empresa.

Finalmente la investigación demuestra que el vector de ataque es una vulnerabilidad en el software usado para el panel de control del hosting (CPanel), que permite el acceso total a todos los buzones de correo del dominio y que es necesario actualizar dicho software o cambiar a un software distinto.

El interés del caso radica en mostrar los giros de guión que se producen en una investigación, las limitaciones para investigar que se encuentra cualquier investigador forense en el día a día, y como unas evidencias inicialmente
catalogadas como irrelevantes sirven para resoverlo.

Por [Juan Torres Ibañez]({{< ref "/blog/ponentes-1-day-con-forense-2022#JuanTorresIbañez" >}})

## When Rust meets forensics

La charla girara entorno a https://lib.rs/crates/forensic-rs  y el potencial que tiene para poder automatizar la extracción de evidencias, encontrar anomalías y poder crear timelines de actividad de usuario de forma sencilla.

Por [Samuel Garces]({{< ref "/blog/ponentes-1-day-con-forense-2022#SamuelGarces" >}})

## Repadesastre en APK Downgrade

Se trabaja todo desde la terminal de ubuntu, no se usan máquinas virtuales, directamente se usa el teléfono físico visualizando con scrcpy en todo momento. El proceso APK downgrade es conocido y se introduce en alguna CON, pero no se expone al detalle como en esta presentación que tiene en cuenta todas las situaciones y como resolver problemas.

Por [Buenaventura Salcedo]({{< ref "/blog/ponentes-1-day-con-forense-2022#BuenaventuraSalcedo" >}})

## Para hacer el amor hay que venir al SU: Forensic & OSINT VS ransomware 

Ponencia realizada por Jorge Coronado de forma dinámica y práctica. La idea es enseñar como la ciencia de datos, OSINT y forense informático van de la mano para luchar contra el ransomware.

Muchos equipos en CSOC y HelpDesk deben justificar o investigar la procedencia de los ciberdelincuentes que realizan intrusiones e instalan ransomware. El objetivo de esta charla son:
1.  Listar los diferentes grupos de ransomware
2. Clasificarlos y ordenarlos
3. Analizar sus páginas web y grupos de Telegram
4. Realizar una investigación OSINT de un caso real donde encontramos a los autores

Por [Jorge Coronado]({{< ref "/blog/ponentes-1-day-con-forense-2022#JorgeCoronado" >}})