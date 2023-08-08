# Descrição das opções que aparecem ao criar uma Máquina Virtual

## Create a virtual machine

### Basics

- **Project Details**
  - **Subscription** =>  Assinatura que da VM
    - **Resource Group** => Grupo de Recurso da VM

- **Instance details**
  - **Virtual machine name** => Nome da VM
  - **Region** => Região da VM
  - **Availability options** =>
  - **Security type** =>
  - **Image** =>
  - **VM Architecture** => Arquitetura da VM
  - **Run with Azure Spot discount** => Usa a capacidade de computação do Azure não utilizada. A VM fica mais barata mas pode haver interrupções. Não usar em ambientes críticos.
    - **Eviction type**
      - **Only Capacity:** => Sua máquina virtual será removida quando o excesso de capacidade do Azure desaparecer.
      - **Price ou capacity:**  => Sua máquina virtual será removida quando o excesso de capacidade do Azure desaparecer ou os custos excederem o preço máximo especificado.
    - **Eviction policy** [^1]
      - **Stop/Deallocate** => A VM será desalocada permitindo que seja reimplementada novamente (sem garantia que terá êxito). Terá cobrança pelos custos de armazenamento.
      - **Delete** => A VM será removida.
  - **Size** => 

- **Administrator account**
  - **Authentication type** =>
  - **Username** => 

[^1]: Microsoft Learn https://learn.microsoft.com/pt-br/azure/virtual-machines/spot-vms#eviction-policy
