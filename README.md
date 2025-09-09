⚙️ Laboratório Azure: Explorando o Poder Computacional
Este repositório documenta a execução de um desafio de projeto da DIO, focado em entender e provisionar diferentes tipos de instâncias de computação na Microsoft Azure. O objetivo é aprender a escolher o serviço certo para a necessidade certa, desde Máquinas Virtuais personalizadas para tarefas específicas (como workstations) até a agilidade do serverless com Azure Functions.

🎯 O Desafio
O propósito deste laboratório é ir além da criação de uma VM genérica e explorar como a Azure oferece um leque de opções computacionais para diferentes cenários. O desafio consiste em provisionar uma VM customizada para um fim específico e contrastar essa abordagem com modelos mais gerenciados, como as Functions.

Objetivos de Aprendizagem
Ao final deste projeto, fui capaz de:

Diferenciar os principais modelos de serviço de computação: IaaS, PaaS e Serverless.

Criar uma Máquina Virtual personalizada a partir de imagens do Azure Marketplace para atender a uma necessidade específica.

Compreender o caso de uso ideal para Azure Functions em comparação com uma VM tradicional.

🚀 Resumo da Execução do Laboratório
A execução foi dividida em duas frentes principais: a criação de uma workstation de desenvolvimento completa (IaaS) e a exploração de uma função serverless (FaaS).

1. Provisionando uma Workstation de Desenvolvimento (VM Personalizada)
O objetivo aqui era simular a criação de uma máquina de alta performance para um desenvolvedor, com todo o ambiente já configurado.

Planejamento e Grupo de Recursos: Criei um novo grupo de recursos chamado rg-dev-workstation-lab para isolar o ambiente.

Escolha da Imagem (O Ponto Chave): Em vez de uma imagem de SO base, utilizei o Azure Marketplace para encontrar uma imagem pré-configurada de "Windows 10 + Visual Studio 2022". Isso economiza horas de instalação e configuração manual.

Seleção do Tamanho (Performance): Escolhi uma instância da série Dsv3 (ex: Standard_D2s_v3), que é otimizada para aplicações de uso geral e oferece um bom equilíbrio entre CPU e memória para compilação de código e desenvolvimento.

Configuração e Acesso: Configurei as regras de rede para permitir acesso via RDP (porta 3389) e, após o provisionamento, conectei-me à máquina para validar que o Visual Studio e todas as ferramentas de desenvolvimento estavam prontas para uso.

2. Explorando a Abordagem Serverless (Azure Functions)
Para contrastar com a complexidade e o controle total da VM, criei uma pequena função para executar uma tarefa simples.

Criação do Function App: Dentro do mesmo grupo de recursos, criei um Aplicativo de Funções. O provisionamento foi muito mais rápido, pois não há um sistema operacional completo para gerenciar.

Desenvolvimento da Função: Criei uma função simples com um gatilho HTTP. O objetivo era receber um nome como parâmetro na URL e retornar uma saudação "Olá, [nome]".

Teste e Validação: Utilizei a própria interface do portal para testar a função, passando um parâmetro na URL de teste e verificando a resposta. A simplicidade e o foco exclusivo no código foram evidentes.

🛠️ Ferramentas e Recursos Utilizados
Microsoft Azure Portal: Para provisionamento e gerenciamento de todos os recursos.

Azure Marketplace: Para encontrar imagens de VM especializadas.

Cliente de Área de Trabalho Remota: Para conectar à workstation virtual.

GitHub: Para a documentação e versionamento deste projeto.

Materiais de Apoio
Série de tamanhos de VM para fins gerais

Introdução ao Azure Functions

✨ Conclusão
Este laboratório foi essencial para entender que não existe uma "solução única" para computação na nuvem.

Máquinas Virtuais (IaaS) brilham quando você precisa de controle total, ambientes persistentes e softwares específicos, sendo a escolha ideal para workstations, servidores de legado ou aplicações com requisitos complexos de sistema operacional.

Azure Functions (Serverless/FaaS) é a ferramenta perfeita para tarefas orientadas a eventos, processamento de dados em pequena escala e microsserviços, onde o foco é a lógica do negócio, e não a infraestrutura
