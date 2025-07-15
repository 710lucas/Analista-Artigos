# Analisador de Artigos PDF 📄✨

Este projeto oferece uma solução automatizada para analisar artigos em formato PDF, extraindo informações relevantes e gerando análises detalhadas. Utiliza bibliotecas Python como `crewai`, `pdfminer.six` e `pdfplumber` para o processamento dos arquivos, além de modelos de linguagem (LLMs) para interpretação e análise de conteúdo.

---

## 🌟 Funcionalidades

* **Extração de Texto**: Lê e extrai texto de arquivos PDF. 📖
* **Análise de Conteúdo**: Utiliza um LLM para gerar resumos, insights ou informações personalizadas. 🧠💡
* **Geração de Relatórios**: Salva as análises em arquivos `.md` para consulta posterior. 📝

---

## 🧭 Como Funciona (Experiência do Usuário)

A aplicação oferece três modos de análise, cada um voltado para diferentes necessidades:

### 🔹 Modo Simples

* Análise totalmente automatizada.
* Gera um resumo do artigo, tópicos principais e possíveis aplicações.
* Ideal para leituras rápidas.

### 🔸 Modo Personalizado

* Permite inserir perguntas específicas ou comandos customizados.
* Indicado para análises direcionadas (ex: “Quais são as contribuições do artigo?”, “Como o autor trata o tema da educação?”).

### 🔷 Modo Misto

* Combina o resumo automático com respostas a perguntas personalizadas.
* Recomendado para revisões completas e aprofundadas.

A escolha do modo de operação é feita no próprio notebook, ajustando as variáveis de entrada ou os parâmetros das funções principais.

---

## 🚀 Requisitos

* Python 3.8 ou superior
* Dependências listadas em `requirements.txt`

---

## 🔧 Como Usar

### 1. Preparar os Artigos

Coloque seus arquivos PDF na mesma pasta onde está o notebook `Analista_de_artigos.ipynb`.

### 2. Configuração das Variáveis de Ambiente

Crie um arquivo `.env` com o seguinte conteúdo:

```env
GOOGLE_API_KEY="SUA_CHAVE_DE_API_AQUI"
MODEL_NAME="SEU_MODELO_DE_LINGUAGEM_AQUI"
```

Substitua com seus dados reais:

* `GOOGLE_API_KEY`: sua chave de API do Google.
* `MODEL_NAME`: nome do modelo (ex: `gemini/gemini-1.5-flash`).

📢 **Recomendado:** Utilize o [Google AI Studio](https://aistudio.google.com/app/apikey) para obter gratuitamente uma chave de API e acessar os modelos Gemini. Eles são potentes, acessíveis e de fácil integração.

### 3. Execução do Notebook

#### ✅ Ambiente Local

```bash
pip install -r requirements.txt
jupyter notebook  # ou jupyter lab
```

Abra o notebook `Analista_de_artigos.ipynb` e execute as células sequencialmente.

#### ☁️ Google Colab

1. Acesse o [Google Colab](https://colab.research.google.com/)
2. Faça upload do `Analista_de_artigos.ipynb`
3. No painel lateral esquerdo:

   * Clique em 📂 > ⬆ Upload dos PDFs
4. Configure as variáveis de ambiente usando o menu de “Secrets”:

   * Adicione `GOOGLE_API_KEY` e `MODEL_NAME`
   * Ative a opção "Notebook access"
5. Execute todas as células

---

## 📁 Estrutura do Projeto

```
.
├── Analista_de_artigos.ipynb
├── .env (opcional)
├── artigo1.pdf
├── artigo2.pdf
├── saida_artigo1.md
└── saida_artigo2.md
```

---

## 🤝 Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir *issues* ou enviar *pull requests* com melhorias, correções ou novas funcionalidades.

---

## 👌 Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---

📄 Desenvolvido com foco em automação inteligente de leitura e análise de artigos acadêmicos.

---
