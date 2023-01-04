# Definição de Orgamento de Billing na Google Cloud Plataform


Neste momento iremos permitir a definição alertas de orçamento para controlar o uso de recursos dentro de nossa arquitetura de organização de nossa plataforma da GCP de forma eficiente.

### Para acessar o menu:

<a href="https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/GoogleCloudPlatform/java-docs-samples&page=editor&open_in_editor=appengine-java11/README.md">
<img alt="Open in Cloud Shell" src ="https://user-images.githubusercontent.com/32373902/210641943-86dc6428-dfaf-4391-a472-758d91af0533.png" width=250 ></a>

- No menu lateral esquerdo, selecione:
    - **Faturamento → Orçamentos e alertas**
    

### Crie e nomeie o orçamento

**Escopo:**

1. No prompt, **escolha a conta de faturamento do Cloud** em que você quer definir um orçamento. A página *Orçamentos e alertas* é aberta para a conta de faturamento selecionada.
2. Clique em **Criar orçamento**.
3. Vamos determinar o escopo do alerta
    1. No campo **Nome**, insira um nome para o orçamento.
    2. O intervalo em que esse alerta irá funcionar
    3. Selecione os **Projetos** que compõem esse alerta
        1. Foram selecionados dois projetos
    4. Selecione os **Serviços** que compõem esse alerta
        1. Foram limitados a **todos** os serviços do GCP
        
    ![Screenshot_1](https://user-images.githubusercontent.com/32373902/210639392-598eb214-caac-4997-b3b3-34a8a2b8bd42.png)
    
************Valor:************

1. Vamos selecionar o tipo de orçamento como **Valor Especificado**
2. Selecionar o valor desejado para nosso alerta
    1. No momento como temos **R$ 2.387,82**, vamos limitar a **R$ 2.000** para questões de organização entre projetos
    
      ![Screenshot_2](https://user-images.githubusercontent.com/32373902/210639397-0a439994-7463-4684-a0fa-b5e1e12f1328.png)
      
    2. Assim que configurar o valor é possível  determinar o threshold para determinar a porcentagem do alerta 
    
      ![Screenshot_3](https://user-images.githubusercontent.com/32373902/210639398-411e05ac-2ba6-4d71-9dc2-13dba5f9d87e.png)


**Notificações:**

1. É necessário selecionar quais serão quais serão os usuários que receberão os alertas, bem como, criar canais de notificação

![Screenshot_4](https://user-images.githubusercontent.com/32373902/210639399-1beead2e-73d3-4b4d-827c-dd3466af2938.png)


## Exportação de Faturamento

É possível exportar nossas tabelas de faturamento utilizando o ************BIGQUERY EXPORT,************ criando um conjunto de dados.



1. Vá no menu lateral em faturamento, selecione:
    1. Exportação de Faturamento




![Screenshot_5](https://user-images.githubusercontent.com/32373902/210639401-9cb92645-fb48-494e-ac7d-7041737a5eed.png)
