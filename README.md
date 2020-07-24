# express_api_docker_containerizing
Ejemplo de Contenerización con docker de una api en express

## Requisitos 
Tener instalado docker en su maquina

## Pasos:
1 Clonar el repositorio 

2 Entrar en la carpeta del repositorio 

3 Ejecutar: ``npm install``.

4 Ejecutar el comando  ``docker build``. Este proceso creara una imagen en docker a partir del archivo <strong>Dockerfile</strong>. 
Al finalizar nos dara el siguiente mensaje: ``Successfully built 6560ae2a7f76``. Este codigo con 12 palabras es el id de la imagen creada por docker

5 Ejecutar el comando ``docker image ls`` Nos desplegara una lista de nuestras imagens

6 Ahora toca crear nuestro contenedor a partir de la imagen creada para esto ejecutamos el siguiente comando: ``docker run -d -p 3000:3000 6560ae2a7f76``. Configuramos
el puerto 3000 en nuestra computadora para este contendor

7 Ahora toca entrar al navegador y ver si nuestra api en docker funciona entramos al siguiente [http://127.0.0.1:3000](http://127.0.0.1:3000)

8 Listo tenemos nuestro contenedor creado exitosamente en docker 

