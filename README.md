aqui les dejare algunas posibles ayudas al crear o con problemas que puedan tener

si tienen algunos problemas o se les carga raro la imagen, posiblemente sea porque tienen una pantalla igual pero con un chip distinto, yo al inicio tuve problemas porque usaba librerias distintas a estas, la verdad me ha ayudado mucho gemini entonces no puedo decirles exactamente lo que deben hacer, pero tengan cuidado con eso, igualmente aunque no les funcione, pueden preguntarle a un agente de ia y adaptarla a sus pantallas 


#include <U8g2lib.h>
#include <Wire.h>
U8G2_SH1106_128X64_NONAME_2_HW_I2C u8g2(U8G2_R0, /* reset=*/ U8X8_PIN_NONE);


# ben10_aliens-code


este codigo me funciono para la pantalla 128x64 usa el protocolo i2c 
si quieren aportar aliens pueden comentarlo en el post de reddit,


creacion de personajes:
para crearlos necesitan entrar a este link: https://javl.github.io/image2cpp/

las configuraciones que yo use fueron estas:

1. suben la imagen normal sin mover nada
2. white
3. Scaling:scale to fit keeping proportions
4. Center image: horizontally
5. Draw mode: horizonal-1 bit per pixel
6. Swap bits in byte: [x] swap
7. generar code
   ya con eso se les deberia dar los parametros que deben copiar en el codigo de arduino que les puse, no necesitan copiarlo todo, hay 2 bloques que se generan ese ultimo bloque que luce asi "// Array of all bitmaps for convenience. (Total bytes used to store images in PROGMEM = 35904)
const int epd_bitmap_allArray_LEN = 1;
const unsigned char* epd_bitmap_allArray[1] = {
	epd_bitmap_GHSgSyKWwAAur12
};" , pueden quitarlo, solo copien y peguen lo de arriba
