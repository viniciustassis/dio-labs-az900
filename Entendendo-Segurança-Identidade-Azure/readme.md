# Entendendo Segurança e Identidade na Azure

Este guia aborda os principais conceitos de segurança e identidade no Azure, incluindo Microsoft Entra ID, controle de acesso e proteção em nuvem.

---

## 1. Microsoft Entra ID

O **Microsoft Entra ID** (antigo Azure Active Directory - Azure AD) é o serviço de gerenciamento de identidade da Azure, usado para autenticação, controle de acesso e gerenciamento de usuários.

### Usuários
- **Gerenciar Usuários**: Adicione, edite ou remova usuários para controlar o acesso aos recursos da Azure.
- **Usuários Deletados**: Visualize e restaure usuários que foram excluídos recentemente dentro de um período de recuperação.

### Grupos
- **Grupos**: Organize usuários em grupos para aplicar políticas de acesso em escala e simplificar a administração.

### External Identities
- **External Identities**: Permita que usuários externos, como parceiros e fornecedores, acessem recursos usando seus próprios métodos de autenticação.

### Roles and Administrators
- **Funções e Administradores**: Atribua permissões específicas a usuários ou grupos usando **roles** (funções). Cada função tem permissões diferentes para gerenciar recursos da Azure.

---

## 2. Microsoft Entra Connect

O **Microsoft Entra Connect** é uma ferramenta que sincroniza seus diretórios locais (como o Active Directory) com o Microsoft Entra ID. Ele permite:
- Sincronização de identidades entre o ambiente local e a nuvem.
- Autenticação única (SSO) para simplificar o login dos usuários.

---

## 3. Controle de Acesso (IAM)

O **Access Control (IAM)** na Azure permite gerenciar o acesso a recursos por meio da atribuição de funções (roles) a usuários, grupos e identidades de serviço.

### Principais ações:
- **Atribuir permissões**: Controle quem tem acesso a quais recursos e com quais permissões.
- **Princípios de Menor Privilégio**: Sempre atribua a menor permissão necessária para executar uma tarefa, garantindo maior segurança.

---

## 4. Microsoft Defender for Cloud

O **Microsoft Defender for Cloud** é uma solução de gerenciamento de segurança que fornece monitoramento contínuo, avaliação de vulnerabilidades e recomendações de melhoria para os recursos na Azure.

### Principais Funcionalidades:
- **Proteção de Infraestrutura**: Detecta ameaças e vulnerabilidades em suas VMs, bancos de dados e outros recursos.
- **Recomendações de Segurança**: Oferece sugestões automáticas para melhorar a postura de segurança da sua infraestrutura.

---

## Conclusão

Compreender os serviços de segurança e identidade na Azure é essencial para garantir que seus recursos estejam protegidos. Use este guia para gerenciar usuários, implementar controle de acesso adequado e proteger sua infraestrutura com o Microsoft Defender for Cloud.

---

**Referências adicionais:**
- [Documentação oficial do Microsoft Entra ID](https://learn.microsoft.com/pt-br/azure/active-directory/)
- [Documentação do Microsoft Defender for Cloud](https://learn.microsoft.com/pt-br/azure/defender-for-cloud/)
