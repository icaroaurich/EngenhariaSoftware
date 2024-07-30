# EngenhariaSoftware
# Plano de Projeto para Sistema de Controle de Portarias

## 01 - Introdução
O Instituto Federal da Bahia campus Eunápolis emite anualmente centenas de portarias com diversas finalidades. O processo atual de criação e controle de portarias é ineficiente, dificultando respostas rápidas a perguntas cruciais, como a vigência de portarias, membros de comissões e vencimentos de prazos. Este projeto visa desenvolver uma solução digital para gerenciar portarias e comissões de maneira eficiente, melhorando a acessibilidade e a gestão dessas informações.

## 02 - Organização
O projeto será desenvolvido por uma equipe de três pessoas:

- **Ícaro** - **Líder do Projeto**: Responsável pela coordenação geral do projeto, definição de requisitos, comunicação com stakeholders, e supervisão do desenvolvimento.
- **Anderson** - **Gerente de Desenvolvimento**: Responsável pelo desenvolvimento das funcionalidades principais, revisão de código, e garantia de qualidade do software.
- **Thiago** - **Desenvolvedor Júnior**: Responsável por auxiliar na programação de funcionalidades, realizar testes unitários, e ajudar na documentação do sistema.

## 03 - Análise de Risco
- **Risco:** Atrasos na entrega dos requisitos pelo IFBA.
  - **Mitigação:** Definir um cronograma claro e realizar reuniões semanais para acompanhamento.
- **Risco:** Falhas técnicas na integração com sistemas existentes.
  - **Mitigação:** Realizar testes detalhados e ter um plano de contingência.

## 04 - Requisitos de Hardware/Software
- **Hardware:**
  - Servidores com especificações mínimas de processador, memória e armazenamento.
- **Software:**
  - Sistema Operacional: Windows Server.
  - Banco de Dados: MySQL.
  - Framework de Desenvolvimento: Django (Python) ou PHP.
  - Ferramentas de Integração: APIs para integração com sistemas existentes do IFBA.

## 05 - Tarefas
- **Levantamento de Requisitos**
- **Desenvolvimento do Sistema**
  - **Design de Interface**
  - **Programação de Funcionalidades**
    - **Funcionalidades Básicas Iniciais (Módulo de Pessoas)**
      - **Perfis de usuário:**
        - LEITOR (perfil público, sem necessidade de autorização de acesso).
        - GESTOR (perfil privado, necessita de autorização de acesso).
      - **Usuário GESTOR:**
        - Capaz de cadastrar, editar e excluir pessoas.
      - **Usuários GESTOR e LEITOR:**
        - Capazes de listar e visualizar pessoas.
        - Capazes de buscar pessoas.
      - **Cadastro de pessoas:**
        - Nome.
        - Matrícula (opcional).
        - CPF.
        - Área de atuação / Especialidade.
      - **Listagem de pessoas:**
        - Informar todas as portarias vinculadas à pessoa.
      - **Relatórios gerenciais:**
        - Lista de pessoas e suas comissões (possível inserir uma faixa de datas).
        - Lista de pessoas ordenadas pelo número de comissões de que fazem parte.

    - **Funcionalidades Básicas Iniciais (Módulo de Portarias)**
      - **Perfis de usuário:**
        - LEITOR (perfil público, sem necessidade de autorização de acesso).
        - GESTOR (perfil privado, necessita de autorização de acesso).
      - **Usuário GESTOR:**
        - Capaz de cadastrar, editar e excluir portarias.
      - **Usuários GESTOR e LEITOR:**
        - Capazes de listar e visualizar portarias.
        - Capazes de buscar portarias.
      - **Relacionamento entre portarias:**
        - Informar o tipo de relacionamento entre portarias (ex.: uma portaria altera o conteúdo de uma anterior).
      - **Cadastro de portarias:**
        - Número.
        - Data.
        - Processo SEI (opcional).
        - Resumo (motivação da portaria).
        - Validade (opcional).
        - Observação (informações pertinentes contidas ou não na portaria; opcional).
        - Arquivo (opcional).
      - **Estados das portarias:**
        - Em vigor, vencida, revogada e alterada.
      - **Relatórios gerenciais:**
        - Lista de portarias (possível inserir uma faixa de data).
        - Informações detalhadas de uma portaria.

    - **Funcionalidades Básicas Iniciais (Módulo de Comissões)**
      - **Perfis de usuário:**
        - LEITOR (perfil público, sem necessidade de autorização de acesso).
        - GESTOR (perfil privado, necessita de autorização de acesso).
      - **Usuário GESTOR:**
        - Capaz de cadastrar, editar e excluir comissões.
      - **Usuários GESTOR e LEITOR:**
        - Capazes de listar e visualizar comissões.
        - Capazes de buscar comissões.
      - **Relacionamento com portarias:**
        - Toda comissão é vinculada a uma ou mais portarias, como a portaria que designa a comissão.
        - O sistema deve listar, na tela de comissões, todas as portarias vinculadas a ela.
      - **Membros da comissão:**
        - Toda comissão possui um ou mais membros (não necessariamente servidores do IFBA).
      - **Cadastro de comissões:**
        - Portarias vinculadas.
        - Membros.
        - Se é permanente ou não.
        - Prazo de validade da comissão.
        - Motivação da comissão.
      - **Relatórios gerenciais:**
        - Lista de comissões (possível inserir uma faixa de data).
        - Informações detalhadas de uma comissão.
  - **Testes Unitários e Integrados**
- **Implantação do Sistema**
  - Treinamento de Usuários
  - Migração de Dados
- **Suporte e Manutenção**

## 06 - Cronograma
- **Mês 1:** Levantamento de Requisitos e Planejamento
- **Mês 2-3:** Desenvolvimento do Sistema
- **Mês 4:** Testes e Correções
- **Mês 5:** Implantação e Treinamento
- **Mês 6:** Suporte e Manutenção

## 07 - Monitoramento e Reportagem
O progresso do projeto será monitorado através de reuniões semanais de status, relatórios mensais de progresso, e ferramentas de gerenciamento de projetos como o Microsoft Project ou Trello. Relatórios detalhados serão enviados aos principais stakeholders, destacando marcos alcançados, tarefas pendentes e quaisquer riscos ou problemas identificados.
