# PAGOEFECTIVO E2E FORM
1. [PRE REQUISITOS](#pre-requisito)
2. [INSTALACION](#instalacion)
3. [CONFIGURAR PRE Y PROD](#configurar-pre-y-prod)
4. [EJECUCION](#ejecucion)

## PRE REQUISITOS
***
1. Configuracion de llaves SSH en la pc y repositorio
2. Instalar Programas
    * Visual Studio Code: [link](https://code.visualstudio.com/)
    * Git: [link](https://git-scm.com/)
    * Node.js: [link](https://nodejs.org/en/)

**NOTA:** Si se tiene configurado las llaves SSH y instalados los programas, obviar este paso.

## INSTALACION
***
1. Ingresar al link del repositorio: 
    * [link bitbucket](https://bitbucket.org/orbisunt/pagoefectivo-e2e-form/src/master/): https://bitbucket.org/orbisunt/pagoefectivo-e2e-form/src/master/
2. Boton Clonar, elegir SSH y copiar 
    ```
    git clone git@bitbucket.org:orbisunt/pagoefectivo-e2e-form.git
    ```
3. Crear una carpeta en la unidad de tu escritorio, ubicarse dentro de la carpeta
    * Carpeta: PROYECTO-CYPRESS
 **NOTA:** Si se tiene la carpeta creada, obviar este paso.

4. Abrir git bash y pegar  
    ```
    git clone git@bitbucket.org:orbisunt/pagoefectivo-e2e-form.git
    ```
5. Se visualiza la carpeta creada 
    * Carpeta: pagoefectivo-e2e-form
6. Abrir el proyecto en Visual Studio y ejecutar comandos en el terminal
    * Añadir paquetes faltantes
        npm install 

## CONFIGURAR PRE Y PROD
***
1. **PRE**
    * Verificar si el servicio esta con la configuracion formulario y activo
        - Carpeta: cypress/fixtures/form-testdata.pre.js
2. **PROD**
    * Verificar si el servicio esta con la configuracion formulario y activo
        - Carpeta: cypress/fixtures/form-testdata.prod.js
## EJECUCION
***
1. **PRE**

    **PARA FORM PERU:**
    * Ingresar al terminal del Visual Studio y ejecutar 
    ```
    npm start
    ```
    * Se abre la pagina de Cypress y seleccionar
        - form-peru-register.spec.js
    * Se ejecuta las pruebas automatizadas
    * Se pondra en pausa la ejecucion para ingresar el codigo captcha
        - Copiar codigo captcha y clic al boton play

    **PARA FORM ECUADOR:**
    * Ingresar al terminal del Visual Studio y ejecutar 
    ```
    npm start
    ```
    * Se abre la pagina de Cypress y seleccionar
        - form-ecuador-register.spec.js
    * Se ejecuta las pruebas automatizadas
    * Se pondra en pausa la ejecucion para ingresar el codigo captcha
        - Copiar codigo captcha y clic al boton play

2. **PROD**

   **PARA FORM PERU:**
    * Ingresar al terminal del Visual Studio y ejecutar 
    ```
    npm run start-prod
    ```
    * Se abre la pagina de Cypress y seleccionar
        - form-peru-register.spec.js
    * Se ejecuta las pruebas automatizadas
    * Se pondra en pausa la ejecucion para ingresar el codigo captcha
        - Copiar codigo captcha y clic al boton play

    **PARA FORM ECUADOR:**
    * Ingresar al terminal del Visual Studio y ejecutar 
    ```
    npm run start-prod
    ```
    * Se abre la pagina de Cypress y seleccionar
        - form-ecuador-register.spec.js
    * Se ejecuta las pruebas automatizadas
    * Se pondra en pausa la ejecucion para ingresar el codigo captcha
        - Copiar codigo captcha y clic al boton play