# Gerenciando Políticas em Acessos no Azure

Este guia cobre as principais práticas e ferramentas para gerenciar políticas de acesso e controle em sua infraestrutura Azure.

---

## 1. Portal de Confiança do Serviço

O **Portal de Confiança do Serviço** é uma ferramenta que fornece uma visão centralizada sobre a conformidade e segurança dos serviços Azure.

### Funcionalidades:
- **Visualizar Conformidade**: Verifique a conformidade dos serviços Azure com as regulamentações e padrões de segurança.
- **Gerenciar Certificações**: Acompanhe as certificações de segurança e relatórios de auditoria dos serviços que você utiliza.

[Explore o Portal de Confiança do Serviço](https://azure.microsoft.com/pt-br/trust-center/)

---

## 2. Bloqueios de Grupos de Recursos

Os **bloqueios de grupos de recursos** ajudam a proteger seus recursos contra exclusão acidental ou modificações indesejadas.

### Como usar:
- **Criar Bloqueios**: Aplique bloqueios a grupos de recursos para prevenir alterações ou exclusões acidentais. Você pode definir bloqueios de:
  - **Leitura**: Impede a modificação dos recursos.
  - **Excluir**: Impede a exclusão dos recursos.
- **Movimentação de Recursos**: Os bloqueios são aplicados a todo o grupo de recursos, e os recursos individuais não podem ser movidos para outro grupo sem remover o bloqueio.

[Documentação sobre Bloqueios de Recursos](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/lock-resources)

---

## 3. Microsoft Purview

O **Microsoft Purview** é uma plataforma de governança de dados que ajuda a gerenciar, classificar e proteger seus dados na nuvem.

### Funcionalidades:
- **Classificação de Dados**: Classifique e rotule dados para facilitar a conformidade e a segurança.
- **Gerenciamento de Políticas de Dados**: Defina e aplique políticas para proteger dados sensíveis e garantir a governança.

[Saiba mais sobre Microsoft Purview](https://learn.microsoft.com/pt-br/microsoft-365/compliance/microsoft-purview?view=o365-worldwide)

---

## 4. Policy

**Azure Policy** permite criar, atribuir e gerenciar políticas para garantir que os recursos na sua assinatura Azure estejam em conformidade com os requisitos e padrões organizacionais.

### Principais funcionalidades:
- **Criar Políticas**: Defina regras e efeitos que controlam quais recursos podem ser criados e como devem ser configurados.
- **Atribuir Políticas**: Aplique políticas a grupos de recursos, assinaturas ou management groups para garantir conformidade em grande escala.
- **Monitorar Conformidade**: Use relatórios para monitorar e verificar a conformidade das políticas aplicadas.

[Documentação sobre Azure Policy](https://learn.microsoft.com/pt-br/azure/governance/policy/overview)

---

## Conclusão

Gerenciar políticas e acessos no Azure é crucial para proteger seus recursos e garantir a conformidade com padrões organizacionais. Utilize as ferramentas e práticas descritas neste guia para implementar e monitorar políticas eficazes.

---

**Referências adicionais:**
- [Portal de Confiança do Serviço](https://azure.microsoft.com/pt-br/trust-center/)
- [Bloqueios de Recursos](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/lock-resources)
- [Microsoft Purview](https://learn.microsoft.com/pt-br/microsoft-365/compliance/microsoft-purview?view=o365-worldwide)
- [Azure Policy](https://learn.microsoft.com/pt-br/azure/governance/policy/overview)
