# cryptoHID



## Kurzbeschreibung

Komplexe Geräte wie Smartphones sind keine zu 100% vertrauenswürdige Geräte für einen Aufbau einer sicheren Kommunikation.
Ziel ist, die Entwicklung eines kleinen Open-Source-Gerätes, samt Smartphone-Companion-Software, welches in der Lage ist, verschlüsselte textbasierte Kommunikation über unsichere Kanäle zu leiten und dennoch eine Ende-zu-Ende-Verschlüsselung zu realisieren. Die Methodik dazu ist einen strikte Trennung von Überträger und Kryptoeinheit. Damit läuft zu keiner Zeit unverschlüsselte Kommunikation über das als unsicher anzusehende Gerät. Jegliche Ver- und Entschlüsselung wird auf ein externes Gerät ohne direkte Verbindung zum Internet oder anderen Netzen realisiert. Der Fokus bei der Entwicklung wird auf die Verwendung von frei verfügbaren und kostengünstigen Bauteilen gelegt.




-------
Tastatur 
```
,---,---,---,---,---,---,---,---,---,---,---,---,---,-------,
|1/2| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 0 | + | ' | <-    |
|---'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-----|
| ->| | Q | W | E | R | T | Y | U | I | O | P | ] | ^ |     |
|-----',--',--',--',--',--',--',--',--',--',--',--',--'|    |
| Caps | A | S | D | F | G | H | J | K | L | \ | [ | * |    |
|----,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'---'----|
|    | < | Z | X | C | V | B | N | M | , | . | - |          |
|----'-,-',--'--,'---'---'---'---'---'---'-,-'---',--,------|
| ctrl |  | alt |                          |altgr |  | ctrl |
'------'  '-----'--------------------------'------'  '------'
```
            |
           USB -Tastatur
            |
Raspberry Pi Zero W - mit Display                             
```                                
+--------------------------+           +-----------------------------+    
|() 2#################40 ()|           | Crypto HID  online          |
|   1#################39   |           |                             |
+---+    +--+   \/   ## RUN|           | crypted      a4lpg,a+ßlfsd  |
|MIC|    |  |  ()()  ## TV |           | encrypted    Geheimer Text  |
| SD|    +--+   ()         |-----------|                             |
+---+              Pi-Zero |           |                             |
|()+----+    +---+ +---+ ()|           | *Senden*                    |
+--|HDMI|----|USB|-|PWR|---+           +-----------------------------+    
   +----+    +---+ +---+
```

            |
        Bluetooth Verbindung
            |

Smartphone
```
      \   /    
    -=  o  =-  
      / | \    
        |      
        |      
        |      
     |=====|   
     |.---.|   
     ||=o=||   
     ||   ||   
     ||___||   
     |[:::]|   
     '-----'
 ```