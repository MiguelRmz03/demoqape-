# PAGOEFECTIVO E2E CHARGE
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
    * [link bitbucket](https://bitbucket.org/orbisunt/pagoefectivo-e2e-charge/src/master/): https://bitbucket.org/orbisunt/pagoefectivo-e2e-charge/src/master/
2. Boton Clonar, elegir SSH y copiar 
    ```
    git clone git@bitbucket.org:orbisunt/pagoefectivo-e2e-charge.git
    ```
3. Crear una carpeta en la unidad de tu escritorio, ubicarse dentro de la carpeta
    * Carpeta: PROYECTO-CYPRESS    
    * **NOTA:** Si se tiene la carpeta creada, obviar este paso.

4. Abrir git bash y pegar  
    ```
    git clone git@bitbucket.org:orbisunt/pagoefectivo-e2e-charge.git
    ```
5. Se visualiza la carpeta creada 
    * Carpeta: pagoefectivo_e2e_charge
6. Abrir el proyecto en Visual Studio y ejecutar comandos en el terminal
    * Crea el package.json
    ```
    npm init
    ```
        Boton Enter hasta que aparesca el mensaje
    ```
    Is this OK? (yes)  yes
    ```
    * Añadir paquetes faltantes
        npm install cypress 

## CONFIGURAR PRE Y PROD
***
1. **PRE**
    * Ingresar al archivo "cypress/cypress.env.json" y configurar
    ```
        {
            "host" : "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
            "api" : "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
            "login": {
                "userName": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
                "password": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)"
            },
            "db": {
                "server": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
                "options": {
                    "database": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
                    "port": (ARCHIVO DRIVE - DATA AUTOMATIZACION),
                    "rowCollectionOnRequestCompletion": true,
                    "trustServerCertificate": true
                },
                "authentication": {
                    "type": "default",
                    "options": {  
                        "userName": "(USUARIO DE BD)",
                        "password": "(PASSWORD DE BD)"
                    }
                }
            }
        }
    ```

2. **PROD**
    * Ingresar al archivo "cypress/cypress.env.json" y configurar
    ```
        {
            "host" : "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
            "api" : "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
            "login": {
                "userName": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
                "password": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)"
            },
            "db": {
                "server": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
                "options": {
                    "database": "(ARCHIVO DRIVE - DATA AUTOMATIZACION)",
                    "port": (ARCHIVO DRIVE - DATA AUTOMATIZACION),
                    "rowCollectionOnRequestCompletion": true,
                    "trustServerCertificate": true
                },
                "authentication": {
                    "type": "default",
                    "options": {  
                        "userName": "(USUARIO DE BD)",
                        "password": "(PASSWORD DE BD)"
                    }
                }
            }
        }
    ```

## EJECUCION
***
1. **PRE**

    * Ingresar al terminal del Visual Studio y ejecutar 
    ```
    npm start
    ```
    * Se abre la pagina de Cypress y seleccionar
        - complete-flow.spec.js
    * Se ejecuta las pruebas automatizadas
    * Se pauseara la automatizacion para que cambie de estado la cobranza
        - Esperar un minuto y clic al boton play

    
2. **PROD**

   **PARA FORM PERU:**
    * Ingresar al terminal del Visual Studio y ejecutar 
    ```
    npm run start
    ```
    * Se abre la pagina de Cypress y seleccionar
        - complete-flow.spec.js
    * Se ejecuta las pruebas automatizadas
    * Se pauseara la automatizacion para que cambie de estado la cobranza
        - Esperar un minuto y clic al boton play
    
