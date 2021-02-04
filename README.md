# README

La idea de este proyecto es probar una aplicacion cion de test en NODEJS

Se crea una clase simple que convierte colores RGB en HEX . "converter.js"
que tiene 2 metodos **rgbToHex** y **HexToRgb**. Estos metodos se prueban 
usando **chai** y se definen en **test/converter.js**.

Ademas se expone una api (usando express) para invocar a los metodos

Para correr los test ejecutar el comando **npm test**. Si se quiere probar
la api priemro se deve levantar el servicio **node app/server.js**


El resultdo del test debe ser

```sh

$ node app/server.js
$ npm test

 npm test

> converter@0.0.0 test /home/dugalman/Documents/Works/CLIENTE_DUGALMAN/JS_EMAC6_mocha/converter-ci-test
> mocha --reporter spec



  Color Code Converter
    RGB to Hex conversion
      ✓ converts the basic colors
    Hex to RGB conversion
      ✓ converts the basic colors

  Color Code Converter API
    RGB to Hex conversion
      ✓ returns status 200
      ✓ returns the color in hex
    Hex to RGB conversion
      ✓ returns status 200
      ✓ returns the color in RGB


  6 passing (64ms)

```

## Coverage

Hay que instalar la biblioteca **istambul** y ejecuar el comando 

## LINKS

https://istanbul.js.org/docs/tutorials/mocha/
