Standard for kommunikajson mellom enheter

## RS-232
Standard seriekommunikasjon 1 - til 1
Spenningsnivå, signalrate, timing
Brukes med UART

Dekker Fysisk lag og UART dekker Datalink

![[Pasted image 20250414150722.png]]
DTE: PC
DCE: Ekstern enhet

Full duplex: kan lese og sende sammtidig siden dedikerte linjer fir transmisjon

Sender til DCE og leser fra DCE

signal nivå:

$$
\begin{matrix}
0: \space [+3, +15]V \\
1: \space [-3,-15]V
\end{matrix}
$$
Stort område på grunn av dårlig signalkvalitet
Medfører litt tregt siden begrensing i hvor fort man kan gå fra + til - her
Felles jord, sårbar for støy
Enhver enhet må tilordnes ene eller andre rolle

Ingen spesifisering av flykontroll

RTS (request to send)
CTS (clear to sen


## RS-422


Løser viktigste utfordringer
lavere spenningsforskjeller ($\pm 0.4V$)
10Mbit/s
Full duplex
![[Pasted image 20250414151945.png]]
1-N kommunikasjon kan settes opp

# RS-485

Enheter som kan dele samme transmisjonslinje, fellesbuss
Adressering nødvendig, men ikke standarden

Billig og enkel feltbuss

Differensialspenning
Transmittere med 3-state logikk
setter høy impedans for å koble seg av dersom ikke i bruk

2 wire:
Mottaker tolker data Som 

$DATA = DATA(B)-DATA(A)$

![[Pasted image 20250414153209.png]]
flere kan koble seg på bussen til master
HALV duplex, bare mulig å enten sende eller lese
Alle kan kommunisere med alle

**Full duplex:**

![[Pasted image 20250414153413.png]]
Men da blir master slave struktur
slave kan bare kommunisere med master