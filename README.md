# Docker
- Os containers são isolados uns dos outros
- Um container só fica em pé enquanto o comando especificado estiver em execução
 - Quando o comando é finalizado o Docker derruba o container
- Aruivos vivem e morrem dentro dos containers

# Docker Compose
- Tudo que é feito pelo Docker em linha de comando pode ser feito facilmente com o Docker Compose

# Docker: IMAGE
- Fonte de somente leitura usada para subir container
## # Docker: Dockerfile
- Com o `Dockerfile` é possível criar `Docker Images`
- FROM...
- Comando que dever ser executado assim que o container estiver em pé CMD
- Libera um porta dentro do container : EXPOSE
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