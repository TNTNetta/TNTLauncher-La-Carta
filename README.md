<p align="center"><img src="./app/assets/images/SealCircle.png" width="150px" height="150px" alt="aventium softworks"></p>

<h1 align="center">TNTLauncher</h1>
<em><h5 align="center">(Launcher creado por TNTStudios)</h5></em>

<p align="center">Bienvenido al TNTLauncher, un launcher creado por TNTStudios para cubrir todas tus necesidades de Minecraft.</p>

## Comandos Nebula

- Instalar dependencias: `npm i`
- Agregar archivo `.env`
- Crear distribución: `npm start -- init root`
- Crear carpeta:
   - Ejemplo: `npm start -- generate server [nombre del servidor] [versión de Minecraft (ej. 1.12.2)] --forge [versión de Forge (ej. 14.23.5.2859)]`
   - Ejemplo: `npm start -- generate server MangoLand 1.18.2 --forge 40.2.1`
- Generar archivos para servidor de alojamiento: `npm start -- generate distro`

## TNTLauncher

- Instalar dependencias: `npm i`
- Probar launcher: `npm run start`
- Compilar para sistema operativo:
   - Windows x64 (.exe): `npm run dist:win`
   - MacOS: `npm run dist:mac`
   - Linux x64: `npm run dist:linux`

Para evitar la recarga de archivos cada vez que inicies el juego, configura el archivo `server.meta`. Por ejemplo, para evitar que se recarguen las opciones, puedes usar el siguiente código:

   { //este simbolo no va
     "untrackedFiles": [
    {
      "appliesTo": ["files"],
      "patterns": [
        "config/*.cfg",
        "config/**/*.yml"
      ]
    }
  ]
}


También puedes usar el siguiente código para evitar la recarga de otros archivos específicos:

{ //este simbolo no va
     "untrackedFiles": [
    {
      "appliesTo": ["files"],
      "patterns": [
        "config/*.cfg",
        "config/**/*.yml"
      ]
    }
  ]
}
