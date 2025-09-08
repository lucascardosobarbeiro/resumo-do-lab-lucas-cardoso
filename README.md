🗃️ Laboratório Azure: Configurando um Banco de Dados SQL na Nuvem
Este repositório documenta a execução e os aprendizados do desafio de laboratório da DIO, focado na criação e gerenciamento de uma instância de Banco de Dados SQL na Microsoft Azure. O objetivo é aplicar os conceitos teóricos de PaaS (Plataforma como Serviço) em um cenário prático.

🎯 O Desafio
O propósito deste laboratório é praticar o processo de configuração de uma instância de Banco de Dados na plataforma Microsoft Azure. A proposta é criar um material de apoio com resumos, anotações e dicas sobre o uso de bancos de dados gerenciados na Azure, servindo como guia para estudos e futuras implementações.

Objetivos de Aprendizagem
Ao final deste projeto, fui capaz de:

Aplicar os conceitos de banco de dados como serviço em um ambiente prático.

Documentar processos técnicos de forma clara, estruturada e compartilhável.

Utilizar o GitHub como uma ferramenta essencial para o portfólio e documentação técnica.

🚀 Resumo da Execução do Laboratório
Para completar o desafio, segui os seguintes passos, que refletem o ciclo de vida básico de um recurso de banco de dados na Azure:

Planejamento e Configuração Inicial:

Acesso ao Portal da Azure.

Criação de um Grupo de Recursos (resource-group-lab-sql) para isolar e gerenciar todos os ativos criados. Isso é crucial para a organização e para facilitar a limpeza dos recursos após a conclusão.

Provisionamento do Banco de Dados SQL:

Criação de um novo recurso Banco de Dados SQL do Azure.

Configuração do Servidor: Criei um novo servidor lógico para hospedar o banco de dados, definindo um nome, login e senha de administrador.

Modelo de Computação: Optei pelo modelo Serverless, que é ideal para cargas de trabalho com uso intermitente e imprevisível, além de ser econômico para ambientes de desenvolvimento.

Rede: Configurei as regras de firewall do servidor para permitir o acesso do meu endereço IP de cliente, garantindo que eu pudesse me conectar ao banco de dados a partir da minha máquina.

Conexão e Verificação:

No painel do banco de dados no portal, obtive as cadeias de conexão (connection strings).

Utilizei o Azure Data Studio para me conectar ao banco de dados recém-criado, usando as credenciais do servidor.

Executei uma consulta simples (ex: SELECT @@VERSION) para confirmar que a conexão foi bem-sucedida e o banco de dados estava operacional.

Documentação e Limpeza:

Capturei telas (screenshots) dos principais passos do processo para incluir neste README.

Após a conclusão e documentação, o passo final foi excluir o Grupo de Recursos, o que garantiu a remoção de todos os recursos associados (servidor SQL, banco de dados, etc.).

🛠️ Ferramentas e Recursos Utilizados
Microsoft Azure Portal: Para criação e gerenciamento de todos os recursos.

Azure Data Studio: Ferramenta para conectar e gerenciar o banco de dados.

GitHub: Para a documentação e versionamento deste projeto.

Markdown: Para a criação deste arquivo README.md.

Materiais de Apoio
Início Rápido: criar Instância Gerenciada de SQL do Azure

GitHub Quick Start

Documentação do GitHub

✨ Conclusão
Este desafio prático foi essencial para entender as vantagens de utilizar um serviço de banco de dados gerenciado (PaaS) na Azure. A facilidade de provisionamento, configuração de segurança e escalabilidade, sem a necessidade de gerenciar a infraestrutura subjacente, demonstra o poder da nuvem para acelerar o desenvolvimento de aplicações modernas.
