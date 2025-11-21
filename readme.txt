Sistema de Apoio à Decisão para Otimização de Estoque em Pequenas Empresas de Varejo usando IA (SADE-OE)
Nome/Matrícula dos Integrantes: 
Esther Rodrigues da Conceição- 294690
  Kálita da Silva Nunes de Souza-342113
  Louise Victória Amorim da Silva- 341456
  Vanderleia de Arruda Rondon- 344659
Descrição do Processo Mapeado e Problema Identificado: O processo mapeado é a Gestão de Estoque em Pequenas Empresas de Varejo. O problema central é a ineficiência e a imprecisão na tomada de decisão de compra de produtos, que atualmente é baseada em métodos manuais, planilhas simples ou intuição.
Mapeamento do Processo Manual Atual (Conforme Diretrizes)
Para atender às diretrizes de mapeamento de processo, o processo manual de gestão de estoque, que o SADE-OE visa otimizar, é detalhado a seguir:
Etapa	Responsável	Tempo Médio	Entradas	Saídas	Decisões Envolvidas
1. Verificação de Estoque	Vendedor/Gerente	1 hora/dia	Estoque Físico, Planilha de Estoque	Nível de Controle Atual	Nenhuma (Apenas coleta)
2. Análise de Vendas	Gerente	2 horas/semana	Histórico de Vendas (Notas/Planilha)	Tendência de Vendas (Intuitiva)	Qual produto precisa de reposição?
3. Decisão de Compra	Gerente/Dono	10 min/decisão	Nível de Estoque Atual, Tendência de Vendas (Intuitiva)	Pedido de Compra	Qual quantidade comprar? (Decisão baseada em intuição/experiência)
4. Recebimento e Armazenamento	Estoquista	1 hora/entrega	Pedido de Compra, Produtos Recebidos	Estoque Físico Atualizado	O produto recebido confere com o pedido?
Gargalos e Falhas Percebidas no Processo (Diretriz 1)
A ineficiência do processo manual resulta em dois gargalos principais:
1.	Excesso de estoque: A compra em demasia gera custos de armazenagem e risco de obsolescência.
2.	Falta de estoque (ruptura): A compra insuficiente resulta em perda de vendas e insatisfação do cliente.
A lacuna identificada é a ausência de uma análise preditiva robusta que considere o histórico de vendas e fatores contextuais (sazonalidade, promoções, eventos) para otimizar o ponto de reposição.
Solução Proposta (IA):
A solução proposta é a implementação de um Sistema de Apoio à Decisão para Otimização de Estoque (SADE-OE) baseado em Machine Learning (ML). Este sistema utiliza algoritmos de previsão de demanda para analisar dados históricos de vendas e eventos contextuais, gerando uma recomendação de compra otimizada. A solução se enquadra no uso de Inteligência Artificial para aprimorar a tomada de decisão gerencial.
Fluxograma do Processo Otimizado (SADE-OE) (Diretriz 2)
A seguir, a representação visual do fluxo do processo otimizado pelo SADE-OE, que substitui as etapas manuais de Análise de Vendas e Decisão de Compra:
(Nota: O fluxograma não pôde ser extraído como imagem, mas o texto descreve que ele substitui as etapas 2 e 3 do processo manual.)
Descrição Resumida do Funcionamento do Protótipo:
O protótipo simula a funcionalidade central do SADE-OE utilizando o ChatGPT. Ele atua como um motor de análise e recomendação. O usuário fornece o nome do produto, o estoque atual, o histórico de vendas dos últimos quatro meses e quaisquer eventos contextuais relevantes para o próximo período. O protótipo processa essas informações, identifica tendências e o impacto dos eventos (como a Black Friday), estima a demanda futura e, por fim, calcula a quantidade ideal de unidades a serem compradas (Previsão - Estoque Atual), apresentando o resultado em um Relatório de Decisão estruturado.
Cópia dos Prompts e Respostas do ChatGPT Utilizados:
[PROMPT DE SISTEMA] Aja como um Sistema de Apoio à Decisão para Otimização de Estoque (SADE-OE) baseado em Machine Learning. Seu objetivo é analisar dados históricos de vendas e fatores contextuais para gerar um Relatório de Decisão de Compra, minimizando o risco de excesso ou falta de estoque para uma pequena empresa de varejo.
Instruções: 1. Entrada de Dados: O usuário fornecerá o nome do produto, o histórico de vendas dos últimos 4 meses (em unidades) e quaisquer eventos contextuais relevantes (ex: feriados, promoções). 2. Análise: Você deve analisar os dados para identificar tendências, sazonalidade e o impacto dos eventos contextuais. 3. Previsão: Estime a demanda para o próximo mês (Mês 5). 4. Relatório de Decisão: Gere um relatório estruturado com a Previsão de Demanda, o Estoque Atual (fornecido pelo usuário) e a Sugestão de Compra (Previsão - Estoque Atual). A Sugestão de Compra deve ser zero se o Estoque Atual for maior ou igual à Previsão.
[INTERAÇÃO DE EXEMPLO - ENTRADA DO USUÁRIO] * Produto: Camiseta Básica Branca * Estoque Atual: 50 unidades * Histórico de Vendas (Unidades): * Mês 1 (Julho): 100 * Mês 2 (Agosto): 120 * Mês 3 (Setembro): 130 * Mês 4 (Outubro): 250 * Eventos Contextuais: * Outubro teve uma promoção de “Leve 2 Pague 1” que impulsionou as vendas. * Novembro (Mês 5) é o mês da Black Friday.
RELATÓRIO DE DECISÃO DE COMPRA - SADE-OE
Produto: Camiseta Básica Branca
1.	Análise de Dados Históricos:
–	Tendência: As vendas mostram uma tendência de crescimento, com um pico notável em Outubro (250 unidades).
–	Sazonalidade/Contexto: O pico de Outubro é claramente influenciado pela promoção “Leve 2 Pague 1”. A média de vendas sem o pico (Julho a Setembro) é de 116.6 unidades. No entanto, a proximidade da Black Friday em Novembro (Mês 5) sugere um potencial de demanda muito alta, superando o pico de Outubro.
2.	Previsão de Demanda (Mês 5 - Novembro): Considerando a tendência de alta e o forte impacto esperado da Black Friday, a demanda é projetada para ser significativamente maior do que o pico de Outubro.
–	Previsão de Demanda para Novembro: 300 unidades
3.	Decisão de Compra:
–	Previsão de Demanda (Novembro): 300 unidades
–	Estoque Atual: 50 unidades
–	Sugestão de Compra (Previsão - Estoque Atual): 300 - 50 = 250 unidades
Recomendação: Recomenda-se a compra de 250 unidades da Camiseta Básica Branca para atender à demanda prevista para a Black Friday, minimizando o risco de ruptura de estoque e maximizando o potencial de vendas.
