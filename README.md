# trabalhorasi
1. Contexto e Problema
Dificuldade clássica: A divergência de ambientes entre desenvolvimento e produção ("na minha máquina funciona").   
PDF

Solução: O Docker empacota a aplicação com todas as suas dependências, garantindo consistência, portabilidade e rápida execução em qualquer máquina.   
PDF
+ 1

2. Conceitos Teóricos Fundamentais
Container: Pacote leve e executável com código, dependências, bibliotecas, variáveis de ambiente e arquivos de configuração.   
PDF

Container vs. Máquina Virtual (VM):

Containers: Compartilham o kernel do host, virtualizam o sistema operacional, iniciam em segundos e utilizam menos recursos.   
PDF

VMs: Emulam hardware completo, possuem sistema operacional próprio, iniciam em minutos e consomem mais recursos.   
PDF

Arquitetura do Docker:

Client: Interface/comando docker.   
PDF

Daemon: Processo em background que gerencia os containers.   
PDF

Registry (Docker Hub): Repositório público/privado de imagens.   
PDF

Elementos Chave:

Imagem: Template imutável com a aplicação e dependências.   
PDF

Dockerfile: Arquivo de instruções para compilar/construir uma imagem.   
PDF

Sistema de Camadas (Copy-on-Write): Camadas read-only compartilhadas com uma camada read-write superior no container.   
PDF

3. Comandos e Exemplos Práticos
Comandos Iniciais:

docker --version (verificar versão)   
PDF

docker run hello-world (testar execução)   
PDF

docker pull ubuntu:20.04 (baixar imagem)   
PDF

docker run -it ubuntu:20.04 bash (executar modo interativo)   
PDF

docker ps / docker ps -a (listar containers ativos / todos)   
PDF

docker images (listar imagens locais)   
PDF

Servidor Web: Exemplo de execução em segundo plano com mapeamento de portas (docker run -d -p 8080:80 httpd) e verificação de logs/parada (docker logs, docker stop).   
PDF

Dockerfile Simples: Instruções básicas (FROM, WORKDIR, RUN, COPY, EXPOSE, CMD) aplicadas em um exemplo com Python e Flask.   
PDF

4. Boas Práticas
Um processo por container (responsabilidade única).   
PDF

Utilizar imagens oficiais e mantê-las leve (ex: imagens Alpine).   
PDF

Utilizar volumes para dados persistentes (não salvar dados voláteis dentro do container) e variáveis de ambiente para configurações.   
PDF

5. Guia Prático do Trabalho em Grupo
Configuração da VM / Ambiente:

Instalar o Docker no Lubuntu/Ubuntu Server conforme a documentação oficial.   
PDF

Ajuste de repositórios: se usar a VM pronta no disco D:, remover os arquivos docker.list e docker.sources e atualizar os repositórios.   
PDF

Configuração de Rede na VM: usar NAT caso ocorra erro de conexão/download; alterar para Bridge para acessar a aplicação pelo navegador fora da VM.   
PDF

Atividades no GitHub:

Cada integrante deve criar um repositório individual intitulado “Introdução ao Docker” com um arquivo README.md sobre a primeira etapa (Docker, Python e Flask).   
PDF

O relatório principal do grupo deve incluir os links de todos os repositórios individuais logo na Seção 1 (1. Introdução -> 1.1 Repositórios de Introdução ao Docker dos Integrantes).   
PDF

Elaboração da Documentação:

O grupo pode utilizar o modelo no Google Docs ou LaTeX (Overleaf) disponibilizado.   
PDF

Seções não necessárias (como Revisão Bibliográfica) podem ser removidas.   
PDF
