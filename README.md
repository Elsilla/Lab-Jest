🧪 Proyecto Jest ES6+
Testing moderno con import/export, Jest 29+ y compatibilidad ESM mediante Babel.

📌 Descripción
Este proyecto proporciona una base completa para trabajar con pruebas unitarias en JavaScript utilizando Jest y sintaxis moderna ES6+ (import/export).

Está preparado para usarse en:

Bootcamps
Cursos introductorios
Proyectos Node.js ESM
Prácticas de testing unitario
🛠️ ¿Por qué usamos Babel en este proyecto?
Jest todavía presenta limitaciones al ejecutar proyectos 100% ES Modules (type: "module"), especialmente al trabajar con:

mocks
coverage
imports relativos
transformaciones internas
Para evitar errores y asegurar estabilidad, usamos:

babel-jest
@babel/preset-env
Esto permite que Jest entienda correctamente tus archivos ES6+ sin que tengas que usar require() o module.exports.

👉 Importante:

Tu código sigue siendo 100% ES Modules
No estás haciendo CommonJS
Babel solo actúa como “capa de compatibilidad” para Jest
📁 Estructura del proyecto
jest-esm-demo/
│
├── package.json
├── babel.config.js
├── jest.config.js
│
├── src/
│   ├── suma.js
│   ├── usuario.js
│   └── texto.js
│
└── tests/
    ├── suma.test.js
    ├── usuario.test.js
    └── texto.test.js
⚙️ Tecnologías utilizadas
Tecnología	Uso
Node.js	Entorno de ejecución
Jest 29+	Framework de testing
Babel + babel-jest	Compatibilidad con ES Modules
ES6+ import/export	Código moderno
▶️ 6. Cómo ejecutarlo
Instalar dependencias
npm install
Ejecutar pruebas
npm test
Modo watch
npm run test:watch
Cobertura
npm run coverage
Genera una carpeta:

coverage/
📘 Contenido del proyecto
Funciones en /src:

suma(a, b)
crearUsuario(nombre, edad)
capitalize(texto)
Pruebas en /tests:

Casos normales y borde
Manejo de errores
Validación de datos
🎯 Objetivo educativo
Permite aprender:

Estructura de pruebas unitarias
Jest con ES Modules
Uso de coverage
Testing moderno mantenible
