# Aplicación de One Piece List

Una aplicación de Flutter que presenta una lista de personajes o elementos relacionados con One Piece, permitiendo navegar hacia una vista de detalle con animaciones fluidas.

## Tabla de Contenidos
- [Tecnologías utilizadas](#tecnologías-utilizadas)
- [Características](#características)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Configuración](#configuración)
- [Cómo ejecutar el proyecto](#cómo-ejecutar-el-proyecto)
- [Ejemplos de uso](#ejemplos-de-uso)
- [Estructura de carpetas](#estructura-de-carpetas)
- [Explicaciones de los módulos](#explicaciones-de-los-módulos)
- [Solución de Problemas](#solución-de-problemas)
- [Notas Adicionales](#notas-adicionales)

## Tecnologías utilizadas
- **Flutter**: Framework para el desarrollo multiplatforma.
- **Dart**: Lenguaje de programación utilizado por Flutter.
- **Cupertino Icons**: Iconografía estilo iOS.

## Características
- **Lista Interactiva**: Visualización de una colección de elementos con imágenes.
- **Vista de Detalle**: Pantalla detallada para cada elemento seleccionado.
- **Animaciones Personalizadas**: Implementación de efectos de desvanecimiento (`fade animation`) para una experiencia de usuario más pulida.
- **Diseño Moderno**: Uso de contenedores con efecto de desenfoque (`blur container`) y widgets personalizados.

## Requisitos
- [Flutter SDK](https://docs.flutter.dev/get-started/install) (versión >= 2.19.0 < 3.0.0)
- [Dart SDK](https://dart.dev/get-started/sdk)
- Un editor de código (VS Code, Android Studio o IntelliJ IDEA)

## Instalación
1. Clona el repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tenshi98/one_piece_app.git
   cd one_piece_app
   ```
2. Descarga las dependencias del proyecto:
   ```bash
   flutter pub get
   ```

## Configuración
Este proyecto no requiere configuraciones externas adicionales (como APIs o bases de datos), ya que utiliza activos locales almacenados en la carpeta `assets/`.

## Cómo ejecutar el proyecto
Asegúrate de tener un emulador abierto o un dispositivo físico conectado y ejecuta:
```bash
flutter run
```

## Ejemplos de uso
1. Al iniciar la aplicación, serás dirigido a la `HomePage`.
2. Desliza a través de la lista de elementos.
3. Haz clic en cualquier elemento de la lista para navegar a la `DetailPage` y ver más información y una imagen ampliada.
4. Regresa a la lista principal utilizando el botón de retroceso del dispositivo o la navegación de Flutter.

## Estructura de carpetas
```text
one_piece_app/
├── android/              # Configuración específica para Android
├── assets/               # Imágenes y recursos estáticos (.png, .jpg)
├── ios/                  # Configuración específica para iOS
├── lib/                  # Código fuente de la aplicación
│   ├── main.dart         # Punto de entrada de la aplicación
│   └── src/              # Código organizado por módulos
│       ├── animations/   # Animaciones personalizadas (ej. FadeAnimation)
│       ├── pages/        # Pantallas principales (HomePage, DetailPage)
│       └── widgets/      # Componentes de UI reutilizables
├── linux/                # Configuración específica para Linux
├── macos/                # Configuración específica para macOS
├── pubspec.yaml          # Definición de dependencias y activos
├── test/                 # Pruebas unitarias y de widgets
├── web/                  # Configuración específica para Web
└── windows/              # Configuración específica para Windows
```

## Explicaciones de los módulos
- **`animations`**: Contiene la lógica de las transiciones visuales, permitiendo que los elementos aparezcan o desaparezcan suavemente.
- **`pages`**: Define la estructura de las vistas. La `HomePage` gestiona la lista general y la `DetailPage` muestra la información específica de un elemento.
- **`widgets`**: Almacena componentes pequeños y reutilizables (como el `BlurContainer` o `HeaderWidget`) para evitar la duplicación de código y facilitar el mantenimiento.
- **`assets`**: Repositorio de todas las imágenes utilizadas en la interfaz de usuario.

## Solución de Problemas
- **Error de dependencias**: Si encuentras errores al ejecutar, intenta limpiar el proyecto y reinstalar dependencias:
  ```bash
  flutter clean
  flutter pub get
  ```
- **Errores de renderizado**: Asegúrate de que la versión de Flutter coincida con la especificada en `pubspec.yaml`.

## Notas Adicionales
Este proyecto fue desarrollado con fines educativos para demostrar el uso de widgets personalizados, navegación y animaciones básicas en Flutter.
