# Adquisición de la evidencia

### **Documentación Inicial de la Escena**

Durante la adquisición de la evidencia, se realizó la documentación exhaustiva del estado de la escena y de los dispositivos presentes, siguiendo los principios forenses para asegurar la trazabilidad de cada elemento:

* **Presencia de dispositivos en la escena:**  
  * **Marca, modelo y número de serie**: En el caso del dispositivo identificado, se registró como **Máquina Windows 7**. No se dispone de número de serie ya que es una máquina virtual en un entorno de práctica.  
  * **Ubicación exacta**: El dispositivo virtual está ubicado dentro del entorno controlado de VirtualBox.  
  * **Estado del dispositivo**: El dispositivo estaba en vivo, y mostró la ventana de selección de configuración de red al inicio del proceso.  
* **Fotografías de la Escena:**

![](img1.jpeg)

* **Etiquetado del Dispositivo:**  
  * **Código Único**: Se le asignó el código **VM-001** para identificarlo en el proceso.  
  * **Etiqueta de Evidencia**: La máquina virtual fue etiquetada virtualmente con el identificador **VM-001** en la documentación.

### **Capturas de datos volátiles**

En esta sección se documenta el proceso de adquisición en vivo de evidencias digitales, siguiendo el orden de volatilidad para maximizar la preservación de datos. El objetivo principal de la adquisición en vivo es preservar la memoria volátil y otros elementos temporales del sistema, asegurando siempre la integridad de los datos durante la recolección.

##### **Captura de la memoria RAM**
Para obtener la memoria RAM , se ha utilizado la herramienta ```RamCapturer64``` . Esta herramienta permite realizar un volcado completo de la memoria RAM sin afectar la integridad de los datos.

![](ramCapturer.png)

Una vez completada la captura, se ha procedido a calcular los valores hash, utilizando los algoritmos MD5 y SHA-1 para asegurar la integridad del archivo de volcado. Los hashes calculados nos permiten verificar que el volcado de memoria no ha sido alterado durante su almacenamiento o transferencia.

|Nombre|hash|
|-|-|
|md5|7412d141d11af0bd304975f943c4e1e3|
|sha1|b4f79ca54f4bba663cd59fcbb32d9b61b614c447|

##### 	**Adquisición de el disco duro**

Para hacer una adquisición del disco duro se ha utlizado ```FTK imager```. Esta herramienta permite generar una copia exacta del contenido del disco, preservando toda la información y asegurando la integridad de los datos adquiridos.

Se rellenaron los datos del caso en la interfaz de FTK Imager, incluyendo el número de caso VM-001, número de evidencia 001, y una descripción única del dispositivo como hard disk copy. Además, el nombre del examinador, Alejandro Díaz Barea, se incluyó para identificar al responsable del proceso.

![](nombreCasoDIsc.png)

A continuación, se seleccionó la ubicación de destino para almacenar la imagen del disco y se eligió el formato raw, un formato común para adquisiciones forenses que facilita el análisis posterior sin modificar la estructura de los datos. La copia de la imagen se generó con éxito, preservando todos los sectores del disco.

![](discoDuro.png)

Finalmente, se calcularon los valores hash (MD5 y SHA1) del archivo de imagen generado para asegurar la integridad de los datos y verificar que no se produjeron alteraciones durante el proceso de copia.

![](hashDisco.png)


| Nombre | Hash                                    |
| ------ | --------------------------------------- |
| md5    | 5708010b9ba58a7bfcd33b8cd124eeeb        |
| sha1   | cb38cce7a61b9b0f4619796bd10aea18a49fdd5 |


##### **Triaje de el disco duro**



##### **Adquisición de logs del sistema** 

### **Cadena de custodia**

##### Formulario de Cadena de Custodia para Evidencias Digitales

~~~

1. Número de caso / Identificador único: **VM-001**

2. Descripción detallada del dispositivo:

   - Tipo de dispositivo: Máquina Virtual
   - Marca: Windows
   - Modelo: Windows 7
   - Número de serie: N/A (Máquina virtual sin número de serie)
   - Características adicionales: Configuración para práctica forense

3. Recolección:

   - Fecha: 0/11/2024
   - Hora: 17:35 hrs
   - Lugar de recolección: Entorno controlado VirtualBox

4. Recolector:

   - Nombre completo: Alejandro Díaz Barea
   - Cargo/Institución: C.E Ciberseguridad
   - Firma: Alejandro Díaz Barea

5. Estado del dispositivo al momento de la recolección:
   El dispositivo estaba encendido al inicio de la adquisición, en un escenario en vivo, mostrando la ventana de selección de configuración de red.

6. Observaciones adicionales:
   El dispositivo es una máquina virtual Windows 7. La adquisición se realizó siguiendo el orden de volatilidad para asegurar la preservación de los datos.

Certifico que la información proporcionada en este formulario es verdadera y precisa según mi mejor conocimiento.

Firma del recolector: Alejandro Díaz Barea Fecha: 10/11/2024
~~~


##### Documentación detallada

Elaboraremos un informe detallado, incluyendo hora, fecha, todos los procedimientos realizados en detalle, etc. De forma que quede todo registrado de la forma mas detallada, precisa y completa posible. 

- Registro cronológico detallado:
~~~
Fecha: 18/10/2024
17:53 - Llegada a la escena
17:53 - Fotografía inicial de la disposición de la escena
17:54 - Verificación del estado: encendido
17:57 - Identificación de computadora de escritorio (Windows 7)
~~~

- Tabla de acciones y resultados:

| Hora  | Acción                           | Herramienta utilizada | Resultado/Observación                    |
|-------|----------------------------------|----------------------|------------------------------------------|
| 17:53 | Aseguramiento de la escena       | N/A                  | Área acordonada, acceso restringido      |



