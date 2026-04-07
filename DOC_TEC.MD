# Informe Técnico de Implementación - Alke Wallet

## 1. Justificación de la Arquitectura (MVVM)
Se seleccionó **MVVM** sobre MVP para aprovechar la potencia de **LiveData** y los **ViewModels**. Esto permite que la aplicación sea resiliente a cambios de configuración (como rotaciones) y garantiza que la lógica de negocio no esté acoplada a la actividad, facilitando el mantenimiento a largo plazo.

## 2. Estrategia de Persistencia (Room)
Para cumplir con el requerimiento de "Acceso Rápido y sin Conexión", se implementó una base de datos SQLite gestionada por Room. 
- **Estrategia de caché:** El Repositorio actúa como mediador; siempre muestra datos de Room primero y actualiza la base de datos en segundo plano cuando la API de Retrofit responde con éxito.

## 3. Capa de Red (Retrofit)
La integración con la API REST se realizó mediante una interfaz de servicios desacoplada. Se implementaron:
- **Interceptors:** Para manejo de logs y debugging.
- **Converters:** GSON para transformar el JSON del servidor directamente en objetos de dominio.

## 4. Decisiones de Diseño y Seguridad
- **Firma Digital:** Se generó un almacén de claves **JKS** con algoritmo de cifrado fuerte para la distribución del APK/Bundle.
- **Manejo de Errores:** Se utiliza un sistema de estados (Loading, Success, Error) para que el usuario siempre sepa qué está ocurriendo en la aplicación.
