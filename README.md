# Docker hello world

En este proyecto podras encontrar
ejemplos de API's REST desarrolladas en diferentes lenguajes de programación empaquetadas en imagenes de Docker.

---
## Java :

Para ejecutar el proyecto en Java es necesario tener el JDK y Maven, recomiendo instalar las herramientas usando [SDKMAN](https://sdkman.io/i).

Instalar SDKMAN:

```bash
curl -s "https://get.sdkman.io" | bash
```

Cerramos y abrimos la terminal después ejecutamos los siguientes comandos:

```bash
sdk install java

sdk install maven

cd java

mvn clean install

docker build . -t docker:java

docker run -p 4567:4567 docker:java
```

Abrimos la liga http://localhost:4567/

---
## Nodejs :

Para ejecutar el proyecto en Nodejs, debemos instalarlo y también instalar Yarn, para ello usaremos [NVM](https://github.com/nvm-sh/nvm).

Instalamos NVM:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

Cerramos y abrimos la terminal y ejecutamos:

```bash
nvm install node

curl -o- -L https://yarnpkg.com/install.sh | bash

yarn install

docker build . -t docker:nodejs

docker run -p 3000:3000 docker:nodejs
```
Abrimos la liga http://localhost:3000/

---
## Python :

Para ejecutar el proyecto en python necesitamos instalar ... 