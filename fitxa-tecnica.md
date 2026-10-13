# Montaje de un PC de escritorio e instalación del SO
![S](https://repararordenadores.com/wp-content/uploads/2024/09/PC-por-Componentes-1024x576.jpg.webp)
## Objetivo
Montar un ordenador de escritorio desde cero conectando correctamente todos los componentes de hardware e instalar un sistema operativo (Ubuntu Linux o Windows) para dejar el equipo completamente funcional y verificado.
## Materiales 
- Placa base (Motherboard)                                              
- Procesador (CPU) y disipador / ventilador
- Memoria RAM (Módulos DDR4/DDR5)
- Unidad de almacenamiento (SSD NVMe M.2 o SSD SATA)
- Fuente de alimentación (PSU)
- Caja / Chasis de PC (Case)
- Tarjeta gráfica dedicada (GPU, opcional según el procesador)
- Destornillador de estrella (PH2) y pulsera antiestática
- Memoria USB de arranque (mínimo 8 GB) con el instalador del Sistema Operativo
## Procedimiento 
1. **Preparación de la placa base:** Instalar el procesador (CPU) en el zócalo correspondiente alineando las marcas de posición, aplicar la pasta térmica (si el disipador no la incluye preaplicada) y fijar el sistema de refrigeración.

![alt text](image-14.png)

2. **Instalación de memoria RAM y almacenamiento M.2** Insertar los módulos de memoria RAM en las ranuras recomendadas (habitualmente ranuras 2 y 4 para *Dual Channel*) e instalar la unidad SSD NVMe M.2 asegurándola con su tornillo.

![alt text](image-18.png)

3. **Montaje en el chasis:** Montar la fuente de alimentación (PSU) en la caja y fijar la placa base utilizando los tornillos separadores (*standoffs*) de latón para evitar cortocircuitos.

![alt text](image-24.png)

4. **Conexión de cableado:** Conectar la alimentación principal (ATX 24 pines), la alimentación de la CPU (4/8 pines EPS), los cables del panel frontal (botón de encendido, LED, puertos USB) y los conectores PCI-Express de la tarjeta gráfica si corresponde.

![alt text](image-19.png)

5. **Primera puesta en marcha y BIOS/UEFI:** Enchufar el monitor, teclado y cable de corriente. Encender el equipo y pulsar la tecla `DEL` o `F2` para acceder a la BIOS/UEFI y verificar que reconoce la totalidad de la memoria y el disco duro.

![alt text](image-23.png)

6. **Instalación del Sistema Operativo:** nsertar el pendrive de arranque, seleccionar la unidad USB en el menú de inicio (*Boot Menu*) e iniciar el asistente de instalación del SO.

![alt text](image-20.png)

 
 ## Incidencias y soluciones

| Incidencias | Solución |
|---|---|
| El equipo no enciende ni emite señales de luz | Comprobar que el interruptor I/O de la fuente de alimentación esté en 'I' y revisar las conexiones de los pines `POWER SW` del panel frontal. |
| El PC enciende pero no da señal de vídeo | Asegurarse de que el cable HDMI/DisplayPort esté conectado directamente a la GPU dedicada y no a la placa base. Volver a insertar la memoria RAM firmemente. |
| El instalador del SO no detecta la unidad de disco | Acceder a la configuración de la BIOS y cambiar el modo del controlador SATA/NVMe de RAID/RST a modo AHCI. |
## Comprobaciones
- []La BIOS/UEFI reconoce la capacidad completa de la RAM y la frecuencia adecuada (perfil XMP/EXPO).
- []Las temperaturas del procesador en reposo (*idle*) se mantienen estables por debajo de los 45 °C.
- []Todos los ventiladores (chasis, disipador de CPU y fuente) giran correctamente y sin ruidos extraños.
- []El sistema operativo inicia correctamente, se detecta la tarjeta de red (cable o Wi-Fi) y hay conexión a Internet.

## Recursos
-[Cómo montar un PC](https://blog.jetcomputer.net/como-montar-un-pc/?srsltid=AU7gw4V8dSo-Sto8QJv5JivYlALBtyDTis8ajq6Q727XATR6IqfhHsdH)
-[instalación del SO](https://help.pccomponentes.com/hc/es-es/articles/30377918118685-Instalaci%C3%B3n-y-migraci%C3%B3n-de-Sistema-Operativo)

## Comandos de comprobación
 - sudo lshw 
 - sudo lshw -short 


[def]: /PC/Captura-de-pantalla-2026-04-28-a-las-8.30.04.png