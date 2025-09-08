💻 Laboratório Azure: Construindo uma Máquina Virtual do Zero
Este repositório documenta a execução e os aprendizados do desafio de laboratório da DIO, focado na criação e gerenciamento de Máquinas Virtuais (VMs) na Microsoft Azure. O objetivo é aplicar os conceitos teóricos em um cenário prático e estruturar o conhecimento adquirido.

🎯 O Desafio
O propósito deste laboratório é consolidar o conhecimento prático em um dos serviços mais fundamentais da Azure: as Máquinas Virtuais. A proposta é ir além da teoria, executando o passo a passo de provisionamento, configuração e acesso a uma VM na nuvem.

Objetivos de Aprendizagem
Ao final deste projeto, fui capaz de:

Aplicar os conceitos de computação em nuvem em um ambiente real.

Documentar processos técnicos de forma clara, estruturada e compartilhável.

Utilizar o GitHub como uma ferramenta essencial para o portfólio e documentação técnica.

🚀 Resumo da Execução do Laboratório
Para completar o desafio, segui os seguintes passos, que refletem o ciclo de vida básico de um recurso na Azure:

Planejamento e Configuração Inicial:

Acesso ao Portal da Azure.

Criação de um Grupo de Recursos (resource-group-lab-vm) para isolar e gerenciar todos os ativos criados neste laboratório. Isso é crucial para a organização e para facilitar a exclusão dos recursos após a conclusão, evitando custos inesperados.

Provisionamento da Máquina Virtual:

Criação de uma nova Máquina Virtual a partir do Marketplace.

Sistema Operacional: Selecionei a imagem do Windows 10 Pro.

Tamanho da VM: Optei por um tamanho da série B-series (ex: Standard_B1s), que é econômico e ideal para cargas de trabalho de desenvolvimento e teste.

Autenticação: Configurei um usuário e senha de administrador para acesso.

Regras de Rede: Habilitei a porta RDP (3389) para permitir o acesso remoto a partir da minha máquina.

Conexão e Verificação:

Após o deploy da VM, realizei o download do arquivo de conexão RDP.

Utilizei o Cliente de Área de Trabalho Remota do Windows para me conectar à máquina virtual usando as credenciais criadas.

Verifiquei a conectividade com a internet e o funcionamento básico do sistema operacional dentro da VM.

Documentação e Limpeza:

Capturei telas (screenshots) dos principais passos do processo para incluir neste README.

Após a conclusão e documentação, o passo final e mais importante foi excluir o Grupo de Recursos, o que garantiu a remoção de todos os recursos associados (VM, disco, interface de rede, etc.) de forma limpa.

🛠️ Ferramentas e Recursos Utilizados
Microsoft Azure Portal: Para criação e gerenciamento de todos os recursos.

GitHub: Para a documentação e versionamento deste projeto.

Markdown: Para a criação deste arquivo README.md.

Materiais de Apoio
Início Rápido: Criar uma máquina virtual do Windows no Portal do Azure

GitHub Quick Start

Documentação do GitHub

✨ Conclusão
Este desafio foi fundamental para solidificar a compreensão sobre o serviço de IaaS (Infraestrutura como Serviço) da Azure. A experiência de criar, configurar e acessar uma Máquina Virtual na prática torna o aprendizado muito mais tangível e prepara o terreno para explorar cenários mais complexos de arquitetura em nuvem.
