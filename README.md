# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 22/08/2025
**Empresa:** Farmácia Vida Saudável
**Responsável:** Lucas Santos do Amaral

---

## Introdução
Este relatório apresenta o processo inicial de implementação de ferramentas em nuvem na **Farmácia Vida Saudável**, realizado por **Lucas Santos do Amaral**.

 **Objetivos do projeto:**
- Reduzir custos de infraestrutura.
- Garantir maior segurança no armazenamento de informações.
- Disponibilizar recursos que facilitem a operação diária da farmácia.

Como a empresa nunca havia utilizado serviços em nuvem, foi necessário aplicar soluções básicas e de fácil manutenção, garantindo entendimento gradual da equipe.

---

##  Descrição do Projeto

O projeto de implementação foi dividido em **3 etapas principais**, cada uma representando um serviço da AWS.

### Etapa 1: **Amazon S3**
- **Foco da ferramenta:** Armazenamento em nuvem seguro e escalável.
- **Caso de uso:**
  A farmácia poderá armazenar documentos importantes, como relatórios de vendas, notas fiscais digitais e registros de fornecedores, sem depender apenas de HDs locais.
   Isso reduz riscos de perda de dados e diminui custos com servidores físicos.

---

### Etapa 2: **Amazon RDS (MySQL)**
- **Foco da ferramenta:** Banco de dados gerenciado.
- **Caso de uso:**
  A farmácia terá um banco de dados centralizado para cadastro de clientes, controle de estoque e histórico de vendas.
   Com o RDS, a empresa não precisará se preocupar com atualizações manuais e backup, pois a AWS faz essa gestão automaticamente.

---

### Etapa 3: **Amazon EC2**
- **Foco da ferramenta:** Servidor virtual na nuvem.
- **Caso de uso:**
  Um servidor leve foi configurado para hospedar o sistema interno da farmácia (como controle de caixa e estoque).
   Isso permite que os funcionários acessem o sistema de qualquer filial ou local autorizado, garantindo flexibilidade e escalabilidade.

---

##  Conclusão
A implementação de serviços AWS na **Farmácia Vida Saudável** proporcionará:
-  Redução de custos com servidores locais e manutenção.
- Maior segurança no armazenamento de documentos e dados sensíveis.
- Facilidade de acesso remoto ao sistema da farmácia.

Recomenda-se que a farmácia continue utilizando esses serviços e, futuramente, explore novas ferramentas da AWS, como **CloudWatch** (monitoramento) e **AWS Backup**, para aumentar ainda mais a eficiência operacional.

---

###  Guia básico de acesso ao Amazon S3
- **Objetivo:** Ensinar como acessar e gerenciar os arquivos na nuvem.
- **Passos principais:**
  1. Acesse o [AWS Management Console](https://aws.amazon.com/console/).
  2. Faça login com seu usuário da farmácia.
  3. Navegue até o serviço **S3**.
  4. Crie ou abra um bucket (pasta na nuvem) para armazenar documentos.
  5. Faça upload dos arquivos da farmácia para o bucket.

---

###  Manual de login no sistema hospedado em EC2
- **Objetivo:** Acessar o sistema interno da farmácia via servidor na nuvem.
- **Passos principais:**
  1. Abra o terminal ou cliente SSH (como [PuTTY](https://www.putty.org/)).
  2. Conecte usando o IP público do servidor EC2 e a chave privada fornecida.
  3. Digite as credenciais do sistema da farmácia.
  4. Navegue pelo sistema e confirme que todos os módulos estão funcionando.

---

### Estrutura inicial do banco de dados no RDS
- **Objetivo:** Entender como os dados da farmácia estão organizados na nuvem.
- **Tabelas principais:**

| Tabela       | Descrição                          |
|-------------|-----------------------------------|
| Clientes    | Nome, CPF, telefone, endereço     |
| Produtos    | Código, nome, quantidade, preço   |
| Vendas      | Data, produto, cliente, valor     |
| Estoque     | Produto, quantidade atual, limite |

- **Observações:**
  - Todos os backups são automáticos pelo RDS.
  - É possível acessar o banco via ferramentas como MySQL Workbench ou DBeaver.
---

## Responsável pelo Projeto
Lucas Santos do Amaral




