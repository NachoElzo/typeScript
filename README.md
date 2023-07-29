# [Install Node](https://nodejs.org/es)
# Install typeScript
    zsh: npm install -g typescript
# Check typescript version
    zsh: tsc -v
# Creates a file tsconfig.json for configure the compiler (uncomment)
    zsh : tsc -init
[Target]
    - ES2016 --> more stable version
[rootDir]
     ./src --> all the souce code will come from this folder path (create the folder inside the project)
[outDir]
     ./dist --> todo el codigo transpilado a javascript va a esta carpeta (nombre carpetanes una convención)
[noEmitOnError]
    false --> no crear codigo javascript en errores en typscript
[removeComments]
    true --> elimina los comentarios de la transpilacion a javascript 

[sourceMap]
    true -->  creates a .map file after run your code

# En la carpeta src ya creada, crea un archivo .ts para empezar 

# Como ya configuraste la ruta del codigo solo debes ejecutar en consola tsc para correr el codigo
    zsh : tsc

# How to debug de code  after [sourceMap=true]
    - execute run & debug from the button in the left menu of visual code
    - select create a launch .json file.
    - select node.js
    - this will create a launch.son file that contains configuration file
    - add to the file: 
        - "preLaunchTask": "tsc: build - tsconfig.json"
        - In launch.json file, below "program"
# how to debug before the above configuration
    - select a break point in your .ts file
    - execute run & debug from the button in the left menu of visual code
    - click the green play button in the above menu of visual code
    - select the configured Launch program
    - you will se debug buttons and a menu with the step information



    

