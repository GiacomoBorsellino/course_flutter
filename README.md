# Introduzione a Flutter

## Cos'è Flutter?

Flutter è un framework open-source sviluppato da Google per la creazione di applicazioni multi-piattaforma con un'unica codebase. Permette di sviluppare app per **Android, iOS, Web, Windows, macOS e Linux** utilizzando il linguaggio **Dart**.

## Perché scegliere Flutter?

- **Single Codebase**: Scrivi il codice una sola volta ed eseguilo su più piattaforme.
- **UI Nativa e Prestazioni Elevate**: Utilizza il motore grafico Skia per garantire un rendering fluido.
- **Hot Reload**: Aggiorna il codice in tempo reale senza perdere lo stato dell'app.
- **Widget Personalizzabili**: Fornisce widget altamente flessibili per creare interfacce accattivanti.
- **Community e Supporto Google**: Ampia documentazione e supporto attivo.

## Installazione di Flutter

1. **Scaricare Flutter SDK**:
   - [Download Flutter](https://flutter.dev/docs/get-started/install)
2. **Aggiungere Flutter al PATH**
3. **Verificare l'installazione**:
   ```sh
   flutter doctor
   ```
4. **Installare un editor consigliato**:
   - [VS Code](https://code.visualstudio.com/) con estensione Flutter
   - [Android Studio](https://developer.android.com/studio)

## Creare un nuovo progetto Flutter

```sh
flutter create my_app
cd my_app
flutter run
```

## Struttura di un progetto Flutter

- `lib/main.dart` → Entry point dell'app
- `pubspec.yaml` → Gestione delle dipendenze
- `android/` e `ios/` → Configurazioni specifiche per le piattaforme
- `assets/` → Risorse come immagini e font

## Esempio di codice: "Hello, Flutter!"

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(title: Text('Hello, Flutter!')),
        body: Center(child: Text('Benvenuto in Flutter!')),
      ),
    );
  }
}
```

## Risorse Utili

- **Documentazione ufficiale**: [flutter.dev/docs](https://flutter.dev/docs)
- **Pub.dev (Pacchetti Flutter)**: [pub.dev](https://pub.dev/)
- **Dart Language**: [dart.dev](https://dart.dev/)
