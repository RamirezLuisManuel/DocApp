## Control de versiones
### Tecnologias a usar 
#### Mi  (mane) propuesta
Node.js 24 lts +
Angular 20 +
Typescript 5.8 +
MySQL 8.4 LTS

#### En base a documentacion oficial
| Escenario                                | Stack sugerido                                        | Ventaja                                                          | Riesgo                                                                                 |
| ---------------------------------------- | ----------------------------------------------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| **Máxima estabilidad**                   | **Node 20 LTS + Angular 20 + TS 5.8 + MySQL 8.0.x**   | Todo el ecosistema ampliamente probado en producción.            | MySQL 8.0 tendrá soporte un poco más corto que 8.4.                                    |
| **Largo plazo / “bleeding-edge seguro”** | **Node 22 LTS + Angular 20 + TS 5.8 + MySQL 8.4 LTS** | Más años de soporte oficial, buena relación estabilidad/novedad. | Algunas librerías pueden tardar en adaptarse a MySQL 8.4.                              |
| **Último LTS absoluto**                  | **Node 24 LTS + Angular 20 + TS 5.8 + MySQL 8.4 LTS** | Lo más nuevo, mayor horizonte de soporte.                        | Mayor riesgo de dependencias que aún no declaran compatibilidad explícita con Node 24. |


### Conversacion con chat 
https://chatgpt.com/share/68d741e6-5634-8001-8547-fe576f642cdc

Datos importantes que dio chat:

Si este proyecto entra pronto en producción y necesitas cero sorpresas,
👉 Node 20 LTS + Angular 20 + TypeScript 5.8 + MySQL 8.0.x (o 8.0.37+) es hoy el sweet spot.
Todo está documentado y probado, y podrás migrar a Node 22/24 o MySQL 8.4 en el futuro con upgrades graduales.

Si el proyecto es a largo plazo (1 año de desarrollo) y puedes testear drivers,
👉 puedes subir a Node 22 LTS + MySQL 8.4 LTS para maximizar vida útil.

#### La que para mi (mane) es la mejor propuesta

Node 22 LTS + Angular 20 + TS 5.8 + MySQL 8.0 es probablemente el mejor “sweet spot” hoy:

Más soporte futuro que Node 20.

Menos riesgo que Node 24.

MySQL 8.0 garantiza máxima compatibilidad de drivers.
