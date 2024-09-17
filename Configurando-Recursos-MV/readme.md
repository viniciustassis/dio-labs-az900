# Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure

Este guia cobre os principais passos para criar e gerenciar máquinas virtuais (VMs) no Azure, incluindo a configuração de grupos de recursos, opções de disponibilidade, e aspectos relacionados à rede e gerenciamento.

---

## 1. Criar ou Escolher um Grupo de Recursos

Um **grupo de recursos** é um contêiner lógico que agrupa recursos relacionados no Azure.

### Como criar:
- No **Azure Portal**, vá para **Grupos de Recursos**.
- Clique em **Criar** e preencha detalhes como **Nome** e **Região**.
- Finalize clicando em **Revisar e Criar**.

### Como escolher:
- Se já tiver um grupo de recursos, selecione-o ao criar ou configurar uma nova VM.

---

## 2. Criar Máquina Virtual do Azure

Para criar uma VM, siga os passos abaixo:

### Passos básicos:
- No **Portal do Azure**, navegue até **Máquinas Virtuais** e clique em **Criar**.
- Complete os campos obrigatórios:
  - **Nome da VM**
  - **Região** (deve ser a mesma do grupo de recursos)
  - **Imagem** (sistema operacional)
  - **Tamanho** (especificações de hardware)
  - **Nome de usuário e Senha** (ou chave SSH)

### Configurações avançadas:
#### Opções de Disponibilidade
- **Zona de Disponibilidade**: Escolha uma zona para aumentar a disponibilidade e redundância.
- **Contagem de Instâncias**: Defina o número de instâncias para escalar horizontalmente.

#### Portas de Entrada
- Configure regras de **segurança** para permitir tráfego nas portas necessárias, como **RDP (3389)** para Windows ou **SSH (22)** para Linux.

---

## 3. Discos

Os discos armazenam o sistema operacional e os dados da VM.

### Configurações:
- **Discos de Sistema**: Escolha o tipo e tamanho do disco para o sistema operacional.
- **Discos de Dados**: Adicione discos adicionais conforme necessário para armazenar dados.

### Excluir com a VM:
- Configure a VM para excluir os discos quando a máquina for excluída, garantindo que não permaneçam recursos órfãos.

---

## 4. Rede

Configure as opções de rede para sua VM.

### Configurações:
- **Excluir IP Público e NIC**: Configure a VM para remover o IP público e a interface de rede (NIC) quando a VM for excluída, para evitar recursos desnecessários.

---

## 5. Gerenciamento

Gerencie e mantenha sua VM para garantir desempenho e segurança.

### Ações recomendadas:
- **Monitoramento**: Utilize ferramentas de monitoramento e alertas para acompanhar o desempenho e a saúde da VM.
- **Backups**: Configure backups regulares para proteger dados importantes.
- **Atualizações**: Mantenha o sistema operacional e software atualizados para garantir segurança e estabilidade.

---

## Conclusão

Este guia fornece uma visão geral de como configurar e dimensionar suas máquinas virtuais no Azure, desde a criação até o gerenciamento de discos e opções de rede. Siga essas etapas para garantir que sua infraestrutura esteja bem configurada e otimizada.

---

**Referências adicionais:**
- [Documentação oficial do Azure sobre Máquinas Virtuais](https://learn.microsoft.com/pt-br/azure/virtual-machines/)
