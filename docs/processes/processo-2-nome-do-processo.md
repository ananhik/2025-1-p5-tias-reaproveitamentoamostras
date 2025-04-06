### 3.3.2 Processo 2 – TO BE Processo Cadastro e Gerenciamento das Amostras
 
_Apresente aqui o nome e as oportunidades de melhoria para o processo 2. 
Em seguida, apresente o modelo do processo 2, descrito no padrão BPMN._

![TO BE Processo Cadastro e Gerenciamento das Amostras](../images/process.png "Modelo BPMN do Processo 2.")


#### Detalhamento das atividades

_Descreva aqui cada uma das propriedades das atividades do processo 2. 
Devem estar relacionadas com o modelo de processo apresentado anteriormente._

_Os tipos de dados a serem utilizados são:_

_* **Área de texto** - campo texto de múltiplas linhas_

_* **Caixa de texto** - campo texto de uma linha_

_* **Número** - campo numérico_

_* **Data** - campo do tipo data (dd-mm-aaaa)_

_* **Hora** - campo do tipo hora (hh:mm:ss)_

_* **Data e Hora** - campo do tipo data e hora (dd-mm-aaaa, hh:mm:ss)_

_* **Imagem** - campo contendo uma imagem_

_* **Seleção única** - campo com várias opções de valores que são mutuamente exclusivas (tradicional radio button ou combobox)_

_* **Seleção múltipla** - campo com várias opções que podem ser selecionadas mutuamente (tradicional checkbox ou listbox)_

_* **Arquivo** - campo de upload de documento_

_* **Link** - campo que armazena uma URL_

_* **Tabela** - campo formado por uma matriz de valores_

**Registrar no sistema da amostra, quantidade, pedido, localização, validade e outros**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| quantidade     | Número  | deve ser varialvel tipo inteira |           0     |
| pedido           | Caixa de Texto   | não possui |      -     |
| localização          | Caixa de Texto   | não possui |    -       |
| validade        | Data  | não possui |     -      |

| **Comandos**         |  **Destino**                   | **Tipo** |
| ---                  | ---                            | ---               |
| Botão de Registrar              | iniício do processo de Atualizar catálogo de estoque e status    | default           |


**Atualizar catálogo de estoque e status**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| catálogo | imagem/área de texto  |      deve ser realizada automaticamente pelo sistema     |          -         |
|  status            |   caixa de texto          |     deve ser realizada automaticamente pelo sistema         |        -           |

| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| Atualização do catálogo |início do processo de Alertar fim do prazo de armazenagem obrigatória de 15 dias e status  | realizado pelo sistema |



**Alertar fim do prazo de armazenagem obrigatória de 15 dias e status**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| Alerta | área de texto/data  |atividade deve ser realizada pelo sistema|   -     |


| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| Alerta emetido pelo sistema |início do processo de Alertar proximidade do vencimento para amostras disponíveis | realizado pelo sistema  |


**Alertar proximidade do vencimento para amostras disponíveis**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| Alerta | área de texto/data  |atividade deve ser realizada pelo sistema|         -          |


| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| Alerta emetido pelo sistema | início do processo de Alertar amostras vencidas e solicitar descarte | realizado pelo sistema   |

**Alertar amostras vencidas e solicitar descarte**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| Alerta | área de texto/data  |atividade deve ser realizada pelo sistema|          -         |
|  Solicitar descarte               |     área de texto             |      atividade deve ser realizada pelo sistema          |           -        |

| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| Alerta emetido pelo sistema | Alerta gera a solicitação de descarte | realizado pelo sistema   |
|      Solicitar descarte                 |         início do processo de Atualizar status da amostra para vencida              |      realizado pelo sistema               |

**Atualizar status da amostra para vencida**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| Status | área de texto  |atividade deve ser realizada pelo sistema|          -         |


| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| Alerta emetido pelo sistema | Alerta gera a solicitação de descarte | realizado pelo sistema   |
|      Solicitar descarte                 |           início do processo de Descrtar amostra vencida                 |      realizado pelo sistema               |

**Descrtar amostra vencida**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| descartar amostras vencidas| tarefa manual  |atividade deve ser manualmente|        -           |


| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| descartar amostra | Fim do processo| realizado manualmente  |



