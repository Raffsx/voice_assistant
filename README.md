# voice_assistant
Assistente de voz, identifica comandos e realiza ações utilizando python e a API - Vosk.

Instalações dos componentes principais deste projeto:
1- Python 3.8.0: Realmente, até o momento só funciona se o python for "3.8.0"(Nem tente o 3.8.5), no windowns, a API Vosk é muito nova e ainda está sendo melhorada. Porém, é a única com modelo acústico pt-Br que funciona OFFLINE e que não precisa passar meses treinando modelo acústico.

2- Pipwin: "pipwin é como pip, mas instala binários pré-compilados do Windows fornecidos por Christoph Gohlke. Poupa muita procura no Google e downloads manuais." (Tomi Aarnio, usuário do stackoverflow).

3- API - Vosk: Realiza todo o trabalho "Pesado" deste projeto identificando as palavras ditas através do microfone ou de arquivos .WAV;

4- PYAUDIO -: Responsável por capturar o áudio do microfone e transferir à Vosk;

5- Vosk-model-small-pt-0.3: Pequeno (e único) modelo acústico em português pt-Br.

Instalação:
Instale primeiramente python 3.8.0 e remova qualquer outra versão do python existente da sua maquina. Em seguida instale o Pipwin (pip install pipwin). Agora instale o Pyaudio(pipwin install pyaudio) e ao finalizar instale a api-vosk(pip3 install vosk).
Teste:
Para testarmos utilizaremos os arquivos de teste da Api-vosk disponíveis no github "https://github.com/alphacep/vosk-api", baixe e descompacte, extraia também o seu modelo acústico, copie a pasta extraída acesse este diretório dentro do arquivo descompactado "\vosk-api-master\python\example", cole o modelo e renomeie para "model". Com o prompt de comando(CMD) ou Powershell ou VSCODE, navegue até a pasta "example" e execute o arquivo.py chamado "test_microphone", espere carregar e divirta-se. Faça alguns testes para ver a forma como a API consegue identificar a sua pronuncia, e as palavras que ela consegue identificar.

Observações e recomendações:
Recomendo fortemente acessar o site https://alphacephei.com/vosk/ dos criadores desta incrível API Cada item acima foi arduamente testado(hehehe) e houve muita cabeça quebrada até descobrir como tudo isso funcionaria. No linux a instalação é muito mais simples, bastaria o python de qualquer versão e um simples "pip3 install vosk && pip3 install pyaudio", mas tenho a mania de querer o mais difícil(kkkk).

Fontes:
https://alphacephei.com/vosk/ https://github.com/alphacep/vosk-api/issues/189#issuecomment-675278286 https://stackoverflow.com/questions/53866104/pyaudio-failed-to-install-windows-10
