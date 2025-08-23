# Maquina-de-Soldar-Furius-Fix-201
Maquina de Soldar Furius Fix 201

<img width="973" height="691" alt="imagen" src="https://github.com/user-attachments/assets/e67d7d10-b09e-4ce7-a6ad-ab87a8228b6a" />

---

# Información Técnica de Componentes - Tarjeta Soldador Furius XT201

## 1. Listado de Componentes y Números de Parte

| Componente                    | Número de Parte (P/N)         | Serigrafía / Referencia Interna                                          | Descripción Corta                                                              |
| :---------------------------- | :---------------------------- | :----------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| **IGBT**                      | **60T65PES**         | FW201-015 (Referencia UJUETA)                                       | IGBT de **60A y 650V**. Utilizado en los equipos FIX 200 y FIX 201. |
| **Diodos de Salida**          | **SFA70UP20DN**      | FW201-008 (Referencia UJUETA)                                       | Diodos ultrafast duales de **70A y 200V**. Ubicados en el disipador de salida. |
| **Diodos de Salida de T2**    | No especificado [conversation] | **D19, D18** [conversation]                                              | Diodos SMD a la salida del transformador T2 (el *chopper*) [conversation].     |
| **Puente Rectificador Principal** | **BR5010**           | **BR5010** (serigrafía en placa)                                    | Puente de diodos rectificador de **50A, 700V(rms) - 1000V(rrm)**. |
| **MOSFET Fuente Auxiliar**    | **K2611**            | **Q7** (en conversación), FW201-06C (Referencia UJUETA)             | Transistor MOSFET **9A-900V**. Encargado de la fuente auxiliar. |
| **Puente Rectificador Auxiliar** | **DBF310**                | **DB2** con serigrafía **DBF310** (mencionado previamente en conversación) | Rectificador de puente de montaje superficial de **3A y 1000V** VRRM. Adecuado para rectificación de onda completa AC a DC. |
| **Optoacoplador**             | **PC817** / **CT803** | No especificado [conversation]                                           | Optoacoplador, puede presentar cortocircuitos o aislarse.         |
| **Regulador de Voltaje**      | **L7815** (SMD)          | FW205-909 (Referencia UJUETA)                                       | Regulador de voltaje SMD de **15V**.                                  |

## 2. Medidas en Frío de Componentes (Modo Diodo)

| Componente                    | Tipo de Medición          | Valores Obtenidos (en polarización directa / mV) | Notas                                                                                                                                                                                                                                                                                                                             |
| :---------------------------- | :------------------------ | :----------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **IGBTs**                     | Modo diodo                | Entre los puntos 1 y 2: **378 mV**               | Se entiende el formato de los puntos de medición del IGBT. El datasheet del MBQ60T65PES no especifica una Vf directa para el IGBT, sino un **voltaje directo de diodo (VF)** de **1.45V** (típico a 25°C, IF=25A). Las mediciones en frío con multímetro suelen ser menores debido a la baja corriente de prueba. |
|                               |                           | Entre los puntos 2 y 3: **413 mV**               |                                                                                                                                                                                                                                                                                                                                   |
|                               |                           | Entre los puntos 1 y 3: **420 mV**               |                                                                                                                                                                                                                                                                                                                                   |
| **Diodos D19 y D18**          | Vf (voltaje directo)      | **440 mV** (ambos)                               | Estos diodos SMD se encuentran a la salida del transformador T2 (el *chopper*) [conversation]. No se tiene un datasheet específico para estos diodos.                                                                                                                                                                            |
| **Diodos de Salida**          | Vf (voltaje directo)      | **414 mV** (para ambos)                          | Se refiere a los diodos **SFA70UP20DN**. El datasheet del SFA70UP20DN especifica un **voltaje directo (VF)** típico de **0.96V** (a 25°C, IF=35A). Las mediciones en frío con multímetro suelen ser menores debido a la baja corriente de prueba, pero son consistentes entre sí.                                      |
| **Puente Rectificador Principal** | Vf (voltaje directo)      | **490 mV**                                       | Mediciones para los cuatro diodos internos del puente rectificador **BR5010 / FBR5010** [conversation, 16]. El datasheet del FBR5000 - FBR5010 especifica un **voltaje directo máximo por diodo (VF)** de **1.3 Volts** (a IF = 25A). Las lecturas son consistentes y significativamente menores que el máximo, lo cual es esperable. |
|                               |                           | **493 mV**                                       |                                                                                                                                                                                                                                                                                                                                   |
|                               |                           | **486 mV**                                       |                                                                                                                                                                                                                                                                                                                                   |
|                               |                           | **498 mV**                                       |                                                                                                                                                                                                                                                                                                                                   |

---

