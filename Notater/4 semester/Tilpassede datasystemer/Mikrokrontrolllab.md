
Portmapped IO: aksesserer minnet via porter og separerer seg fra minneaddresering. bra for limited aksess

Memprymapped er vanlig minne

Makro for å spare minnet, oppretter ikke nytt objekt

## Volatile 
forteller kompilator at det som ligger på minneadresse kan endre seg når som helst

Hindrer optimalisering hvor variablen inngår

typecast kraftig les opp

```
IOREGS->OUT |= 1<<0 | 1<<4;
IOREGS->OUT = ~(1<<4)
```

Mer leselig med #define


##### Polling 
Sjekker status på ekstern enhet regelmessig, men tregt





##### Interrupts
programmet automatisk og avbryres når hendelser oppstår

- ISR (Interrupt  Service rutine)
	- Lagre CPUS tilstand
		- autogenerere kode
	- Bekrefte interrupt
	- utføre aksjoner
	- gjenopprette prosessorens tilstand
	Lett at skaper feil og disse feilene skaper race conditions som fører til feil
*Race condition*: Situasjon der utfallet avhenger av sekvensen eller timingen av uforutsette hendelser opererr på samme data

#### Watchdog-timere
Timer som resettes før interrupt
Resettes kontinuerlig til kode krasjer

> [!tip]
> Definerer ulike registre iforhold til baseadresse







```C


typedef struct {

    volatile uint32_t RESERVED0[321];

	volatile uint32_t OUT; // Write GPIO port 

    volatile uint32_t OUTSET; //Set individual bits in GPIO port

    volatile uint32_t OUTCLR; //Clear individual bits in GPIO port

    volatile uint32_t IN; //Read GPIO port

    volatile uint32_t DIR; //Direction of GPIO pins

    volatile uint32_t DIRSET; //DIR set register

    volatile uint32_t DIRCLR; //DIR clear register

    volatile uint32_t LATCH; //Latch register indicating what GPIO pins that have met the criteria set in the PIN_CNF[n]

    volatile uint32_t DETECTMODE; //Select between default DETECT signal behaviour and LDETECT mode

    volatile uint32_t RESERVED1[118]; 

    volatile uint32_t PIN_CNF[32]; //Configuration GPIO pins

} NRF_GPIO_REGO;

  
  

#define GPIO0 ((NRF_GPIO_REGO*)0x50000000);
```
Dette fungerer siden vi definerer baseadressen til structen under, og sekvensielt allokeres plass i minnet til alle utganger, 32-bit = 4 byte så er offset på 4 byte mellom mange av registrene