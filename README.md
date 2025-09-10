🚀 Laboratório Azure: Automatizando a Implantação de Infraestrutura
Este repositório documenta um desafio de projeto da DIO, focado em explorar as diferentes Ferramentas de Implantação e Automação na Microsoft Azure. O objetivo é compreender o conceito de Infraestrutura como Código (IaC) e aprender a utilizar as ferramentas que permitem provisionar e gerenciar recursos de forma programática, consistente e escalável.

🎯 O Desafio
O propósito deste laboratório é evoluir da criação manual de recursos via Portal Azure para uma abordagem automatizada e profissional. O desafio consiste em pesquisar e documentar os principais métodos de implantação, desde scripts de linha de comando até templates declarativos, entendendo os benefícios de tratar a infraestrutura da mesma forma que tratamos o código de uma aplicação: com versionamento, revisão e automação. projeto, fui capaz de:

Aplicar o Controle de Acesso Baseado em Função (RBAC) para gerenciar permissões.

Entender como o Azure Policy impõe regras e padrões aos recursos.

Compreender o papel dos Blueprints e Management Groups para governança em larga escala.

🏛️ Pilares da Governança e Acesso na Azure
A Azure fornece um conjunto de serviços projetados para trabalhar juntos, criando um framework de governança robusto.

1. Controle de Acesso Baseado em Função (RBAC - Role-Based Access Control)
O RBAC é o pilar fundamental para gerenciar quem pode fazer o quê. Em vez de dar permissões diretamente aos usuários, você atribui "funções" (roles) a eles em um determinado "escopo" (recurso, grupo de recursos, assinatura).

Princípio do Menor Privilégio: A ideia central é conceder apenas o acesso necessário para que um usuário realize seu trabalho, e nada mais.

Funções Principais:

Proprietário (Owner): Controle total, incluindo a capacidade de delegar acesso a outros.

Contribuidor (Contributor): Pode criar e gerenciar todos os tipos de recursos, mas não pode conceder acesso a outros.

Leitor (Reader): Pode visualizar os recursos existentes, mas não pode fazer alterações.

2. Azure Policy
Enquanto o RBAC foca nos usuários, o Azure Policy foca nos recursos. Ele permite criar, atribuir e gerenciar "políticas" que impõem regras e efeitos sobre os seus recursos para que eles permaneçam em conformidade com os padrões corporativos.

Exemplos de Políticas:

"Permitir apenas a criação de VMs de tamanhos específicos" (para controlar custos).

"Exigir que todos os grupos de recursos tenham uma tag de 'centro de custo'" (para organização).

"Auditar se as contas de armazenamento possuem tráfego seguro (HTTPS) habilitado".

3. Azure Blueprints
O Azure Blueprints permite que arquitetos de nuvem criem um "pacote" ou um "projeto" de um ambiente padrão e repetível. Esse pacote pode incluir:

Atribuições de RBAC.

Atribuições de Políticas.

Modelos ARM (templates para implantar recursos).

Ao usar um blueprint, você garante que novos ambientes (como assinaturas de desenvolvimento ou produção) sejam criados já em conformidade com as regras da organização.

4. Grupos de Gerenciamento (Management Groups)
Quando você tem muitas assinaturas, gerenciá-las individualmente se torna inviável. Os Grupos de Gerenciamento são "contêineres" para suas assinaturas. Eles criam uma hierarquia que permite aplicar políticas e controles de acesso (RBAC) a um grupo inteiro de assinaturas de uma só vez, garantindo a aplicação consistente da governança em toda a organização.

✨ Conclusão
Este estudo demonstrou que RBAC, Azure Policy, Blueprints e Management Groups são ferramentas complementares e essenciais para a governança na nuvem. Juntos, eles formam um sistema poderoso que permite às organizações escalar suas operações na Azure de forma segura, controlada e em conformidade com as regras de negócio.
