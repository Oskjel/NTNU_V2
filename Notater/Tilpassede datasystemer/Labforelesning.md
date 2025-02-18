> [!tip]
> Du kan iterere gjennom array ved bruk av peker.

```
char* currentChar = &tekstreng[0]
while(*currentChar) {
	printf("%c", *currentChar);
	currentChar++;
}
```

> [!tip]
> Du kan overskrive datatype i kode
```
uint_32 a = 12;
uint_8 * p_a = (*uint_8)
```