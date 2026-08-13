OBRAVOZ v3 - Android dictado

Cambios principales:
- Dictado continuo en español (es-ES) usando SpeechRecognition/webkitSpeechRecognition cuando el navegador lo permite.
- La app intenta mantener la sesión de dictado continua y procesa el texto después de terminar, en lugar de interpretar palabra por palabra.
- Solicita acceso al micrófono con getUserMedia cuando está disponible.
- Detecta automáticamente la obra a partir del nombre mencionado.
- Extrae trabajo, material usado, material pendiente y próxima visita mediante frases habituales.
- Guarda los datos localmente en el navegador.

Para probar:
1. Publicar en HTTPS (GitHub Pages sirve).
2. Abrir con Chrome en Android.
3. Crear una obra llamada, por ejemplo, "Juan".
4. Nueva visita -> Empezar a dictar.
5. Decir de corrido: "Obra Juan. Hoy hemos terminado el baño. He usado diez metros de tubo. Hay que traer dos llaves de paso. Volvemos el viernes."
6. Parar -> revisar -> guardar.

Nota:
Esta versión sigue dependiendo de las capacidades de reconocimiento de voz del navegador/Android. No usa una API externa de transcripción ni cobra por voz. Para una transcripción realmente robusta en cualquier móvil, el siguiente paso sería usar un motor de transcripción del lado servidor.
