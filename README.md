# APP-NODE
Este é um exemplo de arquivo README para o projeto que utiliza Docker e Node.js para criar um servidor web simples. O servidor exibe uma página HTML básica que diz "Eu amo Docker!".

## Pré-requisitos
Certifique-se de ter instalado o Docker em sua máquina antes de prosseguir.

## Instruções de uso
Clone este repositório em sua máquina local.

Navegue até o diretório raiz do projeto.

Abra o arquivo Dockerfile e verifique a versão do Node.js especificada na linha FROM. Certifique-se de que você tenha a versão correta do Node.js instalada. Caso necessário, atualize o arquivo para uma versão compatível.

Abra um terminal e navegue até o diretório raiz do projeto.

Execute o seguinte comando para construir a imagem Docker:

docker build -t valterlafuentejr/app-node:latest .

Após a conclusão da construção da imagem, execute o seguinte comando para iniciar um contêiner Docker:

docker run -p 8080:3000 valterlafuentejr/app-node:latest

Aguarde até que o servidor esteja em execução. Você verá uma mensagem no terminal indicando que o servidor está ouvindo na porta 8080.

Abra um navegador da web e acesse http://localhost:8080 para ver a página "Eu amo Docker!".

Para interromper a execução do servidor, pressione Ctrl + C no terminal.

## Estrutura do projeto
O arquivo Dockerfile contém as instruções para construir a imagem Docker.

O arquivo package.json lista as dependências do projeto e é usado para instalar os pacotes Node.js.

O arquivo index.js é o arquivo principal do servidor. Ele usa o framework Express para criar um servidor web simples.

O arquivo index.html contém o código HTML básico para exibir a página "Eu amo Docker!".

O arquivo main.css contém estilos CSS para a página HTML.

## Obrigado!