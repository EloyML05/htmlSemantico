## Para poder utilizar el CSS Nano
 
 **1º** Utilizamos el istalador de paquetes Node.js

 **2º** Utilizamos el siguiente comando:
 ``` bash
 npm install cssnano postcss --save-dev
 ```

 **3º** Utilizamos el siguiente comando que instala el PostCSS CLI
 ``` bash
 npm install --save-dev postcss-cli
 ```

 **4º** Creamos el archivo [postcss.config.js](postcss.config.js) y introducimos el siguiente codigo:

 ```code
module.exports = {
    plugins: [
        require('cssnano')({
            preset: 'default',
        }),
    ],
};
 ```

 **5º**  Una vez instalado y configurado ejecutamos en siguinte comando:
 ```bash
npx postcss input.css > output.css
 ```




