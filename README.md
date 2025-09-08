# 🏛️ Laboratório de Fundamentos Azure: Organizando a Nuvem

Este repositório documenta a execução de um desafio de projeto da DIO, focado nos pilares da organização e governança na Microsoft Azure: **Assinaturas (Subscriptions)**, **Grupos de Recursos (Resource Groups)** e **Redes Virtuais (VNETs)**. O objetivo é construir uma base sólida para projetos futuros na nuvem.

## 🎯 O Desafio

O propósito deste laboratório é entender e aplicar na prática a estrutura hierárquica que a Azure utiliza para organizar, gerenciar e proteger recursos. Em vez de focar em um serviço específico, o desafio aborda a "espinha dorsal" de qualquer arquitetura na nuvem, garantindo que as soluções sejam escaláveis, seguras e bem gerenciadas desde o início.

### Objetivos de Aprendizagem

Ao final deste projeto, fui capaz de:
* Compreender a hierarquia de gerenciamento da Azure (Assinaturas e Grupos de Recursos).
* Implementar a segmentação de rede básica utilizando VNETs e Sub-redes.
* Documentar a estrutura de um ambiente de nuvem de forma clara para referência futura.

## 🚀 Resumo da Execução do Laboratório

A execução foi dividida em três etapas lógicas, refletindo a forma como os recursos são criados e organizados na plataforma.

### 1. Análise da Estrutura de Gerenciamento

O primeiro passo foi explorar a estrutura existente no **Portal Azure**.
* **Assinatura (Subscription):** Identifiquei a assinatura disponível, compreendendo seu papel como uma unidade de faturamento e um limite de gerenciamento. Todos os recursos criados estão vinculados a ela.
* **Grupos de Recursos (Resource Groups):** Analisei como os grupos de recursos funcionam como contêineres lógicos. Para este laboratório, criei um novo grupo chamado `rg-network-lab-dio` na região `Brazil South`, que serviu para agrupar todos os recursos relacionados à rede. A principal vantagem é que o ciclo de vida de todos os recursos dentro dele pode ser gerenciado de forma unificada.

### 2. Criação da Rede Virtual (VNET)

Com o grupo de recursos criado, o próximo passo foi provisionar a rede.
* **Criação da VNET:** Dentro do `rg-network-lab-dio`, criei uma **Rede Virtual (VNET)** chamada `vnet-main-lab-dio`.
* **Espaço de Endereçamento:** Defini o espaço de endereçamento IP principal para a VNET como `10.1.0.0/16`. Isso significa que todos os recursos dentro desta rede terão um IP privado nesse intervalo.
* **Criação de Sub-redes (Subnets):** Para segmentar a rede, criei duas sub-redes:
    * `snet-frontend` com o intervalo de endereços `10.1.1.0/24`, que poderia ser usada para recursos públicos como servidores web.
    * `snet-backend` com o intervalo de endereços `10.1.2.0/24`, destinada a recursos privados como bancos de dados.

### 3. Validação e Limpeza

* **Validação:** Após a criação, naveguei pelos recursos no portal para visualizar a hierarquia: a Assinatura continha o Grupo de Recursos, que por sua vez continha a VNET e suas respectivas Sub-redes.
* **Limpeza:** Ao final do laboratório, para evitar custos e manter o ambiente organizado, **excluí o Grupo de Recursos `rg-network-lab-dio`**. Essa ação removeu automaticamente todos os recursos contidos nele (a VNET e as Sub-redes), demonstrando a eficiência desse modelo de gerenciamento.

## 🛠️ Ferramentas e Recursos Utilizados

* **Microsoft Azure Portal:** Para criação e gerenciamento de todos os recursos.
* **GitHub:** Para a documentação e versionamento deste projeto.
* **Markdown:** Para a criação deste arquivo `README.md`.

### Materiais de Apoio
* [Documentação sobre Grupos de Recursos do Azure](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/manage-resource-groups-portal)
* [O que é uma Rede Virtual do Azure (VNet)?](https://learn.microsoft.com/pt-br/azure/virtual-network/virtual-networks-overview)

## ✨ Conclusão

Este desafio foi crucial para solidificar a importância do planejamento e da organização na nuvem. Uma estrutura bem definida de Grupos de Recursos e VNETs é a base para garantir segurança, controle de custos e escalabilidade em qualquer projeto na Azure. Dominar esses conceitos fundamentais é o primeiro passo para se tornar um arquiteto de soluções na nuvem eficaz.
