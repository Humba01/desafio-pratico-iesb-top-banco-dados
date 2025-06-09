# desafio-pratico-iesb-top-banco-dados

## Mini tutorial

1. Realizar o clone desse repositório dentro da raiz da sua máquina Linux:
'''
$ git clone https://github.com/Humba01/desafio-pratico-iesb-top-banco-dados.git
'''

2. Entrar no diretório gerado pelo git clone:
'''
$ cd desafio-pratico-iesb-top-banco-dados/
'''
ou, se preferir renomeie a pasta como ''desafio-pratico-tbd-humba01''
'''
$ mv desafio-pratico-iesb-top-banco-dados desafio-pratico-tbd-humba01

$ cd desafio-pratico-tbd-humba01/
'''

3. Atualize os pacotes do sistema antes de instalar o docker:
'''
$ sudo apt update && apt upgrade
'''

4. Realize a instalação do docker:
'''
$ sudo apt install apt-transport-https ca-certificates curl software-properties-common

$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

$ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

$ sudo apt update

$ sudo apt-cache policy docker-ce

$ sudo apt-get install docker-ce make ntpsec

$ sudo systemctl status docker

$ sudo apt install docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

$ sudo docker run hello-world

$ sudo apt upgrade
'''

5. Agora, suba o ambiente dentro da pasta do repositório clonado:
'''
# se for a primeira execução 
$ sudo docker compose up --build

# depois da primeira execução
$ sudo docker compose up -d
'''

6. Depois de subir os containers, abra os endereços do Kibana e do Jupyter Notebook:
'''
# kibana
localhost:5601

# Jupyter Notebook 
localhost:8888
'''

7. Teste e aproveite.

