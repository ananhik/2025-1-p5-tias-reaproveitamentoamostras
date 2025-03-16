# Especificação do projeto

<span style="color:red">Pré-requisitos: <a href="01-Contexto.md"> Documentação de contexto</a></span>

Definição do problema e ideia de solução a partir da perspectiva do usuário. É composta pela definição do  diagrama de personas, histórias de usuários, requisitos funcionais e não funcionais além das restrições do projeto.

Apresente uma visão geral do que será abordado nesta parte do documento, enumerando as técnicas e/ou ferramentas utilizadas para realizar a especificações do projeto.

## Personas

|PERSONA|IDADE |PROFISSÃO|DESCRIÇÃO|OBJETIVOS|
|------|-------------------|-------------|-------------|-------------|
|1. Maria de Jesus|38 anos|Coordenadora de ONG de segurança alimentar|Ana trabalha na administração de uma ONG que distribui alimentos para comunidades vulneráveis. Possui conhecimento básico em tecnologia e precisa de um sistema simples e funcional para receber e solicitar doações|Facilitar o acesso a doações regulares de alimentos para atender famílias em situação de vulnerabilidade|
|2. Eduardo Martins|42 anos|Funcionário da Clastec|Eduardo é responsável pelo controle de qualidade das amostras analisadas pela Clastec. Ele precisa de uma ferramenta eficiente para gerenciar a disponibilização das amostras reaproveitáveis|Registrar e disponibilizar amostras para doação, reduzindo desperdícios|
|3. Marcos Silva|50 anos|Funcionário da Clastec|Marcos trabalha na área de logística da Clastec e é responsável por organizar a separação das amostras e coordenar sua retirada pelos beneficiários|Confirmar com o beneficiário a retirada da amostra e atualizar o status da amostra como "Indisponível" no sistema|
|4. Patrícia Oliveira|35 anos|Diretora da Clastec|Patrícia é diretora da Clastec e precisa acompanhar o andamento do projeto para garantir que a redistribuição das amostras seja eficiente e transparente|Visualizar um painel com informações sobre amostras disponíveis, doações realizadas e instituições/pessoas beneficiadas|
|5. Ricardo Gomes|46 anos|Funcionário da Clastec|Ricardo é responsável por definir as permissões de acesso ao sistema e gerenciar os funcionários envolvidos na redistribuição das amostras|Cadastrar os funcionários que podem gerenciar as amostras e confirmar a entrega das doações|



Exemplo: _Pedro Paulo tem 26 anos, é arquiteto recém-formado e autônomo. Pensa em se desenvolver profissionalmente por meio de um mestrado fora do país, pois adora viajar, é solteiro e sempre quis fazer um intercâmbio. Está buscando uma agência que o ajude a encontrar universidades na Europa que aceitem alunos estrangeiros._

Enumere e detalhe as personas da sua solução. Para tanto, baseie-se tanto nos documentos disponibilizados na disciplina e/ou nos seguintes links:

> **Links úteis**:
> - [Rock content](https://rockcontent.com/blog/personas/)
> - [Hotmart](https://blog.hotmart.com/pt-br/como-criar-persona-negocio/)
> - [O que é persona?](https://resultadosdigitais.com.br/blog/persona-o-que-e/)
> - [Persona x público-alvo](https://flammo.com.br/blog/persona-e-publico-alvo-qual-a-diferenca/)
> - [Mapa de empatia](https://resultadosdigitais.com.br/blog/mapa-da-empatia/)
> - [Mapa de stalkeholders](https://www.racecomunicacao.com.br/blog/como-fazer-o-mapeamento-de-stakeholders/)
>
Lembre-se que você deve ser enumerar e descrever precisamente e personalizada todos os clientes ideais que sua solução almeja.

## Histórias de usuários

Com base na análise das personas, foram identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Membro de ONG  | Receber notificações sobre alimentos disponíveis para doação e informar meu interesse em receber os alimentos | Contribuir no projeto de arrecadação e distribuição de alimentos da ONG |
|Funcionário da Clastec| Registrar e disponibilizar alimentos para doação | Evitar desperdício e otimizar a redistribuição |
|Funcionário da Clastec| Confirmar com o beneficiado a separação da amostra e os detalhes para retirada. Além de atualizar o status da amostra como "Indisponível". | Evitar desperdício e otimizar a redistribuição |
|Diretor da Clastec| Visualizar um painel de amostras disponíveis, amostras doadas e quem recebeu a doação | Acompanhar o andamento da redistribuição e ver o histórico de doações |
|Diretor da Clastec| Cadastrar os funcionários que podem gerenciar as amostras e confirmar a entrega das doações. | Garantir permissões adequadas no sistema |

## Requisitos

As tabelas a seguir apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade dos requisitos, aplique uma técnica de priorização e detalhe como essa técnica foi aplicada.

### Requisitos funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir que o usuário cadastre tarefas | ALTA | 
|RF-002| Emitir um relatório de tarefas no mês   | MÉDIA |

### Requisitos não funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser responsivo para rodar em dispositivos móveis | MÉDIA | 
|RNF-002| Deve processar as requisições do usuário em no máximo 3 segundos |  BAIXA | 

Com base nas histórias de usuários, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos não funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).

Lembre-se de que cada requisito deve corresponder a uma e somente uma característica-alvo da sua solução. Além disso, certifique-se de que todos os aspectos capturados nas histórias de usuários foram cobertos.

> **Links úteis**:
> - [O que são requisitos funcionais e requisitos não funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [Entenda o que são requisitos de software, a diferença entre requisito funcional e não funcional, e como identificar e documentar cada um deles](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

## Restrições

Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

O projeto está restrito aos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|001| O projeto deverá ser entregue até o final do semestre |
|002| O custo total do projeto não deve exceder o orçamento definido       |

## Diagrama de casos de uso

O diagrama de casos de uso é o próximo passo após a elicitação de requisitos. Ele utiliza um modelo gráfico e uma tabela com as descrições sucintas dos casos de uso e dos atores. O diagrama contempla a fronteira do sistema e o detalhamento dos requisitos funcionais, com a indicação dos atores, casos de uso e seus relacionamentos.

As referências abaixo irão auxiliá-lo na geração do artefato “diagrama de casos de uso”.

> **Links úteis**:
> - [Criando casos de uso](https://www.ibm.com/docs/pt-br/engineering-lifecycle-management-suite/design-rhapsody/10.0?topic=cases-creating-use)
> - [Como criar diagrama de caso de uso: tutorial passo a passo](https://gitmind.com/pt/fazer-diagrama-de-caso-uso.html/)
> - [Lucidchart](https://www.lucidchart.com/)
> - [Astah](https://astah.net/)
> - [Diagrams](https://app.diagrams.net/)
