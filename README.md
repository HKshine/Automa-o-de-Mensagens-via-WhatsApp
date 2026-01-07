# 📲 Automação de Mensagens automática via WhatsApp
<img width="1015" height="477" alt="Captura de tela 2026-01-08 003208" src="https://github.com/user-attachments/assets/f0bcc1f4-41b5-4b48-a160-6e412fa709e3" />

Este projeto tem como objetivo **automatizar o envio de mensagens de cobrança para clientes via WhatsApp Web**, utilizando uma planilha Excel como base de dados. A automação permite enviar mensagens personalizadas em **datas específicas**, considerando **clientes com vencimentos diferentes**.

---

## 🎯 Objetivo do Projeto

> "Preciso automatizar minhas mensagens para meus clientes, informar valores e vencimentos, e permitir que entrem em contato comigo para explicar melhor. Quero poder mandar mensagens de cobrança em determinado dia, com clientes possuindo vencimentos diferentes."

Este script resolve exatamente esse problema, automatizando o processo de envio de mensagens de cobrança de forma prática e escalável.

---

## ⚙️ Funcionalidades

* 📊 Leitura automática de clientes a partir de uma planilha Excel (`clientes.xlsx`)
* 👤 Mensagens personalizadas com nome e data de vencimento
* 📅 Suporte a clientes com datas de vencimento diferentes
* 🔗 Inclusão de link de pagamento na mensagem
* 🤖 Envio automático via WhatsApp Web
* ❌ Registro de erros em arquivo `erros.csv`

---

## 🧰 Tecnologias Utilizadas

* **Python 3**
* **openpyxl** – leitura de arquivos Excel
* **pyautogui** – automação de cliques e teclado
* **webbrowser** – abertura do WhatsApp Web
* **urllib.parse** – codificação da mensagem

---

## 📁 Estrutura do Projeto

```bash
📦 automacao-whatsapp
 ┣ 📄 main.py
 ┣ 📄 clientes.xlsx
 ┣ 📄 erros.csv
 ┣ 🖼️ seta.png
 ┗ 📄 README.md
```

---

## 📊 Estrutura da Planilha (`clientes.xlsx`)

A planilha deve conter os seguintes dados na aba `Sheet1`:

| Nome | Telefone   | Vencimento |
| ---- | ---------- | ---------- |
| João | 2449XXXXXX | 2026-01-10 |

* **Telefone**: deve conter o código do país (ex: 244)
* **Vencimento**: formato de data reconhecido pelo Excel

---

## ▶️ Como Executar o Projeto

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/automacao-whatsapp.git
```

2. Instale as dependências:

```bash
pip install openpyxl pyautogui
```

3. Abra o WhatsApp Web no navegador e **mantenha-o logado**

4. Execute o script:

```bash
python main.py
```

⏳ O script aguarda 30 segundos para você confirmar o login no WhatsApp Web.

---

## ⚠️ Observações Importantes

* O arquivo `seta.png` deve ser uma **captura do botão de envio do WhatsApp**
* A automação depende da resolução da tela
* Não minimize o navegador durante a execução
* Uso recomendado apenas para **mensagens legítimas e autorizadas**

---

## 📌 Melhorias Futuras

* ⏰ Envio automático apenas para clientes com vencimento no dia atual
* 🗄️ Integração com banco de dados
* 🧠 Interface gráfica (GUI)
* 📱 Uso da API oficial do WhatsApp Business

---

## 🧑‍💻 Autor

**
Nerú Shine e Jhonatan de Souza
**
Automação • Python • Sistemas Web

---

## 📜 Aviso Legal

Este projeto utiliza automação do WhatsApp Web e **não é afiliado ao WhatsApp/Meta**. Use com responsabilidade para evitar bloqueios de conta.
