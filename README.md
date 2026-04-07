
# Alke Wallet - Billetera Digital Proactiva 📱

![Android](https://img.shields.io/badge/Platform-Android-brightgreen.svg)
![Java](https://img.shields.io/badge/Language-Java-orange.svg)
![Architecture](https://img.shields.io/badge/Architecture-MVVM-blue.svg)

## 📝 Descripción
Alke Wallet es una solución de banca digital móvil que permite a los usuarios gestionar su capital, realizar transferencias virtuales y visualizar su historial financiero en tiempo real. Este proyecto representa la culminación del Módulo 6, integrando persistencia local y sincronización con servicios en la nube.

## 🛠️ Stack Tecnológico
- **Arquitectura:** MVVM (Model-View-ViewModel).
- **Base de Datos:** Room (Persistencia local con soporte Offline).
- **Networking:** Retrofit + GSON (Consumo de API REST).
- **UI:** Material Design, RecyclerView, LiveData.
- **Testing:** JUnit & Mockito.

## 🏗️ Estructura del Proyecto
- `data/`: Contiene los repositorios, DAOs de Room y servicios de Retrofit.
- `model/`: Entidades de datos y POJOs.
- `ui/`: Activities y Fragments.
- `viewmodel/`: Lógica de negocio y gestión del estado de la UI.

## 🔑 Características Principales
- **Acceso Offline:** Gracias a Room, el usuario puede ver su último saldo e historial sin conexión.
- **Seguridad:** Validación de fortaleza de contraseñas y cifrado de firma digital (JKS) para el release.
- **Sincronización:** Consumo asíncrono de API para transacciones globales.

## 🚀 Instalación
1. Clonar el repositorio.
2. Abrir en Android Studio.
3. Sincronizar Gradle y ejecutar en API 21+.

---
Desarrollado por **Felipe Leyton Pizarro** - Especialista en Soporte IT & Desarrollador Android.
