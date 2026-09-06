# ObraVoz v6
Versión sin SpeechRecognition del navegador.
Flujo: Android → micrófono → WAV → Vercel → Gemini 3.5 Transcribe → Gemini 3.7 Flash → ficha.
Despliegue: GitHub → Vercel → Environment Variables → GEMINI_API_KEY → Redeploy.
La clave nunca va en index.html.
Grabaciones limitadas a unos 2 minutos para evitar peticiones HTTP grandes.
