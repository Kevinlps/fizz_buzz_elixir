# fizz_buzz_elixir

Este projeto implementa o famoso problema **FizzBuzz** utilizando a linguagem **Elixir**.  
O objetivo é processar uma lista de números e substituir valores de acordo com as seguintes regras:

- Múltiplos de **3** → `"Fizz"`
- Múltiplos de **5** → `"Buzz"`
- Múltiplos de **3 e 5** → `"FizzBuzz"`

## 📦 Pré-requisitos

- **Elixir** (versão mínima recomendada: 1.14 ou superior)
- Git instalado para clonar o repositório

## 🔧 Instalação

Clone o repositório e instale as dependências:

```bash
git clone https://github.com/Kevinlps/fizz_buzz_elixir.git
cd fizz_buzz_elixir
mix deps.get
```

## ▶️ Uso

Inicie o terminal interativo do Elixir:

```bash
iex -S mix
```

Então execute, por exemplo:

```elixir
# Executa o FizzBuzz com base no arquivo de entrada
FizzBuzz.build("numbers.txt")
```

Onde `numbers.txt` contém números separados por vírgula, exemplo:

```
1,2,3,4,5,15
```

Saída esperada:

```elixir
{:ok, ["1", "2", "Fizz", "4", "Buzz", "FizzBuzz"]}
```

## 📂 Estrutura do projeto

- **`lib/`** – Lógica principal da aplicação  
- **`test/`** – Testes automatizados (se existirem)  
- **`numbers.txt`** – Arquivo de exemplo com números para processar  

## ⚙️ Funcionamento

1. Lê o arquivo informado.
2. Converte o conteúdo em uma lista de números.
3. Aplica as regras do FizzBuzz.
4. Retorna uma tupla `{:ok, lista_resultante}` ou imprime no console.

## 🧪 Testes

Para executar os testes:

```bash
mix test
```

Exemplo de saída:

```
Finished in 0.03 seconds
3 tests, 0 failures
```
