# 🐉 AI Dungeon Master: Mestre de RPG Interativo por Voz

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT_3.5_Turbo-green.svg)
![Whisper](https://img.shields.io/badge/Whisper-Speech_to_Text-yellow.svg)

## 📖 Sobre o Projeto
Este projeto transforma o seu navegador em uma verdadeira sessão de RPG de mesa. Utilizando tecnologias de ponta em Inteligência Artificial, um "Mestre de Jogo" automatizado com o qual você pode interagir 100% por voz. 

Diferente de simples chatbots de pergunta e resposta, este sistema possui **gerenciamento de contexto (memória)**, permitindo que a aventura tenha continuidade, consequências lógicas e uma narrativa imersiva estilo fantasia sombria e punitiva, onde cada escolha sua conta.

## ⚙️ Como Funciona o Fluxo (Pipeline)
1. **Ouvir (JavaScript + Colab):** O microfone capta a ação do jogador no navegador.
2. **Transcrever (OpenAI Whisper):** O áudio é convertido em texto com alta precisão.
3. **Pensar (OpenAI GPT-3.5/GPT-4):** O texto é processado por um LLM com um *System Prompt* rigoroso de Mestre de RPG, que analisa o histórico da aventura e gera a continuação da história.
4. **Falar (gTTS):** O Google Text-to-Speech converte a resposta do Mestre em áudio, lendo a narrativa para o jogador.

## 🎮 Exemplo de Interação
* **🧙‍♂️ Mestre (Voz):** Você está diante de um portão de ferro gigantesco coberto de musgo. O som de goteiras ecoa na escuridão. O que você faz?
* **🗡️ Jogador (Voz):** Eu pego minha tocha, acendo e tento empurrar o portão devagar.
* **🧙‍♂️ Mestre (Voz):** O portão range alto. A luz da sua tocha revela três goblins armados que se assustam com o barulho. Eles sacam suas adagas. O que você faz?

## 🚀 Tecnologias Utilizadas
* **Python** (Linguagem base)
* **OpenAI Whisper** (Reconhecimento de fala / Speech-to-Text)
* **OpenAI API** (Geração de texto e controle de narrativa)
* **gTTS** (Síntese de voz / Text-to-Speech)
* **Google Colab** (Ambiente de execução e integração com interface web)

## 🛠️ Como executar
1. Clone este repositório.
2. Abra o notebook no Google Colab.
3. Insira a sua `OPENAI_API_KEY` na célula de configuração.
4. Execute as células sequencialmente e comece a falar!
