# Sistema Contable

Aplicación de escritorio para registrar operaciones contables y consultar libros y estados financieros. Está construida con Electron y utiliza un backend local con Express y una base de datos SQLite.

## Requisitos

- Windows
- La carpeta completa de la aplicación, con `Sistema Contable.exe` y los archivos que lo acompañan

## Iniciar la aplicación

1. Descarga o copia la distribución completa del repositorio a una carpeta local.
2. Abre `Sistema Contable.exe`.

No muevas el ejecutable fuera de la carpeta de distribución: necesita los recursos de Electron incluidos junto a él. No se requiere instalar Node.js para ejecutar esta versión.

## Funciones

- Panel con resumen de saldos, ingresos, costos y gastos.
- Catálogo de cuentas contables.
- Registro de asientos.
- Consulta del libro diario y del libro mayor.
- Balance general y estado de resultados.
- Filtros por período, impresión o guardado en PDF y exportación a Excel en los informes compatibles.
- Creación y restauración de copias de seguridad desde Configuración.

## Datos y respaldos

La aplicación inicia su backend local al abrirse y guarda la base de datos `sistema_contable.db` en el directorio de datos de usuario que administra Electron. Por ello, los datos de trabajo no se guardan necesariamente dentro de la carpeta del repositorio.

Usa **Configuración → Crear copia de seguridad** para guardar una copia en otra ubicación. La opción **Restaurar respaldo** acepta archivos `.db`, `.sqlite` y `.sqlite3`. Conserva las copias en un lugar seguro y verifica que el archivo elegido sea el respaldo correcto antes de restaurarlo.

## Sobre este repositorio

Este repositorio contiene una distribución empaquetada para Windows, no un proyecto de desarrollo listo para compilar. El código de la aplicación está dentro de `resources/app.asar`; no se incluyen scripts de instalación de dependencias, desarrollo o compilación. Por tanto, aquí se documenta cómo ejecutar la aplicación distribuida, no cómo reconstruirla desde el código fuente.
