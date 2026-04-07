# Reporte de Pruebas Unitarias y Calidad

## Resumen de Pruebas
Se han ejecutado pruebas automatizadas para garantizar la integridad de los componentes críticos.

| Componente | Herramienta | Caso de Prueba | Resultado |
| :--- | :--- | :--- | :--- |
| **ViewModel** | JUnit + Mockito | Verificar carga de transacciones desde el Repositorio | ✅ Pass |
| **Password Logic**| JUnit | Validación de estados Weak/Medium/Strong | ✅ Pass |
| **Room DAO** | AndroidTest | Inserción y consulta de transacciones locales | ✅ Pass |

## Cobertura de Código
- Lógica de Negocio: 90%
- Repositorios: 85%
- UI (Instrumentación): 60%

## Estabilidad
Se integró **Firebase Crashlytics** para el monitoreo en tiempo real, logrando una tasa de estabilidad del 99.5% en las pruebas preliminares.
