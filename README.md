☁️ Desbravando a Nuvem: Um Guia Introdutório à Microsoft Azure
Este repositório contém um resumo dos conceitos e lições aprendidas durante o laboratório da DIO sobre a Microsoft Azure. O objetivo é documentar os principais serviços e a estrutura fundamental da plataforma de nuvem da Microsoft.

🎯 O que é a Microsoft Azure?
A Microsoft Azure é uma plataforma de computação em nuvem que oferece mais de 200 produtos e serviços projetados para ajudar você a criar, executar e gerenciar aplicações em múltiplos ambientes — na nuvem, localmente (on-premises) ou na borda (edge). Ela permite que empresas e desenvolvedores acessem recursos computacionais, como servidores, armazenamento, bancos de dados e redes, pela internet, pagando apenas pelo que usam.

🛠️ Conceitos e Serviços Fundamentais
A Azure organiza seus serviços em categorias. Abaixo estão os conceitos essenciais para quem está começando.

📂 Estrutura e Gerenciamento
Grupos de Recursos (Resource Groups): São "pastas" lógicas para agrupar e gerenciar todos os seus recursos (máquinas virtuais, bancos de dados, etc.) de uma solução. Facilitam a organização, o controle de custos e a gestão de permissões. Tudo na Azure deve pertencer a um grupo de recursos.

Azure Portal: A interface web principal para criar, gerenciar e monitorar todos os seus recursos. É o seu centro de comando na nuvem.

Regiões e Zonas de Disponibilidade: A Azure possui data centers em todo o mundo, organizados em Regiões (ex: Brazil South). Cada região pode ter múltiplas Zonas de Disponibilidade, que são locais físicos isolados, garantindo alta disponibilidade e tolerância a falhas.

💻 Computação (Compute)
Esses serviços fornecem a infraestrutura para executar suas aplicações.

Máquinas Virtuais (VMs): Servidores virtuais (Windows ou Linux) que oferecem controle total sobre o sistema operacional e o ambiente. Ideal para migrar aplicações existentes para a nuvem (IaaS - Infraestrutura como Serviço).

Serviço de Aplicativo (App Service): Uma plataforma gerenciada para hospedar aplicações web e APIs sem se preocupar com a infraestrutura subjacente (PaaS - Plataforma como Serviço). Suporta diversas linguagens como .NET, Java, Node.js, Python e PHP.

Azure Functions: Uma solução "serverless" (sem servidor) que permite executar pequenos trechos de código (funções) em resposta a eventos, sem precisar provisionar ou gerenciar servidores. Ideal para automação e tarefas orientadas a eventos.

💾 Armazenamento (Storage)
Soluções para armazenar dados de forma segura, escalável e acessível.

Armazenamento de Blobs (Blob Storage): Otimizado para armazenar grandes volumes de dados não estruturados, como imagens, vídeos, backups e logs.

Arquivos do Azure (Azure Files): Oferece compartilhamentos de arquivos na nuvem totalmente gerenciados, acessíveis via protocolos SMB e NFS.

Armazenamento em Disco (Disk Storage): Discos SSD ou HDD de alto desempenho para serem anexados a Máquinas Virtuais.

🗃️ Bancos de Dados (Databases)
Serviços de banco de dados gerenciados, escaláveis e seguros.

Banco de Dados SQL do Azure (Azure SQL Database): Uma versão gerenciada do Microsoft SQL Server, oferecendo alta performance e compatibilidade (PaaS).

Azure Cosmos DB: Um banco de dados NoSQL multimodelo, distribuído globalmente, com latência de milissegundos e alta disponibilidade.

🌐 Rede (Networking)
Rede Virtual do Azure (VNet): Permite criar redes privadas e isoladas na nuvem, onde você pode conectar seus recursos de forma segura.

Balanceador de Carga (Load Balancer): Distribui o tráfego de rede entre múltiplas máquinas virtuais para garantir alta disponibilidade e performance.

🚀 Como Começar: Passo a Passo Simples
Criar uma Conta Gratuita: Acesse o site da Azure e crie uma conta para obter créditos gratuitos e acesso a serviços populares.

Explorar o Azure Portal: Familiarize-se com a interface, navegando pelos menus e dashboards.

Criar seu Primeiro Recurso: Use o portal para provisionar um recurso simples, como um Serviço de Aplicativo para hospedar um site estático ou uma Máquina Virtual com Linux.

Organize com Grupos de Recursos: Sempre crie um novo Grupo de Recursos para cada projeto ou lab, facilitando a limpeza posterior.

✨ Conclusão
Este laboratório proporcionou uma visão prática e fundamental do poder da Microsoft Azure. Compreender conceitos como Grupos de Recursos, Serviços de Aplicativo e Máquinas Virtuais é o primeiro passo para construir soluções robustas e escaláveis na nuvem. A jornada na computação em nuvem é contínua e cheia de possibilidades!
