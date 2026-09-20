# RSF Vehicle Radio Manager

Herramienta independiente para Windows que permite crear y administrar paquetes de música personalizados para **RSF Vehicle Radio** en Arma 3.

> **Versión actual:** 0.6.0  
> **Plataforma:** Windows  
> **¿Necesita Python o Arma Tools?:** No

## Inicio rápido

1. Descarga y extrae el ZIP de la versión más reciente.
2. Abre **RSF Radio Manager.exe**.
3. Pulsa **Nuevo** para crear el paquete de tu comunidad.
4. Elige una estación o crea una nueva.
5. Arrastra canciones o carpetas, o utiliza el selector de archivos.
6. La preparación comienza automáticamente.
7. Usa **Biblioteca** para escuchar, buscar, editar, mover o quitar canciones.
8. Usa **Estaciones** para cambiar nombres, frecuencia y orden.
9. En **Compartir paquete**, pulsa **Exportar paquete**.
10. Comparte únicamente la carpeta exportada.

## Qué hace

- Importa archivos individuales, varios archivos o carpetas completas.
- Convierte automáticamente el audio a OGG para Arma.
- Genera también el audio utilizado por el Modo Altavoz.
- Permite crear y organizar estaciones personalizadas.
- Conserva una cola de preparación persistente.
- Permite detener y continuar el proceso.
- Omite archivos idénticos ya importados en el mismo proyecto.
- Reutiliza conversiones anteriores cuando es posible.
- Exporta un paquete musical independiente para tu comunidad.

## Herramientas automáticas

En el primer uso de archivos locales, el Manager descarga FFmpeg desde el proveedor configurado y verifica la descarga mediante SHA-256.

La importación opcional desde YouTube descarga yt-dlp y Deno desde sus repositorios oficiales cuando se necesitan.

La función de descarga no concede derechos sobre grabaciones ni autorización para publicarlas. Utiliza contenido propio o con los permisos correspondientes y respeta las condiciones de la plataforma.

## Para tu comunidad

Servidor y jugadores deben cargar:

- **RSF Vehicle Radio**
- Tu paquete musical exportado

La música oficial es opcional. El Manager solo es necesario para la persona que administra o crea el paquete musical.

Si publicas tu paquete en Steam Workshop, marca **RSF Vehicle Radio** como elemento requerido.

## Actualizar el Manager

Cierra el Manager y reemplaza el EXE y la documentación. Conserva tu carpeta **Data**, ya que contiene tus proyectos, originales, cola y herramientas descargadas.

No distribuyas tu carpeta Data personal.

## Licencia

Consulta [LICENSE.txt](LICENSE.txt) y [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt).
