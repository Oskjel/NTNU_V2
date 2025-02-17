
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
