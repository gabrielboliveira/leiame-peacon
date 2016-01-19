# Documentação Projeto Peacon

Essa é toda a documentação do Trabalho de Conclusão de Curso denominado "Desenvolvimento de um Protótipo de Rastreador de Beacons utilizando o Raspberry Pi".

## Estrutura de Pastas

A documentação está separada em pastas, sendo quatro partes.

### Apresentações

Todas as apresentações utilizadas, sendo parciais (PIS 1), seminário, final e banca (PIS 2). As subpastas estão ordenadas por data de apresentação. Os arquivos incluídos são:

- **PPTX**: arquivo de rascunho utilizado para gerar as apresentações;
- **PDF**: arquivo final gerado para facilitar consulta. 

### Código Fonte

Todo o código fonte utilizado no desenvolvimento e projeto do protótipo [Peacon](https://github.com/gabrielboliveira/peacon/). Para executar o código, é necessário ter instalado o [Git](https://git-scm.com/), [Node.js](https://nodejs.org/) e [CouchDB](http://couchdb.org/). Para instalar as dependências no Raspberry Pi, siga os comandos abaixo:

```bash
# Atualizar todos os pacotes
sudo apt-get update && sudo apt-get upgrade

# Instalar o Git
sudo apt-get install git

# Adicionar link de dependência para o nodejs
curl -sLS https://apt.adafruit.com/add | sudo bash

# Instalar o node.js
sudo apt-get install node

# Instalar o CouchDB
sudo apt-get install couchdb
```

Copie o diretório para onde desejar, como por exemplo:

```bash
# copia o código fonte para a pasta 'peacon' 
cp "Código Fonte" peacon
```

Se preferir, em vez de copiar o código fonte, é possível baixar o código direto do repositório do [Github](https://github.com/gabrielboliveira/peacon/):

```bash
# baixa os arquivos fonte para a pasta 'peacon'
git clone https://github.com/gabrielboliveira/peacon.git peacon
``` 

Agora, acesse a pasta com o código fonte:

``` bash
# acessar o código fonte
cd peacon
```

Após, é necessário executar a instalação das dependências de pacote do projeto:

```bash
# instala todas as dependências de uma só vez
npm install
``` 

Em seguida, para rodar o programa, é só executar o comando:

```bash
# executa o código
node index.js
``` 

### Monografia

A monografia entregue para a banca está na pasta Monografia. O arquivo `Monografia TCC - Gabriel Oliveira.pdf` é a versão final entregue no dia 12/01/2016 e impressa para os membros da banca. 

Na pasta `Fonte` estão todos os arquivos utilizados para gerar o PDF. Para compilar o código em LaTeX é necessário ter um compilador instalado, assim como o pacote [abnTeX2](https://github.com/abntex/abntex2/) ([Guia de Instalação](https://github.com/abntex/abntex2/wiki/Instalacao)). 

Após ter instalado todas as dependências, para compilar o código é só executar os comandos abaixo:

```bash
# Faz a primeira compilação dos arquivos auxiliares
xelatex monografia.tex

# Gera todas as referências bibliográficas
bibtex monografia.aux

# Faz a segunda compilação gerando as referências internas
xelatex monografia.tex

# Faz a última compilação, com todas as referências corretas
xelatex monografia.tex
```

Os arquivos da monografia também estão no [Github](https://github.com/gabrielboliveira/Monografia-Peacon), e assim como o código fonte, também pode ser clonado com o comando abaixo:

```bash
# baixa os arquivos fonte da monografia para a pasta 'monografia-peacon'
git clone https://github.com/gabrielboliveira/Monografia-Peacon.git monografia-peacon
``` 

### Proposta e Relatório

Nessa pasta estão a Proposta e o Relatório Parcial, entregues na disciplina Projeto e Implementação de Sistemas 1. Assim como a monografia, esses relatórios também foram desenvolvidos com o LaTex e podem ser acessados no Github:

- **v0.1**: [Proposta](https://github.com/gabrielboliveira/Monografia-Peacon/tree/4c547ca085d6b837a7e838cc99305f4a8f63b0fe);
- **v0.2**: [Relatório Parcial](https://github.com/gabrielboliveira/Monografia-Peacon/tree/0cda1dd8af6ba90cd1b0f801b1d555970d812733).

## Leia-me

Esse arquivo de Leia-me foi desenvolvido com a ferramenta Markdown, muito utilizada nos repositórios do Github.