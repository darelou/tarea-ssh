
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

## 2. Conexión por SSH

- Conectarse por SSH a ambas máquinas
- Crear usuarios: **Alex** y **Brais** en las respectivas máquinas
- Configurar la IP estática de ambas máquinas

![Configuración IP](images/page2_img2.png)

## 3. Conexión entre máquinas

- Desde **Máquina A** conectarse por SSH a **Máquina B**
- Conectarse mutuamente desde A a B y de B a A
- En cada máquina:
  - Crear un directorio en `/tmp`
  - Dejar un archivo como prueba

![Conexión SSH](images/page2_img1.png)

## 4. Transferencia de archivos

- Copiar el archivo creado en cada máquina a la otra

![SCP entre máquinas](images/page2_img2.png)

- Copiar los archivos de ambas máquinas a la **máquina nativa**

![Copia a máquina nativa](images/page2_img3.png)

## 5. Creación de directorio y transferencia masiva

- Crear el directorio `prueba3`
- Generar **200 archivos**

![Generación de archivos](images/page3_img1.png)

- Transferir el directorio a la máquina nativa

![Transferencia a host](images/page3_img2.png)

## 6. Autenticación por clave SSH

- Desde **Máquina A**, generar una clave SSH

![Generar clave SSH](images/page3_img3.png)

- Copiar la clave pública a **Máquina B**

![Copiar clave a B](images/page4_img1.png)

- Conectarse sin contraseña, usando autenticación por **frase de paso**

![Login sin contraseña](images/page4_img2.png)

---

> ✨ *Recuerda verificar que el servicio SSH esté activo en ambas máquinas y que el puerto configurado sea accesible desde tu red.*
