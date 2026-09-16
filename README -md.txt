1. Qual a principal vantagem de usar containers com Docker em vez de instalar um banco de dados e um servidor web diretamente em sua máquina?

A principal vantagem é o isolamento e a facilidade de configuração. Com Docker, o banco de dados e o servidor web ficam dentro de containers, sem precisar instalar e configurar tudo diretamente no sistema operacional. Isso também evita conflitos entre versões e facilita a criação do mesmo ambiente em diferentes computadores.

2. Explique com suas palavras o propósito de um Dockerfile. Por que ele é tão importante para a reprodutibilidade de ambientes?

O Dockerfile é um arquivo que contém as instruções para criar uma imagem Docker. Nele podemos definir o sistema, programas, dependências, configurações e comandos necessários para a aplicação funcionar.

Ele é importante porque permite criar o mesmo ambiente várias vezes, evitando que cada pessoa da equipe tenha que configurar tudo manualmente.

3. Em que cenário o Docker Compose se torna essencial? Por que não usar apenas comandos múltiplos docker run?

O Docker Compose é muito útil quando um projeto possui vários containers que precisam trabalhar juntos, como uma aplicação web, um banco MySQL e um servidor de apoio.

Em vez de executar vários comandos docker run e configurar cada container separadamente, podemos colocar todas as configurações em um arquivo docker-compose.yml e iniciar os serviços de forma organizada com um único comando.

4. Qual a importância dos volumes do Docker (como o que usamos para o banco de dados MySQL)? O que aconteceria com os dados se não usássemos um volume?

Os volumes servem para armazenar os dados fora do ciclo de vida do container. No caso do MySQL, eles permitem que os dados do banco continuem existindo mesmo se o container for removido ou recriado.

Sem um volume, os dados poderiam ser perdidos quando o container fosse removido, dependendo de como o armazenamento estivesse configurado.

5. Como o uso de containers pode facilitar o trabalho da equipe em um projeto de desenvolvimento de software?

Os containers ajudam a equipe porque todos podem trabalhar com o mesmo ambiente de desenvolvimento, usando as mesmas versões de programas, bibliotecas e configurações. Isso reduz problemas do tipo “na minha máquina funciona”.

Além disso, facilita a instalação, os testes, a implantação da aplicação e a reprodução do ambiente em outros computadores ou servidores.

Resumo: Docker facilita principalmente o isolamento, padronização, reprodução e compartilhamento dos ambientes de desenvolvimento.