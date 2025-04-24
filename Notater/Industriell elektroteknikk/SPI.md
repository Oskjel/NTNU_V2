Serial Peripheral Interface
Bussystem for å koble pereferieenheter i småskale

**Linjer:**

SCLK - serial clock styrt av master, synkronisert overføring av data
MOSI - Master out, Slave in, (data fra master til slave)
MISO - Master out Slave in (fra slave til master)

CS - chip select (aktiv lav), hvilken enhet styrt av master

Master SLAVE, kan ha flere selects 
RASK

![[Pasted image 20250414154314.png]]

PAralelle data sendes bit for bit
![[Pasted image 20250414154716.png]]
full duplex 
Når får bit in i MOSI får du bit ut i MISO så har kontinuerlig
dytter ut garbage når ingenting skal sendes, krever dummy-bytes

**Sendemetoder**

Serie med bytes
CS holdes lab mens sekvensen sendes 
til minneengeter

Korte kommander 
byte for byte 
Feks til AD omsetter

DAisy chain
Miso kobles på MOSI

![[Pasted image 20250414155329.png]]
Spare linjer, sender data gjennom slave
CS lik for alle og SCKL lik for alle

Dataformat

Abhenger av klokkepolaritet

lav polaritet, aktiv høy
Aktiv = høy, Idle = lav

lav polaritet aktiv lav

Se på hva som er iforhold til aktiv

MOSI og MISO gyldige 



