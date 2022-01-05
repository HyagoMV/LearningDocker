# Docker
- Os containers são isolados uns dos outros
- Um container só fica em pé enquanto o comando especificado estiver em execução
 - Quando o comando é finalizado o Docker derruba o container
- Aruivos vivem e morrem dentro dos containers

# Docker Compose
- Tudo que é feito pelo Docker em linha de comando pode ser feito facilmente com o Docker Compose

# Docker: IMAGE
- Fonte de somente leitura usada para subir container
- Consiste em camadas de somente leitura
 - Para cada instrução contida no `Dockerfile` uma camada de somente leitura é criada
 - Ao criar um container apartir da image um nova camada de leitura e escrita é criada

### Docker: Dockerfile
- O Docker constrói imagens lendo as instruções de um `Dockerfile`
 - Um arquivo de texto em um formato específico que contém todos os comandos/instruções, **em ordem**, para construir uma imagem
- Com o `Dockerfile` é possível criar `Docker Images`
- FROM...
- Comando que dever ser executado assim que o container estiver em pé CMD
- Libera um porta dentro do container : EXPOSE
#### Referência
- https://docs.docker.com/engine/reference/builder/

# Docker: Build
- Controi uma imagem apartir de um `Dockerfile`

# Docker: RUN
- Sobe um container
``` Docker
> docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```
## Options
- Noméia o Container: --name
- Cria um Terminal Interativo: -it
- Sobe o Container em Background: -d
