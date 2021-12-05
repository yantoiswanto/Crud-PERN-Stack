1. Installations :

- yarn init
- tsc --init
- yarn add typescript ts-node express cors nodemon
- yarn add @types/cors @types/express @types/node
- yarn add typeorm pg graphql express-graphql

2. add folder dist and src
3. edit file tsconfig.json :
   "target": "es5" to "es6"
   // "outDir": "./" to "outDir": "./dist",
   // "rootDir": "./" to "rootDir": "./src",
   // "strictPropertyInitialization": true to "strictPropertyInitialization": true
   // "experimentalDecorators": true to "experimentalDecorators": true
   //"emitDecoratorMetadata": true to "emitDecoratorMetadata": true,
4. edit package.json
   add :
   "scripts": {
   "start": "node ./dist/index.ts",
   "dev": "nodemon ./src/index.ts",
   "build": "tsc -P ."
   }
