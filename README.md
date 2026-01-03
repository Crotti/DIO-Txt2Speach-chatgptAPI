# DIO-Txt2Speach-chatgptAPI

Assistente de Voz: Pontos Turísticos com ChatGPT 🌍🎙️
Este repositório contém um notebook Jupyter projetado para rodar no Google Colab que funciona como um assistente de viagem por voz. O sistema captura o destino falado pelo usuário, identifica os principais pontos turísticos via IA e responde através de áudio sintetizado.

🚀 Funcionalidades
O projeto utiliza um pipeline de quatro etapas principais:

Gravação de Áudio: Captura a voz do usuário diretamente pelo navegador utilizando uma integração entre Python e JavaScript.

Reconhecimento de Fala (STT): Utiliza o modelo Whisper (base) da OpenAI para transcrever o áudio gravado em texto.

Processamento com ChatGPT: Envia o texto transcrito para a API da OpenAI para gerar uma lista dos 5 principais pontos turísticos do destino mencionado.

Sintetização de Voz (TTS): Converte a resposta textual do ChatGPT em áudio utilizando a biblioteca gTTS (Google Text-to-Speech).

🛠️ Tecnologias Utilizadas
Linguagem: Python 3.

Transcrição: OpenAI Whisper.

Inteligência Artificial: API OpenAI (GPT).

Sintetização de Áudio: gTTS.

Interface: Google Colab / JavaScript MediaStream API.

📋 Pré-requisitos
Para rodar este notebook, você precisará de uma chave de API da OpenAI.

Crie uma conta na OpenAI Platform.

Gere uma nova chave em API Keys.

No notebook, substitua o campo [PUT_YOUR_KEY] pela sua chave gerada.

📦 Instalação
As dependências necessárias são instaladas diretamente no notebook:

pip install git+https://github.com/openai/whisper.git -q
pip install --upgrade openai
pip install gTTS
📖 Como Usar
Abra o arquivo Auxiliar_Pontos_Turisticos_ChatGPT.ipynb no Google Colab.

Execute as células em ordem.

Na seção de gravação, clique em executar e diga o nome de uma cidade ou país quando solicitado.

O sistema processará sua fala e reproduzirá automaticamente a descrição dos pontos turísticos.

⚙️ Configuração
O idioma padrão do sistema está configurado para Português (pt), mas pode ser alterado na primeira célula do notebook:

Python

language = 'pt' # Altere para 'en' para Inglês, por exemplo.
