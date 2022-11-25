# Gladystad-Experiencia3-RegistrApp_Matus_Corbalan_005D
En caso de que aparezca un error al ejecutar Ionic Serve por qrcode

Instalar npm install angularx-qrcode --save

Si aparece un problema con el Storage, instalar npm install --save @ionic/storage-angular

Si hay un problema con el ' Import { QRCodeErrorCorrectionLevel } from "qrcode"; '

hay que reemplazar las lineas de código por la siguentes lineas de código en la carpeta ' tsconfig.json':

/* To learn more about this file see: https://angular.io/config/tsconfig. */
{
  "compileOnSave": false,
  "compilerOptions": {
    "baseUrl": "./",
    "outDir": "./dist/out-tsc",
    "sourceMap": true,
    "declaration": false,
    "downlevelIteration": true,
    "experimentalDecorators": true,
    "moduleResolution": "node",
    "importHelpers": true,
    "target": "es2015",
    "module": "es2020",
    "lib": ["es2018", "dom"]
  },
  "angularCompilerOptions": {
    "enableI18nLegacyMessageIdFormat": false,
    "strictInjectionParameters": true,
    "strictInputAccessModifiers": true,
    "strictTemplates": true
  }
}
