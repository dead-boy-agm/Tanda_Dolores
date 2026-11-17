# Tanda Doloreña

Sistema de ahorro rotativo vecinal (tanda) construido con TDD en Flutter.

## Primeros pasos

Este paquete contiene `lib/`, `test/` y `pubspec.yaml`. Para obtener las carpetas de plataforma (android, ios, etc.), ejecuta desde esta carpeta:

```
flutter create .
flutter pub get
flutter test
flutter run
```

`flutter create .` no sobrescribe los archivos existentes de `lib/`, `test/` ni `pubspec.yaml`.

Si `flutter create .` genera `test/widget_test.dart`, bórralo: hace referencia a `MyApp` y ya no aplica.

## Estructura

- `lib/modelos/`: Participante, Tanda, CierreRonda
- `lib/logica/`: ServicioTanda y enums de resultado (Dart puro, sin imports de Flutter)
- `lib/presentation/`: TandaScreen (interfaz animada)
- `test/servicio_tanda_test.dart`: 11 pruebas de las rondas TDD más la de integración
