# Certificados Unifacisa 📃

Um script que gera automaticamente certificados personalizados usando dados de arquivos `.xlsx` ou `.csv`.


## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Como Funciona](#como-funciona)
- [Instalação](#instalação)
- [Uso](#uso)
- [Estrutura do Projeto](#estrutura-do-projeto)

## Sobre o Projeto

O **Certificados Unifacisa** é um script desenvolvido para automatizar a geração de certificados. Ele lê dados de um arquivo `.xlsx` ou `.csv`, e insere essas informações em um template de certificado, gerando um arquivo PDF para cada entrada de dados.

## Como Funciona

1. **Entrada de Dados**: O script aceita arquivos de entrada nos formatos `.xlsx` ou `.csv`, que devem conter as informações necessárias para preenchimento dos certificados.
2. **Template de Certificado**: Um template de certificado no formato imagem (`.png` ou `.jpg`) é usado como base.
3. **Geração de Certificados**: Utilizando bibliotecas de manipulação de imagens e PDFs, o script insere os dados do arquivo de entrada no template e gera os certificados individualmente em formato PDF.

## Instalação

### Pré-requisitos

- Python 3.x
- Bibliotecas necessárias (indicadas no arquivo `requirements.txt`)

### Passos

1. Clone o repositório:
    ```bash
    git clone https://github.com/usuario/certificados-unifacisa.git
    ```
2. Navegue até o diretório do projeto:
    ```bash
    cd certificados-unifacisa
    ```
3. Crie um ambiente virtual (opcional, mas recomendado):
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```
4. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

## Uso

1. Coloque seu arquivo de dados (`.xlsx` ou `.csv`) no diretório de entrada.
2. Coloque o template de certificado na pasta especificada no código.
3. Execute o script:
    ```bash
    python gerar_certificados.py --input dados.xlsx --template template.png
    ```

### Exemplo de Arquivo de Dados

| Nome          | Curso          | Data       |
| ------------- | -------------- | ---------- |
| João da Silva | Python Básico  | 01/01/2024 |
| Maria Souza   | Data Science   | 02/02/2024 |

## Estrutura do Projeto

```plaintext
certificados-unifacisa/
├── data/
│   ├── input/
│   │   └── dados.xlsx
│   └── output/
├── templates/
│   └── template.png
├── gerar_certificados.py
├── requirements.txt
└── README.md
```

##Autores

- [Rafael Macedo](https://github.com/rafaelmacedos)
- [Darllinson Azevedo](https://github.com/darllinsonazvd)
- [Pedro Azevedo Teixeira](https://github.com/pedro-azevedo3)
- [Pedro Henrique Pereira](https://github.com/pedrohpdo)
