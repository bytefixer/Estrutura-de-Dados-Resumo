## pré-ordem
```python
def pre_ordem(raiz):
	if not raiz:
		return
	print(raiz.chave, ", ", end="")
	pre_ordem(raiz.esquerda)
	pre_ordem(raiz.direita)
```
## em ordem
```python
def em_ordem(raiz):
	if not raiz:
		return
	em_ordem(raiz.esquerda)
	print(raiz.chave, ", ", end="")
	em_ordem(raiz.direita)
	
#talvez não precise
raiz = NodoArvore(40)
raiz.esquerda = NodoArvore(20)
raiz.direita = NodoArvore(60)
em_ordem(raiz)
```
## pós-ordem
```python
def pos_ordem(raiz):
	if not raiz:
		return
	pos_ordem(raiz.esquerda)
	pos_ordem(raiz.direita)
	print(raiz.chave, ", ", end="")
```
## inserção
```python
def insere(raiz, nodo):
	if raiz is None:
		raiz = nodo
	elif raiz.chave < nodo.chave:
		if raiz.direita is None:
			raiz.direita = nodo
		else:
			insere(raiz.direita, nodo)
	else:
		if raiz.esquerda is None:
			raiz.esquerda = nodo
		else:
			insere(raiz.esquerda, nodo)
			
#talvez não precise
raiz = NodoArvore(84)  
valores = [90, 200, 53, 12, 17, 9, 51, 86, 83, 85]  
  
for chave in valores:  
    nodo = NodoArvore(chave)  
    insere(raiz, nodo)
```
## busca
```python
def busca(raiz, valor):
	if raiz is None:
		return None
	if raiz.chave == valor:
		return raiz.chave
	if raiz.chave < valor:
		return busca(raiz.direita, valor)
	return busca(raiz.esquerda, valor)

raiz = NodoArvore(40)
valores = [20, 60, 10, 30, 50, 70]

for chave in valores:
	nodo = NodoArvore(chave)
	insere(raiz, nodo)
	
#talvez não precise
valor = 20
resultado = busca(raiz, valor)
if resultado:
	print(f"Busca pelo valor {valor}")
else:
	print(f"Busca pelo valor {valor}")
```
## código padrão de nó
```python
class NodoArvore:
	def __init__(self, chave=None, esquerda=None, direita=None):
		self.chave = chave
		self.esquerda = esquerda
		self.direita = direita
	def __repr__(self):
		return f'{self.esquerda and self.esquerda.chave} <- {self.chave} -> {self.direita and self.direita.chave}'

raiz = NodoArvore(30):
raiz.esquerda = NodoArvore(20)
raiz.direita = NodoArvore(40)
print("Árvore: ", raiz)
```
## código padrão de vários nós
```python
class NodoArvore:
	def __init__(self, chave=None, esquerda=None, direita=None)
		self.chave = chave
		self.esquerda = esquerda
		self.direita = direita
	def __repr__(self):
		return f'{self.esquerda and self.esquerda.chave} <- {self.chave} -> {self.direita and self.direita.chave}'

raiz = NodoArvore(3)  
raiz.esquerda = NodoArvore(1)  
raiz.esquerda.esquerda = NodoArvore(-2)  
raiz.esquerda.direita = NodoArvore(2)  
  
raiz.direita = NodoArvore(5)  
raiz.direita.esquerda = NodoArvore(4)  
raiz.direita.direita = NodoArvore(10)

print(" ", raiz)
print("  ", raiz.esquerda)
print("   ", raiz.direita)
```
## código rotação esquerda esquerda
```python
def rotacaoEsqEsq(raiz):  
    aux = NodoArvore(raiz.chave)  
    if raiz.direita:  
        aux.direita = raiz.direita  
    raiz.chave = raiz.esquerda.chave  
    raiz.esquerda = raiz.esquerda.esquerda  
    raiz.direita = aux
```
## código rotação direita direita
```python
def rotacaoDirDir(raiz):  
    aux = NodoArvore(raiz.chave)  
    if raiz.esquerda:  
        aux.esquerda = raiz.esquerda  
    raiz.chave = raiz.direita.chave  
    raiz.direita = raiz.direita.direita  
    raiz.esquerda = aux
```
## código rotação direita esquerda
```python
def rotacaoDirEsq(raiz):  
    aux = NodoArvore(raiz.chave)  
    aux2 = None  
    if raiz.esquerda:  
        aux.esquerda = raiz.esquerda          
    raiz.chave = raiz.direita.esquerda.chave  
    if raiz.direita.esquerda.esquerda:  
        aux2 = nodoArvore(raiz.direita.esquerda.chave)  
        aux2.esquerda = raiz.direita.esquerda.esquerda  
    if raiz.direita.esquerda.direita:  
        raiz.direita.esquerda = raiz.direita.esquerda.direita  
    else:  
        raiz.direita.esquerda = None  
    if aux2 and aux2.esquerda:  
        aux.direita = aux2.esquerda  
    raiz.esquerda = aux
```
## código rotação esquerda direita
```python
def rotacaoEsqDir(raiz):  
    aux = NodoArvore(raiz.chave)  
    aux2 = None  
    if raiz.direita:  
        aux.direita = raiz.direita          
    raiz.chave = raiz.esquerda.direita.chave  
    if raiz.esquerda.direita.direita:  
        aux2 = nodoArvore(raiz.esquerda.direita.chave)  
        aux2.direita = raiz.esquerda.direita.direita  
    if raiz.esquerda.direita.esquerda:  
        raiz.esquerda.direita = raiz.esquerda.direita.esquerda  
    else:  
        raiz.esquerda.direita = None  
    if aux2 and aux2.direita:  
        aux.esquerda = aux2.direita  
    raiz.direita = aux
```
## código de cálculo de altura
```python
def calcularAlturaNo(raiz):  
    if not raiz:  
        return    calcularAlturaNo(raiz.esquerda)  
    calcularAlturaNo(raiz.direita)  
    if not raiz.esquerda and not raiz.direita:  
        raiz.altura = 0  
    if raiz.esquerda and not raiz.direita:  
        raiz.altura = raiz.esquerda.altura + 1   
if not raiz.esquerda and raiz.direita:  
        raiz.altura = raiz.direita.altura + 1  
    if raiz.esquerda and raiz.direita:  
        if(raiz.esquerda.altura >= raiz.direita.altura):  
            raiz.altura = raiz.esquerda.altura + 1  
        else:  
            raiz.altura = raiz.direita.altura + 1
```
## código cálculo balanceamento
```python
def calcularFatorBalaceamentoNo(raiz,noDesbalanceado = None):  
    if not raiz:  
        return noDesbalanceado  
    noDesbalanceado = calcularFatorBalaceamentoNo(raiz.esquerda,noDesbalanceado)  
    noDesbalanceado = calcularFatorBalaceamentoNo(raiz.direita,noDesbalanceado)  
    if not raiz.esquerda and not raiz.direita:  
        fator = 0  
    if raiz.esquerda and not raiz.direita:  
        fator = raiz.esquerda.altura - (-1)  
    if not raiz.esquerda and raiz.direita:  
        fator = (-1) - raiz.direita.altura  
    if raiz.esquerda and raiz.direita:  
        fator = raiz.esquerda.altura - raiz.direita.altura  
    if(fator < 0):  
        fator = fator *(-1)  
    if(not noDesbalanceado and fator > 1):  
        noDesbalanceado = raiz.chave          
    return noDesbalanceado
```
