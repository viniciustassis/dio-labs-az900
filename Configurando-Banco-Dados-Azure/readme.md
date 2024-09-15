# Configurando uma instância de Banco de Dados na AzureInstância Gerenciada de SQL do Azure

## Introdução

A **Instância Gerenciada de SQL do Azure** oferece uma solução quase 100% compatível com o SQL Server (Edição Enterprise), com segurança aprimorada através de redes virtuais (VNet) e uma boa integração para clientes existentes do SQL Server. Este guia fornece uma visão geral sobre como configurar rapidamente uma Instância Gerenciada de SQL e migrar seus bancos de dados.

---

## Passos Iniciais

### 1. Configurar o Ambiente

O primeiro passo é criar sua Instância Gerenciada de SQL e configurar o ambiente de rede. Existem várias opções para isso:

- **Criar a Instância Gerenciada de SQL pelo portal do Azure**:  
  Configure parâmetros como **nome de usuário**, **senha**, **número de núcleos** e **armazenamento máximo**. O Azure cuidará automaticamente da rede sem a necessidade de detalhes técnicos sobre infraestrutura.

- **Verificar permissões de assinatura**:  
  Certifique-se de que sua assinatura atual permite a criação de uma Instância Gerenciada de SQL.

- **Usar uma rede personalizada**:  
  Se você já possui uma rede existente, pode configurá-la para a Instância Gerenciada de SQL. Consulte a documentação sobre como [Configurar uma VNet existente](https://learn.microsoft.com/en-us/azure/azure-sql/managed-instance/connect-vnet).

### 2. Acesso à Instância Gerenciada de SQL

A Instância Gerenciada é criada dentro de uma **VNet** e não tem um ponto de extremidade público. Existem duas formas de acessá-la:

- **Habilitar ponto de extremidade público**:  
  Acesse a instância diretamente do ambiente externo.

- **Criar uma VM na mesma VNet**:  
  Conecte-se à Instância Gerenciada de SQL a partir de uma **Máquina Virtual do Azure** na mesma VNet (em uma sub-rede diferente).

- **Configurar uma conexão VPN ponto a site**:  
  Conecte seu computador cliente à VNet da Instância Gerenciada de SQL usando uma VPN ponto a site. Essa configuração permite que você utilize o **SQL Server Management Studio** para acessar o banco de dados.

---

## Automação

Caso prefira automatizar o processo de criação da Instância Gerenciada de SQL, use uma das opções abaixo:

- **PowerShell**  
- **Modelos do Resource Manager com PowerShell**  
- **CLI do Azure**

Essas ferramentas permitem criar scripts para simplificar e agilizar a implementação da sua instância.

---

## Conclusão

A Instância Gerenciada de SQL do Azure oferece flexibilidade e segurança, facilitando a configuração e migração de bancos de dados. Seja criando manualmente pelo portal ou usando automações via PowerShell e CLI, você pode integrar rapidamente essa solução no seu ambiente.

---

**Referências adicionais:**
- [Documentação completa](https://learn.microsoft.com/pt-br/training/modules/create-windows-virtual-machine-in-azure/3-exercise-create-a-vm)
