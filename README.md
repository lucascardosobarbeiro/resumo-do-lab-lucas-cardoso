☁️ Laboratório Azure: Migrando e Armazenando Dados na Nuvem
Este repositório documenta um desafio de projeto da DIO, focado em explorar as estratégias e ferramentas para migração de dados e os diferentes tipos de armazenamento disponíveis na Microsoft Azure. O objetivo é entender como mover cargas de trabalho para a nuvem de forma eficiente e escolher a solução de armazenamento correta para cada tipo de dado.

🎯 O Desafio
O propósito deste laboratório é desmistificar o processo de transição para a nuvem. O desafio consiste em pesquisar e documentar os principais serviços que a Azure oferece para migrar aplicações e bancos de dados, além de entender as características dos principais serviços de armazenamento, que são fundamentais para qualquer arquitetura na nuvem.

Objetivos de Aprendizagem
Ao final deste projeto, fui capaz de:

Diferenciar os principais tipos de armazenamento da Azure e suas camadas de acesso.

Identificar as ferramentas certas para diferentes cenários de migração (online, offline, linha de comando).

Compreender as fases de uma jornada de migração para a nuvem.

🗄️ Tipos de Armazenamento na Azure
A escolha do armazenamento é um dos pilares de uma arquitetura de nuvem bem-sucedida. Cada serviço é otimizado para um cenário de uso diferente.

1. Azure Blob Storage (Armazenamento de Objetos)
Ideal para dados não estruturados em grande escala. Pense nele como um repositório massivo para arquivos como imagens, vídeos, documentos, logs e backups.

Camadas de Armazenamento do Blob (Storage Tiers)
Para otimizar custos, o Blob Storage oferece diferentes camadas de acesso baseadas na frequência com que os dados são utilizados:

Hot (Quente) 🔥: Otimizada para dados acessados com frequência. Possui o maior custo de armazenamento, mas o menor custo de acesso.

Cool (Fria) ❄️: Para dados acessados com pouca frequência e armazenados por no mínimo 30 dias (ex: backups recentes, telemetria). O custo de armazenamento é menor, mas o de acesso é maior que a camada Hot.

Archive (Arquivo Morto) 📦: A camada de menor custo, projetada para dados raramente acessados e armazenados por no mínimo 180 dias (ex: arquivamento de longo prazo, dados para conformidade legal). Acessar os dados pode levar várias horas (processo de reidratação).

2. Azure Files
Oferece compartilhamentos de arquivos totalmente gerenciados na nuvem, acessíveis via protocolo SMB. É a solução perfeita para substituir servidores de arquivos on-premises (File Servers) sem precisar de uma VM, criando um drive de rede na nuvem.

3. Azure Disk Storage
Fornece discos de bloco de alto desempenho para Máquinas Virtuais (VMs). Funciona como um HD ou SSD virtual que você anexa a uma VM para instalar o sistema operacional e aplicações.

🚚 Ferramentas e Serviços de Migração
A Azure oferece um conjunto robusto de ferramentas para facilitar a migração de ambientes on-premises para a nuvem.

1. AzCopy
É uma ferramenta de linha de comando (CLI) de última geração para copiar dados de e para o Armazenamento do Azure. É otimizada para alta performance e pode ser usada em scripts para automatizar tarefas de transferência de dados, sendo ideal para uploads e downloads em massa de forma programática.

2. Azure Data Box
Para cenários de migração offline de grandes volumes de dados (terabytes ou petabytes), o Azure Data Box é a solução. O processo é simples:

Você encomenda um dispositivo físico e robusto no portal da Azure.

A Microsoft envia o dispositivo para o seu datacenter.

Você conecta o Data Box à sua rede local e copia os dados para ele.

Você envia o dispositivo de volta para a Microsoft.

A equipe da Azure faz o upload dos seus dados diretamente para a sua conta de armazenamento.

Essa abordagem é ideal quando a sua conexão de internet não é rápida o suficiente para transferir grandes quantidades de dados em um tempo razoável.

3. Azure Migrate
É o hub centralizado para descobrir, avaliar e migrar servidores, aplicações e bancos de dados do seu ambiente local para a Azure. Ele ajuda a planejar a migração, estimando custos e identificando possíveis problemas de compatibilidade antes de mover qualquer coisa.

✨ Conclusão
Este estudo foi fundamental para entender que a migração para a nuvem é um processo bem estruturado e suportado por um ecossistema completo de ferramentas na Azure. A chave para o sucesso está no planejamento cuidadoso, na avaliação correta do ambiente existente e na escolha inteligente dos serviços de armazenamento e das ferramentas de migração — seja via rede com AzCopy ou
