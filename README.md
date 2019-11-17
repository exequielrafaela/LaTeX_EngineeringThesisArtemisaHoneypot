# LaTeX_EngineeringThesisArtemisaHoneypot

## UNIVERSIDAD BLAS PASCAL
###  Ingeniería en Telecomunicaciones

#### Trabajo Final de Carrera

### Implementación, evaluación y desarrollos funcionales sobre Artemisa (Open Source back-end honeypot)

<div align="left">
  <img src="https://raw.githubusercontent.com/exequielrafaela/LaTeX_EngineeringThesisArtemisaHoneypot/master/Figuras/Fig9.jpg" alt="artemisa-honeypot" width="630"/>
</div>


#### Authors
- Barrirero, E.
- Villarroel, M. T.

**Director:** Dr.-Ing. Do Carmo, R. D. \
**Asesor:** Ing. Olocco, G. \
**Asesor Metodológico:** Dr. Ing. Argüello, J.A.

– 2016 –

### Abstract
```
The overall purpose of this engineering degree final work was to implement, evaluate and
develop new functional features over the Open Source honeypot Artemisa. Through an incentive
program for research projects from the Science and Technology Department from Cordoba
province together with Blas Pascal University, hardware requirements were evaluated, and as
a result, servers, networking devices and VoIP phones were acquired. Furthermore, we take
care of the installation of all these new equipment and network elements in the university’s
computer networks lab, for the implementation of a development and experimentation testbed.


The first stage of the project consisted in the implementation of Artemisa in testbeds, and during
this process, carry out configurations, upgrades and rigorous testing of the platform. Next steps
continued with the execution of Artemisa honeypot instances directly exposed and accessible
via the Internet in order to capture real attacks. At the same time, a participation letter was
drafted and shared in several computer security communities and forums, which is presented in
the Annex A, so that authentic and international sources attacks were captured, thus enabling
the proposition of optimal settings and configurations for real world scenarios. This honeypot is
really strong in private network environments, exposing in real-time and with detailed logs the
presence of an internal attacker. 

Additionally, a configuration in the SIP registrar that forwards
all communication attempts destined to a user-agent that it’s not registered in the domain to the
honeypot, increases the level of attacks detection, both internal and external. Then considering
the total number of VoIP SIP calls received by the registrars, a significant number of rejected
calls were validated, which is directly reflected in the REGISTER method statistics, as well as
SIP 401 unauthorized and 404 not found messages present in a substantial number and involved
in this process. Directly related with the excessive amount of the before mentioned events and
contrasted with Asterisk logs, is possible to certify that the mentioned traffic were malicious
registration attempts. 

Moreover, when integrating all the network traffic, to or from public IP
addresses, it stands out that Argentina and Germany were the countries with greater traffic
presence. In third place the United States, and finally Korea, Ireland and Poland. In addition, it
was clear that if the scope of the honeypot is increased to simulate the role of a SIP registrar
server, that will protect in a more effective manner the SIP domain communications, that is to
say, that adding some SIP methods to have basic registrar functions will achieve to evade all the
attacks that the current version of Artemisa is not exposed because of its back-end user-agent
role. The XML-RPC interface added to the source code speeds up and facilitates the honeypot
configuration, it also allows Artemisa integration with other network agents. 

It should be noted
that after the concretion of this project, today UBP has all the necessary resource and devices
to make an implementation of the project in courses such as Computer Networks II, Computer
Security, Network Protocols and Network Management that conforms the Telecommunications
Engineering degree, contributing with valuable practical experience for the graduate student
professional profile.
Keywords: honeypot, computer security, information security, SIP, VoIP, voice over ip.
```

<div align="left">
  <img src="https://raw.githubusercontent.com/exequielrafaela/LaTeX_EngineeringThesisArtemisaHoneypot/master/Figuras/Fig1.jpg" alt="artemisa-honeypot" width="730"/>
</div>

### Resumen
```
El objetivo general de este trabajo final de carrera fue el de implementar, evaluar y llevar
a cabo desarrollos funcionales sobre el honeypot de código abierto Artemisa. A través de un
programa de incentivos a proyectos de investigación del ministerio de ciencia y tecnología de
la provincia de Córdoba en conjunto con la UBP, se evaluaron requerimientos de hardware, y
como resultado se adquirieron servidores, dispositivos de networking, y teléfonos de Voz so-
bre IP (VoIP), los cuales nos encargamos de equipar y acondicionar en el laboratorio de redes
de la universidad, para la implementación en laboratorio de un escenario de prueba y desarro-
llo. 

El proceso fue conformado por la implementación de Artemisa en entornos reales en mesa
de prueba (testbed), llevando a cabo configuración, mejoras y riguroso testing de la platafor-
ma. Luego se continuó con la ejecución de instancias del honeypot (Artemisa) accesibles y
expuestas a Internet y capturando ataques reales. Paralelamente, se redactó y difundió una car-
ta de participación en foros y comunidades de seguridad informática, adjunta en el Anexo A,
para captar ataques auténticos y de fuentes internacionales, favoreciendo así el planteo de los
parámetros óptimos de configuración para entornos reales. Este honeypot se hace fuerte en en-
tornos de red privada, acusando en tiempo real y con registros detallados la presencia de un
atacante interno. 

Una configuración en el registrar de Protocolo de Inicio de Sesión (SIP) del
entorno que encamine hacia el honeypot todo intento de comunicación contra un agente SIP
que no pertenezca al dominio, aumenta el grado de detección de atacantes, tanto internos como
externos. En cuanto a la cantidad de llamadas VoIP SIP total (registrars) se validó un número
importantísimo de llamadas rechazadas, lo que se ve directamente reflejado por las estadísticas
del método REGISTER, como así también de los mensajes SIP 401 unauthorized y 404 not
found presentes en gran número e involucrados en este proceso. Por su número exagerado y
contrastando con los logs de Asterisk es que se acreditaron como intentos de registro mal inten-
cionados. 

Integrando todo el tráfico con origen o destino a direcciones Protocolo de Internet (IP)
públicas se destaca que Argentina y Alemania fueron los países de mayor protagonismo. En ter-
cer lugar Estados Unidos, y por último Corea, Irlanda y Polonia. Se hizo notorio que permitiría
proteger de forma más efectiva el dominio de comunicaciones SIP si se incrementa el alcance
del honeypot para simular el rol de un servidor de registro SIP, es decir, agregar algunos méto-
dos para que tenga funciones básicas de un registrar y así lograr desviar todos los ataques a
los que la actual versión de Artemisa no se ve expuesto por su rol de back-end user-agent. La
interfaz de Llamada de procedimiento remoto de Lenguaje de Marcas Extensibles (XML-RPC)
añadida al código fuente agiliza y facilita la configuración, y permite la integración del honey-
pot con otros agentes de la red. 

Cabe mencionar que en base a la realización y los resultados
del trabajo, hoy la UBP cuenta con los dispositivos y recursos necesarios para hacer viable la
implementación del proyecto en materias como Redes II, Seguridad Informática, Protocolos y
Gestión de Red, dentro de la carrera de Ingeniería en Telecomunicaciones, contribuyendo con
experiencia práctica muy valiosa al perfil profesional del egresado.
Palabras claves: honeypot, seguridad informática, SIP, VoIP, voz sobre ip.
```