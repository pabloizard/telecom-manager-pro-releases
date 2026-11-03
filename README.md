# TelecomManager Pro — Versiones

Este repositorio **solo publica los paquetes de instalación** de TelecomManager Pro, una plataforma de gestión y ciberseguridad de redes: inventario con IPAM, CRM por cliente, dominios y hosting, monitor con alertas y herramientas de diagnóstico y auditoría. No es el repositorio de desarrollo.

## Descargar
Ve a [Releases](../../releases) y descarga `TelecomManager_Pro_Clean_Install.zip` de la última versión.

## Requisitos
- PHP 7.4 o superior con las extensiones `pdo`, `pdo_mysql`, `json`, `openssl` y `zip`
- MySQL o MariaDB (`utf8mb4`)
- Apache, Nginx o IIS, preferiblemente con HTTPS

## Instalar
1. Descomprime el ZIP en tu servidor web.
2. Abre `install.php` en el navegador y sigue las cinco fases.

## Actualizar
1. Haz una copia de seguridad desde **Mantenimiento**.
2. Sustituye `index.php` y `monitor_lib.php` a la vez (y los demás archivos que indique la release). No sobrescribas `ipconfig.php`.
3. Entra en la aplicación: las tablas y columnas nuevas se crean solas.

> **Guarda `tm_key.php` aparte.** Contiene la clave de cifrado de las credenciales y del 2FA. Sin ella no se pueden leer.

## Versiones
Se numeran por fecha: `AAAA.MM.N` (año, mes y número de publicación dentro del mes). Por ejemplo, `2026.11.1`.

## Comprobación de actualizaciones
La aplicación puede consultar la API pública de este repositorio para avisar de nuevas versiones. En **Acerca de → Versión y actualizaciones**, indica esta URL:

`https://api.github.com/repos/pabloizard/telecom-manager-pro-releases/releases/latest`

Solo informa: nunca descarga ni instala nada por sí sola.

## Contacto
Pablo Izard — pabloizard@gmail.com
