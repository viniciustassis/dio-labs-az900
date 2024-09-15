# Laboratório: Criando uma Máquina Virtual Windows no Azure

Este guia passo a passo explica como criar uma máquina virtual (VM) com **Windows** no Azure, com base no exercício disponível na documentação oficial.

## Passos Resumidos:

### 1. Acesse o Portal do Azure
- No **Azure Portal**, busque por **Máquinas Virtuais** no menu de serviços.
- Clique em **Criar** e escolha **Máquina Virtual**.

### 2. Configurações Básicas da VM
- **Nome da VM**: Defina um nome para a máquina.
- **Região**: Escolha a localização do data center.
- **Imagem**: Selecione a imagem do **Windows Server** ou **Windows 10**.
- **Tamanho**: Selecione o tamanho da VM com base nas necessidades de CPU e memória.

### 3. Configurações de Administrador
- Crie um **nome de usuário** e defina uma **senha** para acessar a VM.
  
### 4. Configurar a Rede
- **Rede Virtual (VNet)**: Use a rede padrão ou crie uma nova.
- **Endereço IP público**: Habilite para se conectar à VM externamente via **RDP**.

### 5. Revisar e Criar
- Revise todas as configurações e clique em **Criar**.
- Aguarde enquanto a VM é provisionada.

### 6. Conectar-se à VM
- Após a criação, vá até a página da VM.
- Use o **RDP** para conectar-se à máquina com o IP público e as credenciais criadas.

---

## Conclusão

Este laboratório mostra como criar uma VM Windows no Azure de maneira simples. Siga esses passos para configurar e acessar sua máquina virtual rapidamente.

---

### Link para o tutorial completo:
[Documentação Azure - Exemplo de criação de uma VM Windows](https://learn.microsoft.com/pt-br/training/modules/create-windows-virtual-machine-in-azure/3-exercise-create-a-vm)
