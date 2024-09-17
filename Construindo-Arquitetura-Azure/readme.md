# Construindo Arquiteturas no Azure

Este guia apresenta os principais passos para construir arquiteturas de rede no **Azure**, começando pela criação de um grupo de recursos, rede virtual e usando ferramentas de visualização e logs de atividade.

---

## 1. Criar Grupo de Recursos

Um **grupo de recursos** é um contêiner lógico no qual você pode gerenciar e organizar recursos no Azure.

### Como criar:
- No **Azure Portal**, navegue até **Grupos de Recursos**.
- Clique em **Criar** e preencha os detalhes, como **Nome** e **Região**.
- Finalize clicando em **Revisar e Criar**.

---

## 2. Criar Rede Virtual (VNet)

A **Rede Virtual (VNet)** permite a comunicação segura entre os serviços e máquinas virtuais (VMs) no Azure. 

### Como criar:
- No **Portal do Azure**, vá para **Rede Virtual**.
- Clique em **Criar** e insira as informações como **Nome**, **Endereço IP** e **Sub-rede**.
- Escolha a **região** para a VNet, que deve ser a mesma do grupo de recursos.

### Opção "Baixar" para Automação de Código:
Após a criação da VNet, o Azure oferece a opção de baixar o **template ARM**. Esse template pode ser utilizado para automatizar o processo de criação via código, permitindo que a mesma configuração seja aplicada em diferentes ambientes sem a necessidade de passar pelo portal.

- Na página de conclusão da criação da VNet, clique em **Baixar** para obter o código JSON do template ARM.

---

## 3. Visualizador de Recursos

O **Visualizador de Recursos** é uma ferramenta útil para inspecionar a configuração de todos os recursos dentro do Azure, como uma visão completa da VNet e seus componentes.

### Como usar:
- No **Azure Portal**, selecione a VNet criada.
- Clique em **Visualizador de Recursos** para examinar todos os detalhes da rede, como endereços IP, sub-redes e outros recursos associados.

Essa ferramenta é útil para verificar as configurações de infraestrutura em detalhes.

---

## 4. Log de Atividade

O **Log de Atividade** no Azure permite que você monitore todas as ações e mudanças que ocorreram em seus recursos.

### Como acessar:
- No **Portal do Azure**, vá até o **Grupo de Recursos**.
- Selecione **Log de Atividade** no menu lateral.
- Filtre os logs por **data** e **evento** para visualizar alterações ou atividades recentes, como criação de VMs, mudanças de configuração e uso da rede.

---

## Conclusão

Seguindo esses passos, você estará preparado para construir e gerenciar sua arquitetura de rede no Azure, desde a criação de grupos de recursos e redes virtuais até o uso de ferramentas de automação e monitoramento de logs.

---

**Referências adicionais:**
- [Documentação oficial do Azure](https://learn.microsoft.com/pt-br/azure)

