# HeroesApp - Angular

Aplicación web desarrollada con Angular 11 que permite gestionar un catálogo de superhéroes.  
Incluye funcionalidades de búsqueda, edición, creación y eliminación de héroes, además de un backend simulado con **JSON-Server**.

---

## Descripción del proyecto

HeroesApp es una Single Page Application (SPA) que demuestra el uso de módulos, rutas, servicios, pipes y componentes en Angular.  
La aplicación organiza los héroes por casa (DC o Marvel) y permite realizar operaciones CRUD mediante peticiones HTTP a un servidor local simulado.

---

## Tecnologías utilizadas

|    Tecnología    |  Versión  |            Descripción           |
|------------------|-----------|----------------------------------|
| Angular          |    11.x   | Framework principal del proyecto |
| TypeScript       |    4.x    | Lenguaje base del desarrollo     |
| Angular Material |    11.x   | Diseño visual y componentes UI   |
| Flex Layout      |    11.x   | Diseño responsive                |
| JSON-Server      |    0.17.x | Simulación de backend REST       |
| Node.js          |    14.x   | Entorno de ejecución necesario   |

---

## Instrucciones de instalación y ejecución


### 1. Clonar el repositorio

### 2. Instalar dependencias
npm install
OJO: Es importante tener la versión de angular 11, para ello, usaremos el comando 'npm install -g @angular/cli@11'
Una vez hecho eso, necesitamos verificar la versión mediante el comando 'ng version'

### 3. Ejecutar la aplicación Angular
ng serve -o

Y la aplicación se ejcutará en: http://localhost:4200/

---

## Simulación del backend con JSON-Server

### 1. Creamos otra carpeta en la misma ubicación donde se encuentre nuestra carpeta de heroesApp
Esta carpeta se llamará "heroesService" y contendrá nuestro archivo db.json que contiene la base de datos local con los registros de héroes.

### 2. Necesitamos instalar la versión del Json-Server que sea compatible
npm install json-server@0.17.4 --save-dev
En este caso, usé la versión 0.17.4 ya que es la que no me generaba conflictos.

### 3. Iniciar el servidor
npx json-server --watch db.json

#### El backend estará disponible en:
http://localhost:3000/heroes

---

## En este proyecto usamos lo siguiente:
- Ruteo modular con carga perezosa (Lazy Loading)
- CRUD completo de héroes
- Filtros y pipes personalizados
- Estilos con Angular Material y Flex Layout
- Integración de JSON-Server como backend simulado
