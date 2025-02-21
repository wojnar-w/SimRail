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

----

# Instructions

## Scenario

- Passenger train from Katowice to Sędziszów in the 80s scenery;
- Waiting for the arrival of the passenger train from Wisła Głębce. The train then switches to the passenger train to Sędziszów.
- After entering the cabin, you need to call on the ZEW1 radio.

### Usage Conditions

Thank you for your interest in the scenario! Creating it took a lot of time and effort, so please follow a few rules:

1. **Constructive Issue Reporting**
   - I do not accept reports like:
     *"It doesn't work for me"*
     *"The scenario is unplayable"*,
   - Private messages like:
     *"Fix this, you've made the scenario but don't know what's wrong, when will you fix it?"*
   
   These comments don't contribute to solving the issue because they lack the following information:

2. **Required Information When Reporting Bugs**
   To allow for analysis and fixing of issues, please provide:
   - **Game Logs**:  
     Log location:  
     `%appdata%\..\LocalLow\SimKol\SimRail\MissionData\logs`
   - **Screenshot from the debug dialog box**:
     - Enable debug mode in the `mission.lua` file by setting the value to `true`:
       ```
       DeveloperMode = function()
           return true
       end
       ```
     - After the error appears, take a screenshot with the messages, especially after the response from the dispatcher.

Based on this information, I'll try to find a solution in my free time. Failing to provide logs and screenshots will make it impossible to solve the problem.
Unless we're talking about something trivial like schedule correction or incorrect dialogue, in which case a simple message will suffice.

**Bugs**:
- Tunel Station - internal simulator bug reported (https://forum.simrail.eu/topic/10364-stacja-tunel-lata-80-perony-nie-wykrywaj%C4%85-poci%C4%85gu/#comment-44361), prevents executing the logic for unloading passengers at the station, so after opening the doors at Tunel station, penalties are counted for opening the doors outside the station area, and after leaving Tunel station, we get a message saying we've passed the stopping point.
- Sędziszów Station, after starting maneuvers for the siding, we get a message about passing the stopping point.
- No errors found -> see Usage Conditions

## Installation

1. Paste the folder `Os-Katowice_Sedziszow` into the path:  
   `..\SteamLibrary\steamapps\common\SimRail\SimRail_Data\StreamingAssets\Sceneries\4_The80s\Scenarios\`.

## Additional Information

The scenario was created entirely from scratch. Due to limited availability of 80s-era rolling stock,  
I currently use duplicates of EN57 units (mainly 047) and electric locomotives in green or green with yellow fronts. As SimRail releases more rolling stock from that era, duplicates will be gradually removed.

Please do not share the scenario with modified compositions for modern times, as a version dedicated to modern realities will soon be released based on this scenario.

## Acknowledgements

To the SimRail team for their contribution to the development of the simulator and the ability to create modifications.
