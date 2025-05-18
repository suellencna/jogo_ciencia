# Jogo de Ciências Interativo com IA Gemini (@suellencna's Jogo de Ciências)

Um jogo de perguntas e respostas sobre Ciências para um público infantil/jovem (mas divertido para adultos também!). As perguntas são geradas por IA para um banco de opções dinâmico. Permite escolher o nível de dificuldade e apresenta um tom humorado para uma experiência leve e divertida.

## Como Funciona

O jogo inicia pedindo ao usuário para escolher um nível de dificuldade (inicial, médio ou avançado). Em seguida, uma pergunta de ciências é gerada pela IA Gemini de acordo com o nível escolhido. O jogador tenta responder, e o sistema fornece feedback imediato. Se a resposta estiver incorreta, uma dica é oferecida, e o jogador tem uma segunda chance. Após cada pergunta (correta ou incorreta), o jogador pode continuar no mesmo nível, mudar de nível ou parar o jogo.

## Tecnologias Utilizadas

- 'Python'
- Biblioteca `google-generativeai` (para interagir com a API do Google Gemini)
- Google Colab (ambiente de desenvolvimento recomendado)

## Como Executar no Google Colab

Para executar este jogo no Google Colab, siga estes passos:

1.  **Abra um novo notebook no Google Colab** (Arquivo -> Novo notebook).
2.  **Cole o código do arquivo `quiz_ciencia.py`** (o código do seu jogo) em uma ou mais células de código no notebook.
3.  **Configure sua API Key do Google Gemini como um "Segredo" no Colab:**
    * No menu à esquerda do Colab, clique no ícone de chave ("Segredos").
    * Clique em "**+ Adicionar um segredo**".
    * No campo "Nome", digite `GOOGLE_API_KEY` (exatamente assim, em maiúsculas).
    * No campo "Valor", cole a sua API Key do Google Gemini.
    * Clique em "**Salvar**".
4.  **Na primeira célula do seu notebook (antes do código do jogo), adicione o código para carregar a variável de ambiente da API Key:**

    ```python
    from google.colab import userdata
    import os
    os.environ['GOOGLE_API_KEY'] = userdata.get('GOOGLE_API_KEY')
    ```

5.  **Execute as células de código em ordem para iniciar o jogo.**

## Conteúdo dos Arquivos (Se Você Conseguiu Enviar Separadamente)

Se você conseguiu enviar os arquivos `.py` e/ou `.ipynb` separadamente:

* **`quiz_ciencia.py`:** Contém o código principal do jogo em Python.
* **`[nome_do_notebook].ipynb` (opcional):** É o notebook do Google Colab com o código e as instruções de execução.

## Participação na Imersão IA Alura 2025

Este projeto foi desenvolvido como parte da Imersão IA da Alura e Google Gemini 2025.

## Créditos

Agradecimentos à Alura e ao Google pela oportunidade de aprendizado e pela Imersão IA.

-----
