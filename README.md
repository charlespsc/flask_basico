# Projeto Flask

Este projeto utiliza o framework Flask para desenvolvimento web em Python.

## Pré-requisitos

- Python 3.x instalado

## Configuração do Ambiente Virtual

1. **Crie o ambiente virtual:**
    ```bash
    python3 -m venv venv
    ```

2. **Ative o ambiente virtual:**
    - No Linux/Mac:
      ```bash
      source venv/bin/activate
      ```
    - No Windows:
      ```bash
      venv\Scripts\activate
      ```

3. **Instale as dependências: (se tiver)**
    ```bash
    pip install -r requirements.txt
    ```

4. **Instale o FLASK**
    ```bash
    pip install flask
    ```

## Executando o Projeto

1. **Defina a variável de ambiente do Flask:**
    ```bash
    export FLASK_APP=app.py
    export FLASK_ENV=development
    ```

2. **Primeiros passo com FLASK**
- Crie o arquivo index.py e adicione o seguinte conteúdo.
    ```bash
    from flask import Flask

    app = Flask(__name__)

    @app.route('/')
    def home():
    return "<h2>Hello, World!</h2>"
    ```

- Antes de executar você deve apontar o APP para o arquivo index
    ```bash
    export FLASK_APP=index.py
    ```


3. **Inicie o servidor:**
    ```bash
    flask run
    ```

## Estrutura do Projeto

```
Projeto_Flask/
├── .gitignore
├── LICENSE
├── venv/
├── index.py
└── README.md
```

## Licença

Este projeto está sob a licença MIT.