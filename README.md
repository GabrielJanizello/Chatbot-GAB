# 🤖 Chatbot Gab: Um Assistente com a API do Google Gemini

Um chatbot interativo e carismático construído em **Python**, que utiliza a mais recente **API do Google Gemini**. Este projeto foi desenvolvido no ambiente **Google Colab** e serve como um exemplo prático de como criar, configurar e interagir com um modelo de linguagem de IA generativa de forma segura e eficiente.

---

## ✨ Funcionalidades

- **🧠 Personalidade Customizável**: O chatbot "Gab" possui uma personalidade pré-definida (carismático e objetivo) por meio de uma *system instruction*.
- **💬 Conversa Contínua**: Mantém o contexto da conversa, permitindo um diálogo fluido e natural.
- **🔐 Configuração Segura**: Utiliza o gerenciador de segredos do Google Colab para proteger sua chave de API.
- **🖥️ Interface Interativa no Console**: Experiência simples e direta de chat via terminal.
- **⚙️ Fácil de Executar**: Pronto para ser utilizado no Google Colab com configuração mínima.

---

## 🛠️ Tecnologias Utilizadas

- Python 3  
- Google Colab  
- Google Generative AI SDK (`google-generativeai`)  
- Modelo: `gemini-1.5-flash-latest`

---

## 🚀 Como Executar o Projeto

### 1. Obtenha uma Chave de API do Google

- Acesse o [Google AI Studio](https://makersuite.google.com/app).
- Faça login com sua conta Google.
- Clique em **"Get API key"** para gerar uma nova chave.
- Copie a chave gerada.

### 2. Configure o Ambiente no Google Colab

- Abra o arquivo `.ipynb` deste projeto no **Google Colab**.
- No menu à esquerda, clique no ícone de chave (🔑 Secrets).
- Clique em **"+ Add a new secret"**:
  - **Name**: `GOOGLE_API_KEY`  
  - **Value**: Cole a chave de API que você copiou.
- Ative a opção **"Notebook access"** para este segredo.

### 3. Execute as Células

- Com a chave de API salva, execute todas as células do notebook em ordem:
  1. A primeira célula instala as dependências.
  2. As próximas células configuram o modelo e iniciam o chat.

🎉 Agora você pode interagir com o Chatbot Gab diretamente no Colab!

---

## 📂 Estrutura do Código

O código está contido em um único notebook `.ipynb` e dividido em:

1. **Instalação da Biblioteca**: Instala o pacote `google-generativeai`.
2. **Configuração da API**: Carrega a chave de API a partir dos *Secrets* do Colab.
3. **Definição do Modelo**: Instancia o `gemini-1.5-flash-latest` e define sua personalidade via `system_instruction`.
4. **Início do Chat**: Cria um objeto de chat que mantém o histórico da conversa.
5. **Loop de Conversa**: Um `while` que captura a entrada do usuário, envia à API e exibe a resposta até que o usuário digite `"sair"`.

---

## 📜 Licença

Este projeto está sob a licença [MIT](LICENSE).

---

💬 Em caso de dúvidas ou sugestões, sinta-se à vontade para abrir uma *issue*!

