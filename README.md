
# Tarea de SSH y SCP

## 1. Configuración de las máquinas virtuales

- Crear dos máquinas virtuales: **Máquina A** y **Máquina B**
- Configuración de red:
  - **Adaptador 1**: Tipo NAT
    - Una máquina con el reenvío de puertos predeterminado
    - La otra con el puerto **2223**
  - **Adaptador 2**: Tipo **Red Interna**
    - Para la comunicación entre las dos máquinas

![Configuración de red](images/page1_img1.png)
![Configuración IP](images/page1_img2.png)

## 2. Nos conectamos por ssh a las dos máquinas 

![Conexión SSH](images/page2_img1.png)

Y añadimos correspondientes Alex y Brais a las respectivas máquinas 

![Configuración IP](images/page2_img2.png)

Finalmenta configuramos la ip de las dos maquinas 

![Configuración IP](images/page2_img3.png)

## 4. Conexion entre máquinas

- Nos conectamos a la maquina B desde la máquina A 

![SCP entre máquinas](images/page3_img1.png)

- Ahora nos conectamos a cada maquina entre ellas respectivamente para crear un directorio en /tmp dejando un archivo en cada maquina como prueba de haberlo conseguido  

![Copia a máquina nativa](images/page3_img2.png)

 - Por ultimo copiamos respectivamente de cada maquina el archivo que hemos creado

![Copia a máquina nativa](images/page3_img3.png)
 
## 5. Transferencia de archivos

- Copiamos los archivos de cada máquina a nuestra máquina nativa

![Generación de archivos](images/page4_img1.png)

- Ahora creamos el directorio prueba3 para crear los 200 archivos

![Transferencia a host](images/page4_img2.png)

- Y nos lo pasamos a nuestro ordenador

![Transferencia a host](images/page4_img3.png)

## 6. Claves

- generamos la clave Desde A

![Generar clave SSH](images/page5_img1.png)

- Y se la pasamos a la máquina B  

![Copiar clave a B](images/page6_img1.png)

- Y por último nos conectamos por frase 

![Login sin contraseña](images/page6_img2.png)

