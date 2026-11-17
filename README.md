# Laboratorio 6: Reconocimiento de partes y funcionamiento de una máquina de anestesia (Mindray WATO EX-20)


## Integrantes
Paola Cepeda


## Contenido

1. [Introducción y objetivos](#1-introducción-y-objetivos)
2. [Procedimiento seguido](#2-procedimiento-seguido)
3. [Parte A: preguntas de revisión de literatura](#3-parte-a-preguntas-de-revisión-de-literatura)
4. [Parte B: identificación de partes y preguntas](#4-parte-b-identificación-de-partes-y-preguntas)
5. [Análisis de resultados](#5-análisis-de-resultados)
6. [Conclusión](#6-conclusión)
7. [Preguntas para la discusión](#7-preguntas-para-la-discusión)
8. [Bibliografía](#8-bibliografía)

---

## 1. Introducción y objetivos

Una máquina de anestesia mantiene al paciente en un estado estable de inconsciencia controlada, entrega oxígeno, mezcla gases y vapores anestésicos en la dosis indicada y ventila al paciente [1, 2]. En la práctica se trabajó con la Mindray WATO EX-20 del laboratorio.

**Objetivo general:** familiarizarse con los componentes, el funcionamiento y el mantenimiento de una máquina de anestesia.

**Objetivos específicos:**
- Identificar las partes principales de la WATO EX-20.
- Comprender su funcionamiento y modos de operación.
- Reconocer la importancia del mantenimiento.

## 2. Procedimiento seguido

1. Se asistió a la práctica demostrativa. 
2. Se fotografió el equipo desde varios ángulos (carpeta [`imagenes/originales`](imagenes/originales)), incluida la lista de verificación preoperatoria pegada a la máquina.
3. Se identificaron y numeraron las partes sobre las fotos ([`imagenes/anotadas`](imagenes/anotadas)).
4. Se consultó el manual del usuario del WATO EX-20 y fichas técnicas de Mindray para responder las Partes A y B. Cada dato se contrastó con el manual.
5. Se contaron los mensajes de falla del Apéndice D del manual por subsistema para el Análisis 2 ([`analisis`](analisis)).

### Equipo observado

![Panel frontal de la WATO EX-20]<img width="450" height="800" alt="02_panel_frontal_WATO_EX-20" src="https://github.com/user-attachments/assets/9d1fce7d-162f-41e3-965e-68b42ff6b36c" />


Panel frontal de la Mindray WATO EX-20. La pantalla estaba apagada y con película protectora. El equipo no tenía vaporizador instalado y solo se veía el soporte (manifold).

### Lista de verificación preoperatoria de la máquina

![Lista de verificación preoperatoria]<img width="450" height="800" alt="03_lista_verificacion_preoperatoria" src="https://github.com/user-attachments/assets/ad5168c0-5dfa-4477-9468-8e4703e25ce8" />


La tarjeta pegada a la máquina indica los pasos diarios antes de anestesiar:
- Con la máquina conectada a corriente alterna, poner el interruptor en ON, verificar que funciona con corriente alterna y completar la prueba de conformidad del sistema y fugas.
- Comprobar el mensaje de error y la alarma de suministro de O2, las alarmas de baja concentración de O2, presión alta o baja de vías respiratorias, volumen minuto bajo y apnea.
- Verificar que el sensor de O2 muestre cerca de 21 % en aire ambiente y más de 97 % tras exponerlo a 100 % de O2.
- Comprobar que los vaporizadores estén bien instalados, suficientemente llenos y con los puertos de llenado cerrados, y que solo se encienda uno a la vez.
- Hacer la prueba de presión retrógrada de cada vaporizador.
- Comprobar que el flotador del AGSS se mueve libremente y queda entre las líneas Min y Max.

---

## 3. Parte A: preguntas de revisión de literatura

### a. ¿Cuántos y cuáles son los tipos de anestesia que se aplican durante una cirugía?

Se describen tres tipos principales: general, regional y local. La sedación se trata como un cuarto grupo, porque la ASA considera la anestesia un continuo entre la sedación ligera y la anestesia general [5].

| Tipo | Explicación |
|---|---|
| **General** | El paciente queda inconsciente y no responde a estímulos dolorosos. Suele afectar la respiración, la presión arterial y la frecuencia cardíaca, por lo que requiere ventilación asistida. Es la que se administra con la máquina de anestesia (agentes inhalados e intravenosos). |
| **Regional** | Se inyecta anestésico cerca de los nervios que sirven la zona operada. Incluye bloqueo espinal, epidural y de nervios periféricos. El paciente puede estar despierto o sedado. |
| **Local** | Se inyecta el anestésico directamente alrededor del sitio quirúrgico (cirugías menores). |
| **Sedación** (mínima, moderada, profunda) | Reduce la ansiedad y el nivel de conciencia sin llegar a la anestesia general. En la sedación profunda el paciente cuesta despertarlo y puede necesitar apoyo respiratorio. |

### b. ¿Con qué gases trabaja la máquina y qué función cumple cada uno? ¿Cuáles entran por el sistema de alta presión?

| Gas | Función | Color en la máquina |
|---|---|---|
| **Oxígeno (O2)** | Sostiene la oxigenación del paciente. Además es el gas que activa el fuelle y se usa para el flush de O2 (botón **O2+**). Su pérdida dispara la alarma de falla de suministro de O2. | Verde |
| **Óxido nitroso (N2O)** | Gas analgésico y anestésico débil que acompaña al O2 y reduce la dosis necesaria de agente inhalado. Está enlazado al O2: el sistema mantiene el O2 por encima de aproximadamente 25 % y corta el N2O si el O2 cae. | Azul |
| **Aire medicinal** | Diluyente del O2. Permite bajar la FiO2 sin usar N2O. | Amarillo |

Además, el vaporizador agrega al flujo de gas fresco el agente inhalado líquido (sevoflurano, isoflurano, halotano, enflurano o desflurano, solo uno a la vez).

**Sistema de alta presión:** los gases que entran desde cilindros (O2, N2O y aire, instalados en los yugos de la parte trasera) pasan por el sistema de alta presión y luego por un regulador. Según el manual, los cilindros de O2 y aire están entre 6,9 y 20 MPa y el de N2O entre 4,2 y 6 MPa [6]. Los gases de la toma de pared (280–600 kPa) llegan por mangueras a presión intermedia. En la foto se ven los tres manómetros de toma de pared y **un solo manómetro de cilindro (O2)**. El espacio contiguo estaba vacío.

![Panel de gases y manómetros]<img width="450" height="1015" alt="06_panel_gases_anotado" src="https://github.com/user-attachments/assets/f8091b03-b32a-427a-a261-0414ed6bf643" />


### c. ¿Qué es el sistema de respiración y cuál es su función? ¿Qué partes se esterilizan en autoclave?

Es el circuito circular que conecta la máquina con el paciente. Sus componentes son las válvulas unidireccionales inspiratoria y espiratoria, el recipiente absorbente de CO2, el fuelle, la válvula APL, la bolsa de ventilación manual, el selector manual/mecánico, el manómetro de presión de vía aérea, el sensor de flujo, el sensor de O2 y las mangueras con la pieza en Y.

Su función es llevar al paciente la mezcla de gas fresco y vapor anestésico, recoger el gas exhalado, retirar el CO2 y reutilizar el gas restante (permite anestesia con bajos flujos). Permite ventilar de forma mecánica (fuelle) o manual (bolsa y APL).

**Autoclave (134 °C):** según el manual, la mayoría de las piezas del sistema de respiración se pueden esterilizar a 134 °C (se recomiendan 20 min). Los fuelles admiten 121 °C por 20 min o 134 °C por 7 min. **No** se autoclavan el manómetro de vía aérea, el sensor de flujo estándar, el sensor de O2, los tubos y frascos de succión ni el AGSS [6]. La marca 134 °C aparece grabada en el bloque del sistema de respiración (foto 7). El manual se contradice en un punto (la sección 10.3 menciona no autoclavar "el sistema de respiración y el sensor de O2" y la nota de autoclave permite todo menos manómetro, sensor de flujo y sensor de O2). Se debe confirmar con el técnico o el fabricante qué piezas exactas del equipo del laboratorio lo permiten.

### d. ¿Cuántos y cuáles son los submenús del ventilador? ¿En cuál se activa la pausa inspiratoria?

Con la tecla **Menu** se abre el menú principal con **cuatro submenús** [6]:
1. **Modo vent.** (modo de ventilación: VCV, PCV y ventilación manual).
2. **Config. alarma** (límites de alarmas, incluido el ventilador).
3. **Conf. usuario** (pantalla, sonido).
4. **Mantenimiento** (mantenimiento del usuario y ajustes del sistema).

La **pausa inspiratoria** (parámetro **TIP:TI**, "platô inspiratorio") se activa en el **modo VCV** (ventilación controlada por volumen). Aparece como tecla rápida al seleccionar VCV, con valores de 5 a 60 % del tiempo inspiratorio o apagada. En PCV no aparece.

> Pendiente de confirmar en el equipo real: la pantalla estaba apagada durante la práctica, por lo que el nombre exacto de los submenús se tomó del manual y no de la pantalla.

---

## 4. Parte B: identificación de partes y preguntas

### 1. Identificación y ubicación de las partes

Los números de las fotos corresponden a los de cada lista.

![Vista general anotada]<img width="450" height="1035" alt="01_vista_general_anotada" src="https://github.com/user-attachments/assets/234a3659-8761-48f0-b9a9-88cb7ce35e7b" />


![Bloque del sistema respiratorio visto desde arriba]<img width="450" height="975" alt="07_sistema_respiratorio_anotado" src="https://github.com/user-attachments/assets/628777ec-da8b-4d21-91e1-fa7471897178" />


![Fuelle, bolsa y mascarilla]<img width="450" height="895" alt="05_fuelle_y_mascarilla_anotado" src="https://github.com/user-attachments/assets/c7050336-c00b-4a1b-bc25-6b65ea51347e" />


| Parte | Ubicación | Función |
|---|---|---|
| **a. Vaporizador** | Sobre el soporte plateado con dos posiciones, a la derecha de los flujómetros (foto general, número 7). En la máquina del laboratorio no estaba instalado, solo se veía el soporte. | Convierte el agente anestésico líquido en vapor y lo mezcla con el gas fresco en la concentración elegida. Su dial se presiona y gira, con un seguro de posición. Nunca debe quedar encendido sin flujo de gas fresco, y solo debe usarse uno a la vez. |
| **b. Válvula APL** (*adjustable pressure-limiting*) | Perilla gris grande con escala de 10 a 50 cmH2O, en la parte inferior derecha del bloque respiratorio (foto 7, número 4; foto general, número 3). | Limita la presión del sistema durante la ventilación **manual** y libera el exceso de gas hacia el sistema de evacuación. En ventilación mecánica no actúa. |
| **c. Recipiente absorbente de CO2** | Cilindro transparente bajo el bloque respiratorio (foto general, número 2). En la foto estaba **sin cal sodada**. | Contiene cal sodada que absorbe el CO2 exhalado para poder reutilizar el gas. Cambia de color al agotarse. Se puede cambiar sin detener la ventilación (bypass de CO2). |
| **d. Fuelle** | Domo transparente con escala en mL (300, 600, 900), con una membrana negra dentro (foto general, número 1; foto 5, número 1; foto 7, número 6). | Al inspirar, el gas de accionamiento (O2) entra a la carcasa y comprime el fuelle, empujando el gas por el absorbedor hacia el paciente. Al espirar se llena con gas exhalado más gas fresco. Un fuelle ascendente indica un flujo de gas fresco adecuado y ausencia de fugas. |

Otras partes identificadas: flujómetros, perillas de flujo, manómetros de gases, bolsa manual y su brazo, selector manual/mecánico, válvulas unidireccionales, manómetro Paw, botón de flush de O2 (O2+), carro con frenos y mascarilla con filtro.

### 2. Si aparece "batería en uso" con el paciente conectado, ¿qué hacer?

Ese mensaje es de baja prioridad: indica que se perdió la corriente alterna y la máquina funciona con su batería (litio, unos 90 min con una batería y 150 min con dos). **No se debe apagar ni desconectar al paciente.** Se debe:
1. Revisar que el cable esté bien enchufado, el tomacorriente y el breaker, y reconectar a la red (al volver, el mensaje desaparece y aparece el ícono de carga).
2. Mantener la vigilancia del paciente y tener lista una bolsa de ventilación manual y una fuente de O2 de respaldo por si la batería se agota.
3. Si aparece la alarma de alta prioridad "Baja voltaje de la batería", conectar a la red de inmediato. Si la máquina queda inactiva por batería vacía, ventilar manualmente.
4. Avisar al personal de mantenimiento si la red no vuelve [6].

### 3. ¿Con qué frecuencia se reemplaza el recipiente absorbente de CO2?

El manual no fija un intervalo en horas. Se reemplaza cuando la cal sodada cambia de color de forma evidente y según el monitoreo de CO2 inspirado. En el manual de las A3/A5 de Mindray el criterio es cambiar cuando cerca de 2/3 del contenido está decolorado. También se reemplaza si el absorbente se seca por completo. Después de cambiarlo se debe hacer una prueba de fugas del sistema [6, 7].

### 4. Procedimiento para verificar fugas en el cilindro de alta presión

Según el manual del WATO EX-20 (sección 6.5) [6]:
1. Encender el sistema, desconectar el suministro de pared y cerrar todos los flujómetros.
2. Abrir la válvula del cilindro y registrar la presión.
3. Cerrar la válvula del cilindro y volver a registrar la presión después de 1 minuto.
4. Si la caída supera el límite del manual (más de 5 000 kPa en O2 o más de 700 kPa en N2O), hay fuga. Aire se prueba igual que O2.
5. Si hay fuga, cambiar el sello (empaque) del cilindro y repetir. Si persiste, no usar ese cilindro.

> El manual de servicio de las A3/A5 usa otro criterio (caída de no más de 10 % de la presión inicial en 1 minuto) [7]. Conviene verificar cuál aplica al manual del laboratorio.

### 5. ¿Influye contar con el sensor de O2 en la prueba del sistema de control de flujo?

**Sí.** El manual tiene dos versiones de la prueba [6]:
- **Sin monitoreo de O2 (6.7.1):** se sube el N2O por pasos (0,6; 1,5; 3,0 y 7,5 L/min) y se lee en el flujómetro que el O2 suba al mínimo de cada paso (≥0,2; ≥0,5; ≥1,0 y ≥2,5 L/min). Solo se comprueba el flujo, no la composición del gas.
- **Con monitoreo de O2 (6.7.2):** el sensor, **ya calibrado**, mide la concentración real de la mezcla, que debe ser **≥25 %** con N2O a flujo máximo. Así se comprueba directamente que no se pueda entregar una mezcla hipóxica.

Con sensor la prueba es más completa y segura, porque detecta errores que el flujómetro no ve (por ejemplo, una línea de gas cruzada). Por eso el sensor debe calibrarse antes (21 % en aire y 100 % en O2).

### 6. ¿Para qué se requiere el sistema de presión negativa?

Es un dispositivo de succión que usa el gas de la máquina (efecto Venturi) para generar vacío y aspirar secreciones, sangre y líquidos de la vía aérea y del campo quirúrgico cuando no hay vacío de pared. Tiene regulador, frasco de recolección con protección contra desbordamiento, tubo de aspiración y filtro. Opera en tres modos: TOTAL (presión máxima), OFF y *REG (se regula con la perilla). Debe dejarse en OFF cuando no se usa, para no gastar gas ni aumentar la concentración de O2 en el quirófano. En la inspección debe superar los -40 kPa [6]. En la máquina del laboratorio es el módulo bajo la bandeja (foto general, número 10, identificación probable).

---

## 5. Análisis de resultados

### Análisis 1: fallas posibles por subsistema y sus causas

El Apéndice D del manual lista las alarmas fisiológicas y técnicas [6]. Resumen de lo más frecuente:

| Subsistema | Fallas típicas | Causas habituales |
|---|---|---|
| **Suministro de gas** | Falla en el suministro de O2, baja presión de gas de unidad, flujo de gas fresco muy alto | Cilindro vacío o cerrado, manguera de pared desconectada, fuga, mal ajuste de flujómetros |
| **Sistema de respiración** | Circuito no montado, paciente desconectado, recipiente de CO2 no montado, VC no alcanzado, presión de vía aérea sostenida | Piezas mal ensambladas, fugas en conexiones o empaques, mangueras acodadas, absorbente agotado |
| **Ventilador** | Falla de válvula PEEP o inspiratoria, falla de sensor de flujo, errores de hardware 01 a 11, falla de comunicación | Sensor de flujo mojado o sucio, válvulas desgastadas, falla electrónica, necesidad de calibración |
| **Sensor de O2** | Calibrar o sustituir el sensor, sensor desconectado | Celda de combustible agotada (dura unos 13 meses), calibración deficiente, cable suelto |
| **Energía y batería** | Batería en uso, baja voltaje, batería no detectada, temperatura elevada | Corte de red, cable suelto, batería de litio degradada (se cambia cada 3 años) |
| **Alarmas fisiológicas** | Presión de vía aérea alta o baja, FiO2, VM, apnea, frecuencia | Cambios del paciente (obstrucción, desconexión, intubación) o límites mal ajustados |

### Análisis 2: subsistemas ordenados por número de fallas (mayor a menor)

![Fallas por subsistema]<img width="1000" height="550" alt="fallas_por_subsistema" src="https://github.com/user-attachments/assets/bd48a33e-10ef-4dff-95a8-9cfdbcb0d754" />


| # | Subsistema | Mensajes de falla |
|---|---|---|
| 1 | Ventilador y control | 28 |
| 2 | Energía y batería | 8 |
| 3 | Módulo de control auxiliar | 7 |
| 4 | Suministro de gas y vía aérea | 6 |
| 5 | Sistema y interfaz | 5 |
| 6 | Sensor de O2 | 3 |
| 7 | Sistema respiratorio | 3 |
| 8 | Módulo de calentamiento | 3 |
| 9 | Vaporizador | 0 |

El conteo se hizo sobre los mensajes técnicos del Apéndice D.2/D.3 del manual (los "errores de hardware 01 a 11" se contaron uno a uno). Los datos y el script están en [`analisis/`](analisis). Los subsistemas con más fallas son los de ventilador y energía, y el vaporizador no tiene alarmas propias en la tabla.

## 6. Conclusión

Las fallas que más se presentan al operar una máquina de anestesia se deben a errores de uso y de montaje más que a daños electrónicos: circuito o recipiente de CO2 mal ensamblado, fugas en conexiones, cilindros vacíos o cerrados, sensor de O2 sin calibrar, sensor de flujo húmedo y batería descargada por desconexión de la red. Esto coincide con la literatura, que señala que las fallas de las estaciones modernas suelen relacionarse con el usuario [3]. La lista de verificación preoperatoria y el mantenimiento programado (calibración del sensor de O2, cambio de empaques y baterías, drenado de vaporizadores) son la principal defensa. La práctica permitió reconocer cada subsistema (gases, vaporizador, ventilador y sistema de respiración con su absorbedor) y entender que el equipo no es tan complejo como parece [4].

## 7. Preguntas para la discusión

**Pregunta 1: ¿Qué tipos de anestésicos son los más usados en cirugía?**
- **Inhalados:** sevoflurano, isoflurano y desflurano (el sevoflurano es muy usado por su olor suave y rápida inducción), junto con el óxido nitroso como coadyuvante. Son los que entrega el vaporizador de la máquina.
- **Intravenosos:** propofol (inducción y mantenimiento), además de opioides como el fentanilo y relajantes musculares.
- **Locales y regionales:** lidocaína y bupivacaína.

El manual del WATO EX-20 admite halotano, enflurano, isoflurano, sevoflurano y desflurano, pero solo uno a la vez [6].

**Pregunta 2: ¿Qué diferencias plantea el EX-35 respecto al EX-20?**

| Característica | WATO EX-20 | WATO EX-35 |
|---|---|---|
| Pantalla | LCD a color de 7" | Más grande (10,4" táctil en la ficha actual de Mindray) |
| Modos de ventilación | VCV y PCV (PCV opcional según la ficha) | VCV, PCV, PS, SIMV-VC y SIMV-PC |
| Volumen corriente mínimo | 40 mL | 20 mL |
| Batería | 90 min (una) o 150 min (dos) | 150 min |
| Monitoreo de gases | Sin módulo de gases integrado | Módulo opcional de gases anestésicos y EtCO2 |
| Recipiente de CO2 | Recipiente de extracción rápida | Un solo recipiente de 1,5 L, con sistema respiratorio calefaccionado |
| Otros | Flujómetros mecánicos | Opción de succión de paciente y conmutación automática del gas de accionamiento |

Los datos provienen de las fichas técnicas citadas [8, 9, 10]. Las cifras pueden variar entre versiones y configuraciones del equipo.

---

## 8. Bibliografía

**De la guía:**
- [1] M. P. Dosch, *The Anesthesia Machine*, en *Nurse Anesthesia Secrets*, M. Karlet, Ed., 1ª ed., Philadelphia: Elsevier Health Sciences, 2005.
- [2] M. A. Sherwin y J. B. Eisenkraft, "Anesthesia hazards: What is the role of the anesthesia machine?", *International Anesthesiology Clinics*, vol. 58, no. 1, pp. 27–31, dic. 2020. https://doi.org/10.1097/AIA.0000000000000264
- [3] R. M. Dondelinger, "Anesthesia machines", *Biomedical Instrumentation & Technology*, vol. 38, no. 6, pp. 445–449, 2004.
- [4] I. S. Fischler, C. E. Kaschub, D. E. Lizdas y S. Lampotang, "Understanding of anesthesia machine function is enhanced with a transparent reality simulation", *Simulation in Healthcare*, vol. 3, no. 1, pp. 26–32, 2008. https://doi.org/10.1097/SIH.0b013e31816366d3

**Consultadas:**
- [5] American Society of Anesthesiologists, "Types of Anesthesia". https://community.asahq.org/dcsa/patients/anesthesia-types
- [6] Mindray, *Máquina de Anestesia WATO EX-20, Manual do usuário* (versión en portugués). https://cleanmedical.com.br/wp-content/uploads/2023/06/Manual-Usuario_Aparelho-Anestesia_Mindray-WATO-EX-20.pdf
- [7] Mindray, *A5/A3 Anesthesia System Service Manual*. https://ia902905.us.archive.org/19/items/manual_Mindray_A5_A3_Anesthesia_System_Service_Manual/Mindray_A5_A3_Anesthesia_System_Service_Manual.pdf
- [8] Mindray, *WATO EX-30/20 anesthesia machine* (ficha técnica). https://www.somatechnology.com/pdfFiles/Mindray-WATO-EX-30-20-anesthesia-machine.pdf
- [9] Mindray, *WATO EX-35 anesthesia machine* (ficha técnica). https://www.somatechnology.com/pdfFiles/Mindray-WATO-EX-35-anesthesia-machine.pdf
- [10] Mindray, "WATO EX-35". https://www.mindray.com/uk/products/anesthesia/wato-ex-35
