## UNIFOR

**disciplina** Raciocinio logico algoritmico
**orientador** Prof Ricardo Carubbi

## lista de exercicios

### exercicio 03

#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite um número}}
B --> C[Numero]
C --> D{Numero > 0}
D --NÃO--> E{{O numero deve ser positivo!}}
E --> Z([FIM])
D --SIM--> F[resto = numero % 2]
F --> G{resto == 0}
G --NÃO--> H{{O numero é impar}}
G --SIM--> I{{O numero é par!}}
H --> Z
I --> Z


```
#### Pseudocodigo 
```
ALGORITMO verifica_par_impar
DECLARE numero, resto NUMERICO: "
ESCREVA "Digite um número: "
LEIA numero
SE numero >= 0 ENTAO
	resto <-  numero % 2 
	SE resto == 0 ENTAO
		ESCREVA "o numero é par!"
	SENAO
		ESCREVA "o numero é impar!"
	SENAO 
		ESCREVA "o numero deve ser positivo"
	FIM_ALGORITMO			
