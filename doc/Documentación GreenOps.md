mejorar información en:
pantalla de modelado y simulación

<p align="center">
  <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/iconos/bannerNegro.png?raw=true" alt="GreenOps Logo" width="400"/>
</p>

<h6 align="right">Adrián Camilo Tuta Cortés y Miguel Angel Bejarano</h6>
<h6 align="right">04-08-2023</h6>

---

## <center><h6>Transformando Industrias, Preservando el Planeta.</h6></center>

- **Problemática**

  - Financia proyectos de infraestructura básica.
  <p align="center">
    <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/ilustraciones/Objetivo9.png?raw=true" alt="GreenOps Logo" width="300"/>
  </p>

  > _"De aquí a 2030, modernizar la infraestructura y reconvertir las industrias para que sean sostenibles, utilizando los recursos con mayor eficacia y promoviendo la adopción de tecnologías y procesos industriales limpios y ambientalmente racionales, y logrando que todos los países tomen medidas de acuerdo con sus capacidades respectivas."_ - Objetivo 9.4 de Desarrollo Sostenible

**Modelado y simulación de procesos industriales:** El software de modelado y simulación puede ayudar a analizar y optimizar los procesos industriales, identificando oportunidades para reducir el consumo de recursos, minimizar residuos y mejorar la eficiencia general.

---

## <center>DESCRIPCIÓN DEL PROYECTO</center>

<center>
  <h6>OPTIMIZACIÓN SOSTENIBLE DE PROCESOS INDUSTRIALES</h6>
</center>

_GreenOps_ es un proyecto de software que busca abordar la problemática de la acción por el clima, enfocándose en la optimización sostenible de procesos industriales. La idea central es utilizar el modelado y simulación de estos procesos para identificar oportunidades que permitan reducir el consumo de recursos, minimizar residuos y mejorar la eficiencia general.

### 1. EVALUAR VENTAJAS Y DESVENTAJAS:

| Ventajas                                           | Desventajas                   |
| -------------------------------------------------- | ----------------------------- |
| Sostenibilidad Ambiental                           | Complejidad de Implementación |
| Optimización de Recursos                           | Necesidad de Datos Precisos   |
| Cumplimiento de Objetivos de Desarrollo Sostenible | Costo Inicial                 |
| Competitividad en el Mercado                       | Limitaciones Tecnológicas     |
| Mejora Continua                                    |                               |

### 2. DEFINICIÓN GENERAL:

- #### 1. Definición del problema:

_GreenOps_ busca abordar la problemática de la acción por el clima, enfocándose en la optimización sostenible de procesos industriales. La ineficiencia y falta de sostenibilidad en estos procesos representan un desafío importante para las industrias y el medio ambiente.

- #### 2. Solución ofrecida:

_GreenOps_ consiste en un software de modelado y simulación de procesos industriales. Permitirá a las industrias analizar sus procesos actuales y encontrar oportunidades para optimizarlos y hacerlos más sostenibles. Al utilizar tecnologías y procesos industriales limpios, las empresas podrán reducir su impacto ambiental y ser más eficientes en el uso de recursos.

- #### 3. Justificación:

El valor generado por _GreenOps_ es significativo en términos de sostenibilidad y competitividad. Al ayudar a las industrias a modernizar su infraestructura y adoptar prácticas más sostenibles, _GreenOps_ contribuirá a cumplir con el Objetivo 9.4 de Desarrollo Sostenible de las Naciones Unidas. Además, las empresas que adopten _GreenOps_ podrán reducir costos operativos y mejorar su reputación en términos de responsabilidad ambiental.

- #### 4. Usuario final:

_GreenOps_ está dirigido a empresas y organizaciones industriales que buscan mejorar su rendimiento sostenible y cumplir con las regulaciones ambientales. Los responsables de operaciones y sostenibilidad en estas empresas serán los principales usuarios finales de la plataforma.

- #### 5. Utilidad:

La utilización de _GreenOps_ permitirá a las empresas obtener un retorno de inversión a largo plazo. Al optimizar sus procesos, reducirán el consumo de recursos y los costos operativos, lo que les permitirá ser más competitivos en el mercado y mejorar su rentabilidad.

- #### 6. Espacio de trabajo:

Toda la documentación relacionada con el proyecto se almacenará en la página del proyecto en GitHub. Esto facilitará la colaboración entre los miembros del equipo y el acceso a la información relevante.

### 3. ESPECIFICACIÓN INICIAL DE REQUERIMIENTOS:

- Antecedentes:
  <!-- https://geekflare.com/es/best-process-management-software/ -->

  | Aplicación  | Característica-1                  | Característica-2                   | Característica-3            | Característica-4                  |
  | ----------- | --------------------------------- | ---------------------------------- | --------------------------- | --------------------------------- |
  | **Creatio** | Gestión de Procesos Empresariales | Automatización de Flujo de Trabajo | Panel de Control Analítico  | Integración con CRM               |
  | **Bizagi**  | Modelado de Procesos BPMN         | Gestión de Casos                   | Colaboración en tiempo real | Integración con Sistemas Externos |
  | **Spyro**   | Monitoreo de Actividades          | Seguimiento de Tareas              | Reportes Personalizados     | Integración con APIs              |

- **Requisitos funcionales:**

  - Si el campo de correo o contraseña no están llenos, en el caso de correo el numero de letras debe ser mayor a 11 y la contraseña mayor a 8 se bloquearan los botones de las pantallas de ingreso.
  - Si el usuario no tiene conexión a internet se le debe informar con un mensaje.
  - Cuando un administrador haga un cambio se mostrará en la pestaña quienes fueron los últimos en hacer cambios y la fecha.
  - La visibilidad del campo de contraseña debe ser limitada, solo verán \* por cada carácter en este.

  - **Pantalla de Inicio de Sesión:**

    - Si las credenciales no son correctas debe mostrar un mensaje de contraseña incorrecta.
    - Cuando el usuario ingrese se actualizara en la base de datos la columna "ultima conexión" por la fecha actual.
    - El usuario tendrá tres intentos para ingresar su contraseña, si consume esos tres intentos, se bloqueará el acceso y se envía un correo con la información del intruso o posible ingreso.
    - Si el correo o contraseña no son válidos se enviará a la pestaña de registro.
    - Si el campo de correo no tiene explícitamente "@gmail.com"/"@outlook.com" el botón de ingreso estará desactivo.
    - Si el usuario ya inicio sesión y vuelve a la pantalla de inicio de sesión las credenciales ingresadas por el usuario se deben guardar y mostrar, para agilizar el ingreso de sesión y no escribirlos cada vez que se devuelva.

  - **Pantalla de Registro:**

    - El campo de correo debe tener por lo menos 11 caracteres para activar el botón de "enviar código de confirmación"
    - Cuando se presione el botón "enviar código de confirmación", se debe enviar un correo con un código aleatorio de 6 digitos.
    - El usuario tendrá solo 4 intentos para ingresar el código de confirmación, si consume estos 4 intentos se bloqueará la pantalla de registro.
    - Tendrá dos campos de contraseña, el segundo para confirmarla, si no son iguales no se activara el botón registrar.
    - Si todas las credenciales cumplen con todos los requisitos, Se enviará un correo de bienvenida, se publicará en la base de datos todas sus credenciales y estará en espera para que confirmen su tipo de usuario.

  - **Pantalla de Recuperación de Contraseña:**

    - El campo de correo debe tener por lo menos 11 caracteres para activar el botón de "enviar código de confirmación"
    - Cuando se presione el botón "enviar código de confirmación", se debe enviar un correo con un código aleatorio de 6 digitos.
    - El usuario tendrá solo 4 intentos para ingresar el código de confirmación, si consume estos 4 intentos se bloqueará la pantalla de registro.
    - Tendrá dos campos de contraseña, el segundo para confirmarla, si no son iguales no se activara el botón registrar.
    - Si todas las credenciales cumplen con todos los requisitos, Se enviará un correo de bienvenida, se publicará en la base de datos todas sus credenciales y estará en espera para que confirmen su tipo de usuario.

  - **Pantalla Principal:**

    - Será necesario para proporcionar a los usuarios un punto de entrada claro y funcional a la aplicación.
    - Contendrá una visión completa y completa de las opciones y funciones clave de la aplicación, garantizando que los usuarios puedan acceder a todas las áreas esenciales.
    - Mantendrá una presentación consistente y una disposición organizada de las características para que los usuarios puedan navegar y utilizar la aplicación sin confusión.
    - Mostrará la información de manera correcta y precisa, asegurando que los usuarios reciban una visión correcta de los datos y estadísticas relevantes.
    - Incluirá funciones factibles y alcanzables, evitando características complejas que puedan afectar la usabilidad y el rendimiento de la aplicación.
    - Será diseñado de manera que permita una fácil modificación en el futuro, para que se puedan incorporar nuevas funciones y ajustes según las necesidades cambiantes de los usuarios y el mercado.
    - Priorizará las opciones y funciones según su importancia y frecuencia de uso, para que los usuarios puedan acceder rápidamente a lo que necesitan más.

  - **Pantalla de Modelado y Simulación:**

    - Herramientas Efectivas para Modelados y Simulaciones:

      - Proporcionar una amplia gama de herramientas que abarquen diversos tipos de modelado y simulación, como modelos matemáticos, simulaciones físicas, simulaciones basadas en agentes, etc.
      - Incluir una interfaz intuitiva que permita a los usuarios crear y personalizar sus modelos y simulaciones desde cero, o utilizar plantillas predefinidas para casos comunes.

    - Funciones Completas para Cargar, Configurar, Ejecutar y Analizar:

      - Permitir la importación de datos externos en varios formatos (CSV) para utilizarlos como entradas en los modelos.
      - Proporcionar opciones detalladas de configuración para ajustar parámetros y condiciones iniciales según los requisitos específicos del modelo.
      - Ofrecer la capacidad de ejecutar simulaciones paso a paso para un análisis detallado o en tiempo real para una visión general rápida.
      - Incorporar herramientas de visualización interactiva que permitan a los usuarios analizar los resultados de manera efectiva, como gráficos 2D/3D, animaciones y representaciones visuales de datos.

    - Consistencia en la Disposición de Herramientas y Opciones:

      - Diseñar una interfaz con una disposición coherente, donde las herramientas y opciones relacionadas estén agrupadas de manera lógica y ordenada.
      - Utilizar un diseño y estilo uniforme en toda la pantalla para brindar una experiencia fluida y sin confusiones a través de diferentes simulaciones.

    - Precisión y Corrección en los Cálculos y Representaciones:

      - Emplear métodos numéricos y algoritmos confiables para garantizar que los cálculos sean precisos y consistentes con los principios del modelado y la simulación.
      - Validar las entradas del usuario para evitar errores y prevenir resultados incoherentes debido a configuraciones incorrectas.

    - Herramientas y Funciones Factibles y Realistas:

      - Proporcionar opciones que sean relevantes y aplicables a una variedad de campos, evitando características excesivamente especializadas o difíciles de entender para usuarios no expertos.

    - Diseño que Permita Modificaciones sin Comprometer la Estabilidad:

      - Desarrollar el sistema de manera modular, de modo que los cambios en los parámetros y configuraciones no generen fallas o errores en la aplicación.

    - Priorización de Herramientas y Funciones Esenciales:
      - Identificar las acciones y herramientas más utilizadas en escenarios de modelado y simulación y ubicarlas en posiciones destacadas y de fácil acceso en la interfaz.

  - **Pantalla de Informes y Gráficos:**

    - Será necesario para proporcionar a los usuarios información visual y detallada basada en los datos de la aplicación.
    - Contendrá informes y gráficos completos y exhaustivos que presenten de manera coherente los datos y tendencias relevantes.
    - Mantendrá una presentación consistente y uniforme de informes y gráficos, asegurando que los usuarios puedan comprender fácilmente la información presentada.
    - Garantizará la corrección y precisión de los informes y gráficos generados, evitando errores que puedan afectar las decisiones basadas en datos.
    - Ofrecerá opciones factibles para personalizar y configurar los informes y gráficos según las preferencias del usuario.
    - Será diseñado de manera que permita la modificación y actualización de informes y gráficos según nuevas necesidades o cambios en los datos.
    - Priorizará la generación de informes y gráficos más relevantes y necesarios para los usuarios, para que puedan acceder rápidamente a la información esencial.

  - **Pantalla de Configuración:**

    - Será necesario para permitir a los usuarios personalizar la aplicación según sus preferencias y necesidades.
    - Contendrá opciones completas y completas que abarquen diferentes aspectos de la configuración, como la interfaz de usuario, las notificaciones y la seguridad.
    - Mantendrá una presentación consistente y uniforme de las opciones de configuración, asegurando que los usuarios puedan ajustar la aplicación sin dificultades.
    - Garantizará la corrección y coherencia de las opciones de configuración, evitando configuraciones que puedan causar problemas o conflictos.
    - Ofrecerá opciones factibles que se puedan implementar de manera realista y sin afectar la estabilidad de la aplicación.
    - Será diseñado de manera que permita la modificación de las opciones de configuración sin requerir cambios fundamentales en la arquitectura de la aplicación.
    - Priorizará las opciones de configuración más esenciales y utilizadas para que los usuarios puedan adaptar rápidamente la aplicación a sus necesidades.

  - **Pantalla de Ayuda y Soporte:**

    - Será necesario para brindar a los usuarios la asistencia y recursos necesarios para utilizar la aplicación de manera efectiva.
    - Contendrá información completa y completa, como preguntas frecuentes, tutoriales y manuales de usuario, para ayudar a los usuarios a comprender y utilizar la aplicación.
    - Mantendrá una presentación consistente y uniforme de los recursos de ayuda y soporte, asegurando que los usuarios puedan acceder a la información de manera coherente.
    - Garantizará la corrección y precisión de los recursos de ayuda y soporte, evitando información incorrecta o engañosa.
    - Ofrecerá soluciones factibles y prácticas para los problemas comunes que los usuarios puedan enfrentar durante el uso de la aplicación.
    - Será diseñado de manera que permita la actualización y adición de nuevos recursos de ayuda y soporte según las necesidades cambiantes.
    - Priorizará la presentación de información y recursos de ayuda más relevantes y necesarios para los usuarios, para que puedan resolver rápidamente sus problemas.

  - **Pantalla de Administración de Usuarios:**

    - Será necesario para que los administradores puedan gestionar usuarios y roles de manera efectiva.
    - Contendrá funciones completas y completas que permitan a los administradores agregar, modificar y eliminar usuarios, así como asignar roles y permisos.
    - Mantendrá una presentación consistente y uniforme de las funciones de administración de usuarios, para que los administradores puedan gestionar usuarios de manera coherente.
    - Garantizará la corrección y precisión de las acciones de administración de usuarios, evitando errores que puedan afectar la base de datos de usuarios.
    - Ofrecerá opciones factibles para gestionar usuarios y roles de manera práctica y sin complicaciones.
    - Será diseñado de manera que permita la modificación de roles y permisos sin afectar la integridad de la base de datos de usuarios.
    - Priorizará las funciones de administración de usuarios más esenciales y utilizadas por los administradores, para que puedan realizar tareas de gestión de manera rápida.

  - **Pantalla de Notificaciones:**

    - Será necesario para proporcionar a los usuarios información relevante y oportuna a través de notificaciones.
    - Contendrá notificaciones completas y completas que informen a los

    usuarios sobre eventos importantes, como actualizaciones y mensajes críticos.

    - Mantendrá una presentación consistente y uniforme de las notificaciones, asegurando que los usuarios puedan entender rápidamente la información proporcionada.
    - Garantizará la corrección y precisión de las notificaciones enviadas, evitando errores que puedan causar malentendidos o confusión.
    - Ofrecerá opciones factibles para personalizar las preferencias de notificación según la relevancia y prioridad de los eventos.
    - Será diseñado de manera que permita la modificación y adición de nuevos tipos de notificaciones según las necesidades futuras.
    - Priorizará las notificaciones más relevantes y esenciales para los usuarios, para que puedan estar informados rápidamente sobre eventos importantes.

  - **Pantalla de Actualizaciones y Novedades:**

    - Será necesario para informar a los usuarios sobre las últimas actualizaciones y mejoras de la aplicación.
    - Contendrá descripciones completas y completas de las actualizaciones implementadas, detallando cómo afectan la funcionalidad y la experiencia del usuario.
    - Mantendrá una presentación consistente y uniforme de las actualizaciones y novedades, para que los usuarios puedan comprender rápidamente las mejoras.
    - Garantizará la corrección y precisión de la información proporcionada sobre las actualizaciones, evitando información engañosa o incorrecta.
    - Ofrecerá opciones factibles para acceder a más detalles sobre las actualizaciones y enlaces a recursos adicionales.
    - Será diseñado de manera que permita la adición de nuevas actualizaciones y novedades sin afectar la estructura de la pantalla.
    - Priorizará la presentación de las actualizaciones más importantes y significativas para que los usuarios puedan entender rápidamente los cambios en la aplicación.

- **Requerimientos No Funcionales:**

  - **Gráficas en Tiempo Real:**

    - El sistema debe contar con gráficas en tiempo real que muestren de manera dinámica los procesos en ejecución. Estas gráficas deben ser escalables y eficientes en términos de rendimiento. Además, deben ser configurables para mostrar diferentes tipos de procesos.

  - **Subida de Modelos de Procesos:**

    - Los usuarios podrán subir sus propios modelos de procesos para su análisis y simulación. La aplicación debe admitir una variedad de formatos de archivos, y los modelos subidos deben pasar por un proceso de validación para asegurar su integridad y compatibilidad con la plataforma.

  - **Actualizaciones en Cada Lanzamiento:**

    - La aplicación será actualizada en cada lanzamiento para garantizar la incorporación de nuevas características y correcciones. Los usuarios recibirán notificaciones claras sobre las actualizaciones y podrán acceder a detalles sobre los cambios realizados.

  - **Gama de Colores Adecuados:**

    - La interfaz de la aplicación utilizará una gama de colores diseñada específicamente para el contexto industrial al que está dirigida. Se priorizará la elección de colores que sean legibles, contrastantes y adecuados para transmitir información de manera clara.

  - **Control de Edición en la Aplicación:**

    - Los administradores tendrán la capacidad de modificar contenidos y configuraciones en la aplicación. Sin embargo, para evitar conflictos, solo un administrador podrá realizar cambios en una pestaña específica a la vez. Los otros administradores podrán observar los cambios en tiempo real sin intervenir.

  - **Almacenamiento de Cuentas en la Base de Datos:**

    - Las cuentas de usuarios almacenadas en la base de datos se asegurarán mediante medidas de seguridad adecuadas, como el cifrado de contraseñas. Se implementará un proceso de eliminación segura para las cuentas que no hayan sido utilizadas en un período de tres meses.

  - **Eliminación de Cuentas Inactivas:**

    - Las cuentas de usuarios que no se utilicen durante más de tres meses serán identificadas como inactivas. Antes de eliminarlas, se notificará a los usuarios sobre la posible eliminación y se proporcionará un período de tiempo para reactivar su cuenta si así lo desean.

  - **Tipos de Usuario y sus Roles:**

    - Los usuarios de la aplicación se dividirán en cuatro tipos, cada uno con roles y privilegios específicos:
      - **Gerentes de Producción:** Encargados de la planificación y supervisión de la producción industrial.
      - **Analistas de Eficiencia Energética:** Expertos en optimización del consumo de recursos energéticos.
      - **Ingenieros de Procesos:** Profesionales que modelan y optimizan procesos industriales.
      - **Estudiantes e Investigadores:** Utilizan la aplicación para aprender y estudiar procesos industriales.

  - **Roles de Administrador:**

    - Los administradores tendrán diferentes roles y niveles de acceso en función de sus responsabilidades. Habrá un "superadministrador" con poderes más amplios, mientras que otros administradores tendrán roles más específicos.

  - **Seguridad y Privacidad:**

    - Se implementarán medidas de seguridad sólidas para proteger la información de los usuarios y garantizar la confidencialidad de los datos almacenados en la aplicación. Esto incluirá el cifrado de datos sensibles y la autenticación segura.

  - **Escalabilidad:**

    - La aplicación estará diseñada para ser escalable y capaz de manejar un aumento en la cantidad de usuarios. Se optimizará el rendimiento y la capacidad de respuesta para asegurar una experiencia fluida incluso en momentos de alta demanda.

  - **Compatibilidad de Dispositivos:**

    - La aplicación será compatible con una variedad de dispositivos, incluyendo dispositivos móviles, tablets y computadoras. Se garantizará una experiencia de usuario coherente en todas las plataformas.

  - **Documentación:**

    - Se proporcionará documentación exhaustiva, incluyendo manuales de usuario, guías de administrador y recursos de soporte. Esto permitirá a los usuarios aprovechar al máximo la aplicación y resolver cualquier problema que puedan encontrar.

- **Alcances del sistema:**

  - El sistema se enfocará en implementar las funcionalidades esenciales definidas en los Requerimientos Funcionales y No Funcionales. Se priorizará la funcionalidad sobre la estética de la interfaz de usuario, y se garantizará la compatibilidad con dispositivos de escritorio.

  - La seguridad se mantendrá a través de medidas estándar, aunque características avanzadas como autenticación de dos factores podrían ser consideradas en el futuro. La documentación será básica en un principio, con planes para expandirla en versiones posteriores.

  - El sistema se desarrollará de manera iterativa, lanzando versiones incrementales con nuevas características y mejoras basadas en los comentarios de los usuarios. Las actualizaciones se planificarán según las necesidades del mercado y las retroalimentaciones.

  - La integración con sistemas externos se considerará en etapas posteriores, y se utilizarán eficientemente los recursos disponibles en términos de tiempo y costo.

- **Tecnologías seleccionadas:**
  _GreenOps_ se desarrollará utilizando las siguientes tecnologías:

  - Lenguaje de Programación: _Java_.

  - Entorno de Desarrollo: _Visual Studio Code_, NetBeans, NeoVim.

  - Bibliotecas y Frameworks: Swing, JFreeChart, XChart o JMathPlot, Log4j o SLF4J, JUnit o TestNG, JavaMail, Apache Commons Math.

  - Base de Datos: MySQL.

  - Control de Versiones: Git.

  - Plataforma de Despliegue: Docker.

[Presentación](https://www.canva.com/design/DAFrA2Mk0kg/GPSIsVQc-SVUu8AG1g9nDw/edit?utm_content=DAFrA2Mk0kg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

---

# <center> <h6>APLICACIÓN</h6></center>

<!-- LOGO: [Looka](https://looka.com/dashboard) -->

### 1. LOGOS

- #### Icono de la aplicación:

  <p align="center">
    <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/iconos/icon.png?raw=true" alt="GreenOps icon" width="200"/>
  </p>

- #### Logo grande:

  <p align="center">
    <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/iconos/bannerNegro.png?raw=true" alt="GreenOps banner" width="300"/>
  </p>

### 2. TIPOGRAFÍA

- Títulos: **_MOON GET_**.
- Textos o información: Nunito, Montserrat, Lato.
- Botones: Source Sans Pro, FSP DEMO - Proxima Nova.

### 3. COLORES

<!-- https://www.happyhues.co/palettes/4 -->

| Elemento       | Código de Color | Ejemplo                                                                                                                                           |
| -------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fondo          | `#16161a`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorFondo.png?raw=true" alt="Color de Fondo " width="200"/>               |
| Encabezado     | `#fffffe`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorEncabezado.png?raw=true" alt="Color de Encabezado " width="200"/>     |
| Párrafo        | `#94a1b2`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorParrafo.png?raw=true" alt="Color de Párrafo " width="200"/>           |
| Botón          | `#7f5af0`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorBoton.png?raw=true" alt="Color de Botón " width="200"/>               |
| Texto de Botón | `#fffffe`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorTextoBoton.png?raw=true" alt="Color de Texto de Botón " width="200"/> |
| Resaltado      | `#7f5af0`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorResaltado.png?raw=true" alt="Color de Resaltado " width="200"/>       |
| Borde          | `#010101`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorBorde.png?raw=true" alt="Color de Borde " width="200"/>               |
| Principal      | `#fffffe`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorPrincipal.png?raw=true" alt="Color de Principal " width="200"/>       |
| Secundario     | `#72757e`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorSecundario.png?raw=true" alt="Color de Secundario " width="200"/>     |
| Terciario      | `#2cb67d`       | <img src="https://github.com/CaMiLoTuTa/GreenOps/blob/main/img/colores/colorTerciario.png?raw=true" alt="Color de Terciario " width="200"/>       |

### 4. PANTALLAS

- **Pantalla de Inicio de Sesión:**

  - Permite a los usuarios ingresar sus credenciales para acceder a la aplicación.

- **Pantalla de Registro:**

  - Permite a los nuevos usuarios crear una cuenta en la aplicación.

- **Pantalla de Recuperación de Contraseña:**

  - Permite al usuario recibir un correo para restablecer su contraseña.

- **Pantalla Principal:**

  - Muestra una visión general de los procesos industriales y sus indicadores clave de rendimiento (KPI).

- **Pantalla de Modelado y Simulación:**

  - Permite a los usuarios cargar modelos de procesos, realizar simulaciones y ver los resultados de optimización.

- **Pantalla de Informes y Gráficos:**

  - Presenta informes detallados y gráficos que muestran los resultados de las simulaciones y optimizaciones realizadas.

- **Pantalla de Configuración:**

  - Permite a los usuarios personalizar la configuración de la aplicación y ajustar los parámetros de simulación.

- **Pantalla de Ayuda y Soporte:**

  - Proporciona información y recursos de ayuda para los usuarios que puedan tener preguntas o problemas.

- **Pantalla de Administración de Usuarios:**

  - Permite a los administradores gestionar los usuarios, sus roles y permisos dentro de la aplicación.

- **Pantalla de Notificaciones:**

  - Muestra notificaciones importantes o alertas relevantes para los usuarios.

- **Pantalla de Actualizaciones y Novedades:**
  - Informa a los usuarios sobre nuevas funcionalidades o actualizaciones de la aplicación.

### 5. Funcionalidades Destacadas:

[Listado de las funcionalidades clave de la aplicación GreenOps que la hacen destacar y diferenciarse de otras soluciones similares.]

### 6. Requisitos del Sistema:

[Especificación de los requisitos mínimos del sistema para ejecutar la aplicación, como sistema operativo, versión de Java, memoria RAM, espacio de almacenamiento, etc.]

### 7. Instalación:

[Instrucciones detalladas para instalar la aplicación en diferentes plataformas (Windows, macOS, Linux).]

### 8. Guía de Uso:

[Guía paso a paso sobre cómo utilizar cada una de las pantallas mencionadas anteriormente, explicando las funcionalidades y opciones disponibles.]

### 9. Contribución:

[Invitación a la comunidad de desarrolladores a contribuir al proyecto, proporcionando información sobre cómo realizar contribuciones y el proceso de solicitud de incorporación de cambios (pull requests).]

### 10. Equipo de Desarrollo:

[Presentación del equipo de desarrollo responsable del proyecto, mencionando sus roles y responsabilidades.]

### 11. Licencia:

[Especificación de la licencia bajo la cual se distribuye el código fuente de la aplicación GreenOps y aclaración de los términos y condiciones de uso.]

### 12. Contacto y Soporte:

[Información de contacto para consultas, soporte técnico y cualquier otro tipo de comunicación relacionada con el proyecto.]

### 13. Información Adicional:

[Inclusión de cualquier otro dato relevante o particular sobre la aplicación GreenOps que se desee resaltar.]
