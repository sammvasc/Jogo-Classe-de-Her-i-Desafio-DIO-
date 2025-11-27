# Classe de Herói — Desafio DIO

Implementação simples e elegante de uma classe de herói em Python, utilizando Programação Orientada a Objetos.

## Funcionalidade
A classe representa um herói com:
- **nome**
- **idade**
- **tipo** (mago, guerreiro, monge, ninja)

E possui o método:
- **atacar()** → mostra a ação conforme o tipo de herói.

## Código

```python
class Heroi:
    def __init__(self, nome, idade, tipo):
        self.nome = nome
        self.idade = idade
        self.tipo = tipo

    def atacar(self):
        ataques = {
            "mago": "magia",
            "guerreiro": "espada",
            "monge": "artes marciais",
            "ninja": "shuriken"
        }

        ataque = ataques.get(self.tipo, "um ataque desconhecido")
        print(f"O {self.tipo} atacou usando {ataque}")
```

## Executando
```bash
python heroi.py
```

## Exemplo de saída
```
O ninja atacou usando shuriken
```

