# Exercício — Dicionários em Python

## Objetivo
Praticar a criação, consulta, alteração, adição e remoção de elementos em um dicionário.

## Código

```python
sensor = {
    'id': 'T01',
    'local': 'linha 3',
    'temp': 25.0
}

# Consultando valores
print(sensor['local'])
print(sensor['temp'])

# Alterando um valor existente
sensor['temp'] = 26.4

# Adicionando uma nova chave
sensor['ativo'] = True

# Consultando uma chave que pode não existir
print(sensor.get('umid', 'n/d'))

# Removendo uma chave
del sensor['ativo']

# Consultando a quantidade de elementos
print(len(sensor))
```

## Conceitos praticados

- `dict`: estrutura que armazena dados em pares de chave e valor.
- `sensor['local']`: acessa o valor associado à chave `local`.
- `sensor['temp'] = 26.4`: altera um valor existente.
- `sensor['ativo'] = True`: adiciona uma nova chave ao dicionário.
- `get()`: consulta uma chave e permite definir um valor padrão caso ela não exista.
- `del`: remove uma chave e seu valor.
- `len()`: retorna a quantidade de pares existentes.

## Resultado esperado

- Local: `linha 3`
- Temperatura inicial: `25.0`
- Umidade: `n/d`
- Quantidade final de elementos: `3`

## Observação
A chave `ativo` é removida antes da contagem final. Por isso, o dicionário termina com três elementos: `id`, `local` e `temp`.
