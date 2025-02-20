# mobile_swifty_protein

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## LAUNCH SCREEN
Also called splash screen.
[1st.-] In terminal, in the project directory, execute: flutter pub add flutter_native_splash
[2nd.-] In the project directory, create a directory with the images for the launch sreen (in our case assets/splash/) and put the images there
[3d.-] In pubspec.yaml add the subdirectory (in my case the subdirectory is assets/splash/) with the images under sections flutter: and assets:
flutter:
  assets:
    - assets/splash/
[4th.-] In the project directory Create a file named *.yaml (in my case native_splash.yaml) and fill it in with the files and background color:
flutter_native_splash:
  android: true
  ios: true
  web: true

  background_image: "assets/splash/background.png"
  image: "assets/splash/splash_logo.png"
  branding: "assets/splash/launch_screen.png"

  background_image_dark: "assets/splash/background_dark.png"
  image_dark: "assets/splash/splash_logo.png"
  branding_dark: "assets/splash/launch_screen.png"

  android_12:
    color: "#ff0000"
    image: "assets/splash/splash_logo.png"
    branding: "assets/splash/launch_screen.png"
[5th.-] In terminal, in the project directory, execute (beware the name of the .yaml file, which in my case is native_splash.yaml): dart run flutter_native_splash:create --path=native_splash.yaml


## Icono de la aplicación
Poner un icono a la aplicación Flutter

1.- En la terminal, en el directorio del proyecto, ejecutar: flutter pub add flutter_launcher_icons

2.- A continuación ejecutar: dart run flutter_launcher_icons:generate
Esto generará un fichero llamado flutter_launcher_icons.yaml en el directorio del proyecto

3.- Copiar el logo de la aplicación a una carpeta. Por ejemplo: assets/icons/

4.- Editar flutter_launcher_icons.yaml para indicar la carpeta donde se encuentra el icono de la aplicación, y cambiar algún color.

5.- Ejecutar:
flutter pub get
dart run flutter_launcher_icons
