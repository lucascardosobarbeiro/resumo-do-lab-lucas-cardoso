🛡️ Laboratório Azure: Protegendo a Nuvem com Segurança e Identidade
Este repositório documenta um desafio de projeto da DIO, focado em explorar os pilares de Segurança e Identidade na Microsoft Azure. O objetivo é entender como utilizar as ferramentas da nuvem para proteger dados, aplicações e a infraestrutura contra ameaças, aplicando o princípio da defesa em profundidade.

🎯 O Desafio
O propósito deste laboratório é ir além dos serviços de computação e armazenamento, mergulhando nas camadas que garantem a integridade e a confidencialidade de um ambiente na nuvem. O desafio consiste em pesquisar e documentar os principais recursos de segurança da Azure, desde o controle de quem pode acessar os recursos até a proteção proativa contra ameaças cibernéticas.

Objetivos de Aprendizagem
Ao final deste projeto, fui capaz de:

Entender o papel do Microsoft Entra ID no gerenciamento de identidades e acessos.

Diferenciar as ferramentas de segurança de rede, como NSGs e Azure Firewall.

Identificar os serviços para proteção contra ameaças e gerenciamento da postura de segurança.

Compreender a importância de proteger segredos e chaves com o Azure Key Vault.

🔐 Pilares da Segurança e Identidade na Azure
A segurança na Azure é construída em camadas (defesa em profundidade). Abaixo estão os principais serviços e conceitos estudados.

1. Microsoft Entra ID (anteriormente Azure AD): O Coração da Identidade
É o serviço de gerenciamento de identidade e acesso multinuvem da Microsoft. Ele é a porta de entrada para todos os serviços da Azure e do Microsoft 365.

Gerenciamento de Identidade: Criação e gestão de usuários, grupos e permissões.

Autenticação Multifator (MFA): Adiciona uma camada crucial de segurança, exigindo uma segunda forma de verificação (como um código no celular) para comprovar a identidade do usuário.

Acesso Condicional (Conditional Access): Permite criar regras granulares para o acesso. Por exemplo: "Exigir MFA para todos os administradores que acessam o portal de um local não confiável".

Controle de Acesso Baseado em Função (RBAC): Garante o princípio do menor privilégio. Em vez de dar permissão total, você atribui funções específicas (como Leitor, Contribuidor, Proprietário) a usuários ou grupos para recursos específicos.

2. Segurança de Rede: A Primeira Linha de Defesa
Controlar o tráfego de rede é fundamental para impedir acessos não autorizados.

Grupos de Segurança de Rede (NSGs): Funcionam como um firewall básico no nível da sub-rede ou da placa de rede de uma VM. Permitem criar regras de entrada e saída para liberar ou bloquear tráfego com base em IP, porta e protocolo.

Azure Firewall: Um serviço de firewall de rede inteligente e totalmente gerenciado. Oferece proteção centralizada para todos os recursos em uma rede virtual, com recursos avançados como filtragem baseada em inteligência contra ameaças.

Proteção contra DDoS do Azure: Protege os recursos da Azure contra ataques de negação de serviço distribuído (DDoS), garantindo a disponibilidade das aplicações.

3. Proteção Contra Ameaças e Gerenciamento de Postura
Microsoft Defender for Cloud: É o hub centralizado para o gerenciamento da postura de segurança na nuvem (CSPM) e proteção de cargas de trabalho (CWPP). Ele fornece:

Pontuação de Segurança: Uma nota que indica o quão segura está sua infraestrutura.

Recomendações: Sugestões práticas para corrigir vulnerabilidades (ex: "Habilite o MFA em contas de proprietário").

Alertas de Segurança: Detecta e alerta sobre atividades suspeitas em tempo real.

4. Proteção da Informação: Guardando os Segredos
Azure Key Vault: Um cofre seguro na nuvem para armazenar e gerenciar segredos de aplicação, como chaves de API, senhas e certificados. Isso evita a prática perigosa de armazen
