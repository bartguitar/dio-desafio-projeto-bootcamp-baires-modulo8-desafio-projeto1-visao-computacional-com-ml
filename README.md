# dio-desafio-projeto-bootcamp-baires-modulo8-desafio-projeto1-visao-computacional-com-ml
Desafio de Projeto - Bootcamp Baires - Modulo 8 - Projeto 1

Assistente Virtual com Python

Este projeto é um assistente virtual local, que utiliza Processamento de Linguagem Natural (PLN) para transformar áudio em texto e executar comandos no computador, como abrir sites e responder com voz.

Funcionalidades

Módulo 1: Text-to-Speech (TTS)
Converte texto em fala usando gTTS e reproduz o áudio com playsound.

Módulo 2: Speech-to-Text (STT)
Converte arquivos de áudio (.mp3 ou .wav) em texto usando Whisper.

Módulo 3: Execução de comandos
A partir do texto reconhecido, o assistente executa comandos, como:

Abrir Google

Abrir YouTube

Responder com voz sobre o comando

Processa todos os arquivos de áudio em uma pasta automaticamente.

Pré-requisitos

Python 3.8 ou superior

Navegador instalado (Google Chrome, Firefox, etc.)

Instalação

Clone ou baixe este repositório.

Crie uma pasta chamada audios/ na mesma pasta do script.

Coloque os arquivos de áudio .mp3 dentro da pasta audios/.

Instale as dependências:

sudo apt update
sudo apt install python3-pip -y
pip3 install gTTS playsound pydub git+https://github.com/openai/whisper.git --user

Como usar

Abra o terminal na pasta do projeto.

Execute o script:

python3 assistente.py


O assistente irá:

Ler cada arquivo de áudio na pasta audios/

Falar o comando reconhecido

Abrir o site correspondente (Google ou YouTube)

Estrutura de pastas
/assistente/
│
├─ assistente.py         # Script principal
├─ audios/               # Pasta com arquivos de comando em MP3
│   ├─ abrir_google.mp3
│   └─ abrir_youtube.mp3
└─ README.md

Observações

Arquivos de áudio devem estar em português para melhor reconhecimento.

Para adicionar novos comandos, basta incluir novos arquivos MP3 na pasta audios/.

O script abre os sites no navegador padrão do seu computador.
