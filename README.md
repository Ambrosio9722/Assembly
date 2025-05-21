# Assembly

# Repositório dedicado a projetos envolvendo a linguagem de programação Assembly


#include <stdio.h>
```c
ORG 2000H
    DB 'H', 'E', 'L', 'L', 'O', 0  ; String a ser enviada

ORG 2100H
    LXI H, 2000H      ; HL aponta para o início da string
LOOP:
    MOV A, M          ; Carrega o caractere atual em A
    CPI 0             ; Compara com 0 (fim da string)
    JZ END            ; Se for 0, fim do programa
    OUT 01H           ; Envia A para a porta 01H (simulando uma saída de vídeo)
    INX H             ; Vai para o próximo caractere
    JMP LOOP
END:
    HLT               ; Fim
```
![Assembly]
([https://upload.wikimedia.org/wikipedia/commons/3/30/Assembly_language_logo.svg](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.pinterest.com%2Fpin%2F450289662744269419%2F&psig=AOvVaw1yjNSieu1dvdInJEneP0ip&ust=1747882566244000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCOid7IzIs40DFQAAAAAdAAAAABAE))

