# CURSO: APRENDE BLAZOR

# LECCIÓN 3: Configuración de Carpetas y Archivos de la aplicación Blazor

![image](https://github.com/user-attachments/assets/16d8752d-bceb-4405-909c-bd986cc75ebb)

**Connected Services**: esta carpeta en donde se pueden añadir los servicios como Servicios de Azure (por ejemplo para autenticación de la aplicación, almacenamiento en la nube, etc.)

**Dependencies**: incluye los paquetes Nuget y otras dependencias/librerías del proyecto.  

**Properties**: esta carpeta contiene los archivos de configuración del proyecto. Por ejemplo, el archivo launchSettings.json contiene la configuración para ejecutar la aplicación en los diferentes entornos (desarrollo, producción, etc)

**wwwroot**: esta carpeta include los archivos estáticos de la aplicación (página web). Por ejemplo: archivos de estilo CSS, archivos de JavaScript, Imágenes, y Fuentes (tipos de letras). 

**Components Folder**: en esta carpeta se incluyen los componentes UI reutilizables. Incluye dos subcarpetas: Layout y Pages.

**Layout**:

**MainLayout.razor**: Este archivo incluye la disposición/configuración de la página princial de la aplicación. 

Define que se ha incluido el componente menú (**NavMenu**) a la izquierda. Un hipervínculo denominado **About**. 

El cuerpo central de la página web (**@Body**) y el mensaje mostrado en caso de error al cargar la página.

**NavMenu.razor**: Este componente es el menú de navegación de la aplicación. Incluye los vínculos a las diferentes páginas.

**Pages**: esta carpeta include los Componentes(páginas) que integran la aplicación.
Cada página/componente está definida en un archivo .razor.

**Home.razor**: es la página principal que incluye el mensaje Hello World.

**Counter.razor**: es una página de ejemplo que muestra un contador que se incrementa en una unidad cuando pulsamos sobre el botón.

**Weather.razor**: es una página de ejemplo que muestra una tabla de datos.

**Error.razor**: es la página que se muestra cuando hay un error en la aplicación.

**_Imports.razor**: este archivo contiene los "namespaces" y directivas disponibles para todos los archivos .razor en la misma carpeta y subcarpetas. 

Es un método para no tener que repetir los mismos @using para importar las mismas librerías en todas las páginas.

**App.razor**: este archivo es el Componente Raíz de la aplicación. Gestiona las rutas de la aplicación, y es responsable de renderizar el layout y las paginas requeridas por el usuario.

**Routes.razor**: este componente contiene el mapeado de las rutas de la aplicación.

En Blazor se definen los URLs que corresponden a cada página, y esto es normalmente gestionado por este archivo. 

**appsettings.json**: este es el archivo de configuración de la aplicación.

Normalmente guarda las configuraciones relacionadas con loggin, las URLs de las APIs, las cadenas de conexión a bases de datos, y otros datos de configuración.

**Program.cs**: este archivo contiene el punto de entrada de la aplicación Blazor. Es donde se configura la aplicación y donde se lanza la aplicación.
