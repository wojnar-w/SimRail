# Instrukcje

## Scenariusz

- Pociąg osobowy z Katowic do Sędziszowa na scenerii lat 80.;
- Oczekiwanie na przyjazd pociągu osobowego z Wisły Głębce. Skład przechodzi na pociąg osobowy do Sędziszowa. 
- Po wejściu do kabiny należy wywołać na radiu ZEW1.

### Warunki użytkowania

Dziękuję za zainteresowanie scenariuszem! Stworzenie go wymagało sporo czasu i wysiłku, dlatego proszę o przestrzeganie kilku zasad:

1. **Konstruktywne zgłoszenia problemów**
   - Nie przyjmuję zgłoszeń typu 
     - *"U mnie nie działa"*
     - *"Scenariusz niewykonalny"*,
   - Wiadomości na priv w stylu 
     - *" ja mam kombinować robisz scenariusz i nie umiesz żeby dwa działały ja go robię czy to"* 
     - *"To zrób coś z tym zrobiłeś scenariusz a nie wiesz czego nie działa a kiedy to naprawisz?"*
    
    Takie komentarze nie wnoszą nic do rozwiązania problemu, ponieważ brak jest poniższych informacji 
    czyli:

2. **Wymagane informacje przy zgłaszaniu błędów**
   Aby umożliwić analizę i naprawę błędów, proszę dostarczyć:
   - **Logi z gry**:  
     Lokalizacja logów:  
     `%appdata%\..\LocalLow\SimKol\SimRail\MissionData\logs`
   - **Zrzut ekranu z okienka dialogowego w trybie debug**:
     - Włącz tryb debugowania w pliku `mission.lua`, zmieniając wartość na `true`:
       ```
       DeveloperMode = function()
           return true
       end
       ```
     - Po pojawieniu się błędu wykonaj zrzut ekranu z komunikatami, szczególnie po odpowiedzi dyżurnego.

Na podstawie tych informacji postaram się w miare wolnego czasu znaleźć rozwiązanie. Brak dostarczenia logów i zrzutów ekranu uniemożliwia rozwiązania problemu.
Chyba, że mówimy o czymś banalnym, jak korekta rozkładu, czy niepoprawny dialog, wtedy wystarczy informacja.


**Błędy**:
- Stacja Tunel - błąd wenętrzny symylatora zgłoszony (https://forum.simrail.eu/topic/10364-stacja-tunel-lata-80-perony-nie-wykrywaj%C4%85-poci%C4%85gu/#comment-44361), uniemożliwia wykonanie logiki
wyładowania pasażerów na stacji, w związku z tym, po otwarciu drzwi na stacji Tunel naliczane są kary, za otwarcie drzwi poza obszarem stacji, oraz, po ruszeniu ze stacj Tunel otrzymujemy komunikat o tym
, że minęliśmy punkt zatrzymania
- Stacja Sędziszów, po rozpoczęciu manewrów zjazdu na bocznicę otrzymujemy komunikat o minięciu punktu zatrzymania.
- nie znalezione błędy -> czytaj punkt Warunki użytkowania

## Instalacja

1. Wklej folder `Os-Katowice_Sedziszow` do ścieżki:  
   `..\SteamLibrary\steamapps\common\SimRail\SimRail_Data\StreamingAssets\Sceneries\4_The80s\Scenarios\`.

## Informacje dodatkowe

Scenariusz powstał całkowicie od zera. Ze względu na ograniczoną dostępność taboru z lat 80., 
obecnie wykorzystuję duplikaty jednostek EN57 (głównie 047) oraz elektrycznych lokomotyw w barwach zielonych lub zielonych z żółtymi czołami. W miarę jak SimRail będzie wydawać tabor z tamtych lat, duplikaty zostaną sukcesywnie usuwane.

Proszę o nie udostępnianie scenariusza w zmodyfikowanych składach pod lata współczesne, ponieważ na bazie tego scenariusza w niedługo ukaże się jego wersja dedykowana współczesnym realiom.

## Podziękowania

dla zespołou SimRail za wkład włożony w rozwój symulatora i możliwości tworzenia modyfikacji.
