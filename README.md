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
(https://media.licdn.com/dms/image/v2/D4D12AQEM9F_-u1OT5Q/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1658763190886?e=1753315200&v=beta&t=LzwgNsnzGbyIlUJnX3gOJN2SG-sjdXG-tbthX-1lNwI)

