# Requerimientos no funcionales

| # | Atributo | Metrica | Umbral | Condicion de carga | Verificacion | Consecuencia si no se cumple |
|---|---|---|---|---|---|---|
| 1 | Rendimiento | p95 de latencia | menor a 400 ms | 200 usuarios concurrentes | Prueba de carga | El usuario abandona la operacion |
| 2 | Disponibilidad | Tiempo de actividad | mayor a 99.5% mensual | Operacion normal | Monitoreo continuo | El servicio queda inaccesible para los usuarios |
| 3 | Seguridad | Intentos de acceso no autorizado bloqueados | 100% de intentos detectados | Trafico normal y ataques simulados | Pruebas de penetracion | Exposicion de datos sensibles |

## Escenarios completos

### Escenario 1
- Fuente: Usuario final
- Estimulo: Realiza una consulta en hora pico
- Artefacto: Servicio de consultas
- Entorno: Operacion normal, 200 usuarios concurrentes
- Respuesta: El sistema responde dentro del umbral establecido
- Medida: p95 de latencia menor a 400 ms
