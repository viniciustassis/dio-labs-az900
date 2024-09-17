# Dominando o Armazenamento no Azure

Este guia cobre os principais aspectos do armazenamento no Azure, incluindo a configuração de contas de armazenamento, opções avançadas, e gerenciamento de dados.

---

## 1. Contas de Armazenamento

Uma **conta de armazenamento** no Azure fornece uma forma de acessar e gerenciar seus dados na nuvem.

### Configurações principais:
- **Nome da Conta de Armazenamento**: Escolha um nome único para sua conta de armazenamento. O nome deve ser globalmente único e seguir os requisitos de nomenclatura do Azure.
  
- **Redundância**: Selecione o tipo de redundância para garantir a durabilidade dos dados:
  - **LRS (Locally Redundant Storage)**: Dados são replicados dentro de um único datacenter.
  - **GRS (Geo-Redundant Storage)**: Dados são replicados para uma segunda região geográfica.
  - **ZRS (Zone-Redundant Storage)**: Dados são replicados entre zonas dentro da mesma região.

---

## 2. Avançado

### Camada de Acesso
- **Camada de Acesso**: Escolha a camada que melhor se adapta ao uso dos seus dados:
  - **Hot**: Para dados acessados frequentemente.
  - **Cool**: Para dados acessados esporadicamente.
  - **Archive**: Para dados raramente acessados e com requisitos de retenção de longo prazo.

---

## 3. Rede

Configure o acesso à conta de armazenamento através da rede.

### Opções:
- **Firewall e Redes Virtuais**: Configure regras de firewall e conecte sua conta a redes virtuais para controlar o acesso.
- **Endpoints Privados**: Use endpoints privados para acessar sua conta de armazenamento de forma segura e privada dentro da sua rede.

---

## 4. Proteção de Dados

Garanta a proteção e recuperação dos seus dados.

### Opções:
- **Backup**: Configure backups regulares para proteger seus dados contra perdas.
- **Azure Backup**: Use o serviço Azure Backup para criar e gerenciar backups automatizados.

---

## 5. Contêineres

Os **contêineres** são usados para organizar e gerenciar blobs dentro da conta de armazenamento.

### Como criar:
- No **Portal do Azure**, acesse sua conta de armazenamento e selecione **Blobs**.
- Clique em **Contêiner** e forneça um nome para criar um novo contêiner.

---

## 6. Compartilhamento de Arquivos

O **Azure Files** permite que você compartilhe arquivos na nuvem.

### Como criar:
- No **Portal do Azure**, vá para **Compartilhamentos de Arquivos** na sua conta de armazenamento.
- Clique em **Adicionar Compartilhamento** e defina o nome e o tamanho do compartilhamento.

---

## 7. Fila

O **Azure Queue Storage** permite o armazenamento e gerenciamento de mensagens em filas.

### URL:
- **URL da Fila**: `https://<accountname>.queue.core.windows.net/<queuename>`
  - Substitua `<accountname>` pelo nome da sua conta de armazenamento e `<queuename>` pelo nome da fila.

---

## 8. Tabelas

O **Azure Table Storage** oferece armazenamento NoSQL para grandes volumes de dados estruturados.

### URL:
- **URL da Tabela**: `https://<accountname>.table.core.windows.net/<tablename>`
  - Substitua `<accountname>` pelo nome da sua conta de armazenamento e `<tablename>` pelo nome da tabela.

---

## Conclusão

Compreender e configurar adequadamente as opções de armazenamento no Azure é essencial para gerenciar e proteger seus dados de forma eficiente. Utilize este guia para configurar suas contas de armazenamento, escolher camadas de acesso, e gerenciar contêineres, arquivos, filas e tabelas.

---

**Referências adicionais:**
- [Documentação oficial do Azure Storage](https://learn.microsoft.com/pt-br/azure/storage/)
