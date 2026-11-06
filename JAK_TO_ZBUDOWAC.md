
# AUDIOQUARRY - NATYWNA APKA KOTLIN - BEZ HTML

To nie jest HTML. To jest prawdziwy Kotlin + Jetpack Compose + AudioRecord.

## Co tu jest:
- MainActivity.kt - UI w Compose, 1 duzy przycisk, pady 4x4, presety
- AudioHunter.kt - AudioRecord 48kHz, pre-buffer 500ms, transient -35dB, cisza -45dB
- Dsp.kt - 4 presety w Kotlin: KICK / SNARE / PAD / GLITCH + ML klasyfikacja
- ZERO WebView, ZERO Chrome, ZERO index.html

## Jak dostac APK - TY NIC NIE MUSISZ UMIEĆ:
1. Wejdz na github.com/new -> stworz repo AudioQuarry
2. Wgraj ten folder (Upload files)
3. Zakladka Actions -> Build APK -> Run workflow
4. Po 3-4 min w Artifacts masz AudioQuarry-NATIVE-APK -> Pobierz -> Instaluj
5. Apka zapyta o mikrofon -> ZEZWOL -> kliknij LAP DZWIEK -> klasnij

## Jak z Android Studio (jak masz komputer):
Open -> wybierz ten folder -> Build -> Build APK(s)

## Dlaczego wczesniej mikrofon nie dzialal?
Bo wczesniej dawales Ci HTML otwierane z plikow - Chrome blokuje mic dla file://.
Tutaj mikrofon jest NATYWNY AudioRecord, prosi system o zgode od razu, dziala zawsze.
