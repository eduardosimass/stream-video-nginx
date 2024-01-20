# Descrição do Projeto

Este projeto consiste em configurar um ambiente de streaming de vídeo usando Docker e Nginx.

## Arquivo docker-compose.yml

O arquivo `docker-compose.yml` é responsável por definir e configurar os serviços necessários para o ambiente de streaming de vídeo. Ele utiliza o Docker Compose para orquestrar os contêineres.

Aqui estão algumas das configurações presentes no arquivo `docker-compose.yml`:

- Definição dos serviços, como o serviço de streaming de vídeo e o serviço de banco de dados.
- Configuração das portas de rede para acessar os serviços.
- Definição das variáveis de ambiente necessárias para cada serviço.

## Arquivo nginx.conf

O arquivo `nginx.conf` é a configuração do servidor Nginx, que é usado como um proxy reverso para o serviço de streaming de vídeo. Ele direciona as solicitações de vídeo para o serviço correto e lida com o balanceamento de carga.

Aqui estão algumas das configurações presentes no arquivo `nginx.conf`:

- Definição dos servidores upstream para balanceamento de carga.
- Configuração das regras de roteamento para direcionar as solicitações de vídeo para o serviço correto.
- Definição das configurações de cache para melhorar o desempenho do streaming de vídeo.

## Como executar o projeto

Para executar o projeto, siga as etapas abaixo:

1. Certifique-se de ter o Docker e o Docker Compose instalados em sua máquina.
2. Clone este repositório em sua máquina local.
3. Navegue até o diretório do projeto.
4. Execute o comando `docker-compose up` para iniciar os serviços.
5. Acesse o streaming de vídeo em seu navegador usando o endereço fornecido.

## Como transmitir 

Abra o [OBS](https://obsproject.com/pt-br/download) > Configurações > Transmissão > Servidor
```
rtmp://localhost:1935/live
```

## Para assistir a transmissão 

No chrome com a [ MPEG-DASH + HLS Playback](https://chromewebstore.google.com/detail/native-mpeg-dash-+-hls-pl/cjfbmleiaobegagekpmlhmaadepdeedn) ou no Safari acesse: http://localhost:8081/live/.m3u8

## Contribuição

Contribuições são bem-vindas! Se você encontrar algum problema ou tiver alguma sugestão, sinta-se à vontade para abrir uma issue ou enviar um pull request.


## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
