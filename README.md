# 📊 Automação de Relatório de Vendas

Projeto de automação desenvolvido em Python para envio diário de relatório de vendas por e-mail à diretoria.

## 💡 O que o projeto faz

1. Abre o navegador e acessa o Google Drive para baixar o arquivo de vendas do dia anterior
2. Lê o arquivo Excel com `pandas` e calcula os indicadores:
   - **Faturamento total**
   - **Quantidade de produtos vendidos**
3. Abre o cliente de e-mail e envia automaticamente um relatório para a diretoria

## 🛠️ Tecnologias utilizadas

- [Python 3](https://www.python.org/)
- [pyautogui](https://pyautogui.readthedocs.io/en/latest/) — automação de mouse e teclado
- [pandas](https://pandas.pydata.org/) — leitura e análise do arquivo de vendas
- [openpyxl](https://openpyxl.readthedocs.io/) — suporte à leitura de arquivos `.xlsx`

## ▶️ Como executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Abra o notebook `Projeto_2.ipynb` no Jupyter e execute as células em ordem.

## ⚠️ Configurações necessárias

Antes de executar, ajuste no notebook:

- **Caminho do arquivo:** altere a variável `caminho` para o local onde o arquivo de vendas é salvo no seu computador
- **E-mail do destinatário:** substitua `email_diretoria@suaempresa.com` pelo e-mail correto
- **Coordenadas de clique:** os valores de `x` e `y` no `pyautogui.click()` são específicos para a resolução de tela usada no desenvolvimento — use a célula utilitária ao final do notebook para descobrir as coordenadas corretas na sua tela

## 📁 Estrutura do projeto

```
📦 projeto
 ┣ 📓 Projeto_2.ipynb   # Notebook principal com a automação
 ┣ 📄 requirements.txt  # Dependências do projeto
 ┗ 📄 README.md         # Documentação
```
