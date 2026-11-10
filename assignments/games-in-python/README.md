
# 📘 Assignment: Games in Python

## 🎯 Objective

Pratique strings, listas, condicionais, loops e entrada de dados criando um jogo da Forca em que a pessoa tenta descobrir uma palavra oculta antes de ficar sem tentativas.

## 📝 Tasks

### 🛠️ Implementar o Jogo da Forca

#### Descrição
Crie uma versão jogável da Forca no terminal. O programa deve escolher uma palavra de uma lista predefinida e permitir que a pessoa tente adivinhá-la, uma letra por vez.

#### Requisitos
O programa concluído deve:

- Selecionar aleatoriamente uma palavra de uma lista predefinida.
- Mostrar as letras descobertas e representar as letras ainda ocultas por `_`.
- Solicitar palpites até que a palavra seja descoberta ou o limite de tentativas incorretas seja atingido.
- Diminuir o número de tentativas restantes somente quando o palpite não estiver na palavra.
- Exibir uma mensagem de vitória com a palavra descoberta ou uma mensagem de derrota com a palavra correta.

### 🛠️ Validar os Palpites

#### Descrição
Melhore a interação do jogo validando as entradas e mantendo o controle das letras que já foram tentadas.

#### Requisitos
O programa concluído deve:

- Aceitar apenas um único caractere alfabético por palpite e pedir uma nova entrada quando ela for inválida.
- Informar quando a pessoa repetir uma letra já tentada, sem descontar uma tentativa.
- Exibir as letras já tentadas a cada rodada.
- Tratar letras maiúsculas e minúsculas como o mesmo palpite.