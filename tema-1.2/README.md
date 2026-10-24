

\# Tema 1.2: Entornos de desarrollo portables y ligeros



\## Estudiante

Jaimer Hebbel Vélez Párraga



\## Características del equipo

\- Procesador: AMD Ryzen 7 5800X

\- Memoria RAM: 16 GB

\- Almacenamiento disponible: 189,74 GB en E:

\- Virtualización: habilitada en firmware

\- Sistema operativo: Windows



\## Entorno de desarrollo

\- Flutter: 3.47.7 (stable)

\- Dart: 3.13.5

\- Visual Studio Code: versión portable

\- Ruta del entorno: E:\\dev

\- Extensiones: Dart y Flutter 3.144.0



\## Destinos disponibles

\- Windows

\- Google Chrome

\- Microsoft Edge



\## Actividades realizadas

Se configuró un entorno portable de Dart y Flutter, se comprobó su funcionamiento mediante flutter doctor y se desarrollaron dos proyectos.



\### Proyecto hola\_entorno

Aplicación de consola creada con Dart que solicita el nombre del usuario y muestra un saludo, el sistema operativo y la versión de Dart.



\### Proyecto hola\_flutter

Aplicación Flutter ejecutada en Chrome, personalizada con el nombre del estudiante y un tema de color verde. Se comprobó el funcionamiento de Hot Reload.



\## Diagnóstico del entorno

Flutter doctor identificó una advertencia en Android toolchain debido a la falta de cmdline-tools y la aceptación de licencias. También indicó que Visual Studio no está instalado.



Estos componentes no son indispensables para las prácticas actuales en consola y Chrome.



\## Problema resuelto

Al ejecutar el programa Dart mediante F5, la consola de depuración no permitía introducir correctamente el nombre del usuario.



Se solucionó mediante el archivo .vscode/launch.json, configurando "program": "${file}" y "console": "terminal".



\## Entorno portable

Se creó iniciar.bat para configurar temporalmente el PATH y PUB\_CACHE, ejecutar Flutter y abrir VS Code portable.



La expresión %\~dp0 permite obtener automáticamente la carpeta donde se encuentra el archivo BAT.



\## Evidencias

Las capturas se encuentran en la carpeta evidencias y el diagnóstico de Flutter está disponible en doctor.txt.



