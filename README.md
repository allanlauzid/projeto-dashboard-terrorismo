# projeto-dashboard-terrorismo

Dashboard de Análise de Eventos Terroristas (1970-2021)
Arquivo .pbix com Dashboard e Documentação do mesmo em .pdf e abaixo.


Documentação do Dashboard de Análise de Eventos Terroristas (1970-2021) 

Faculdade Nova Roma 

Prof.: Davi Maia 
 
Allan	Lauzid 

 
Objetivo
Este dashboard foi desenvolvido para analisar eventos terroristas globais de 1970 a 2021, fornecendo insights sobre padrões temporais, impacto geográfico e tipos de ataques. Utiliza elementos visuais interativos e operações OLAP para facilitar a exploração dos dados.
 
Escolha dos Elementos Visuais
1. Mapa de Bolha
Objetivo:
  Explorar o impacto geográfico dos ataques terroristas.
 
Por quê?
  Este visual permite identificar rapidamente os países mais afetados, destacando o número de mortes por ataque em cada região.
 
Configuração:
  Eixo de Localização: country_txt (País).
  Tamanho: nkill (Número de Mortes).
 
2. Gráfico de Linha
Objetivo:
  Analisar a evolução do número de ataques e mortes ao longo do tempo. 
 
Por quê?
  Exibe padrões temporais, como picos em anos específicos, ajudando a entender períodos de maior intensidade.
 
Configuração:

  Eixo X: iyear (Ano).
  
  Eixo Y: nkill (Número de Mortes).
 
 
3. Gráfico de Barras (Distribuição por Tipo de Ataque):
Objetivo:
  Comparar a frequência de mortes por diferentes tipos de ataques.

Por quê?
  Ajuda a identificar quais ataques causaram mais impacto em termos de vítimas.

Configuração:
  Eixo Y: attacktype1_txt(Tipo de Ataque).
  Valores: nkill (Número de Mortes).
 
 
Operações OLAP
 
1. Drill-Down e Drill-Up:
 
  Uso: No gráfico de linha, foi implementada uma hierarquia de dados (Ano → Mês → Dia), permitindo que o usuário amplie ou reduza o nível de detalhamento temporal.
  Benefício: Detalhamento de eventos em períodos específicos, como analisar ataques em um mês específico.
 
2. Slice and Dice:
  Uso: Filtros para country_txt (País) e attacktype1_txt (Tipo de Ataque) foram adicionados.
 
Benefício: Exploração segmentada dos dados, permitindo análises personalizadas, como visualizar apenas ataques em um país específico.
 
3. Ranking:

  Uso: No gráfico de barras, foi configurada uma classificação para exibir os 5 maiores tipos de ataque em termos de mortes.
  Benefício: Destaque para os ataques mais letais, facilitando a priorização da análise.
 
 
Design do Dashboard
1. Minimalismo:
 o Por quê?
  Um design claro e simples reduz distrações efacilita a interpretação rápida dos dados.
 o Implementação:
   ▪ Esquema de cores consistente e neutro.
   ▪ Elementos visuais espaçados para evitar sobrecarga de informações.
   ▪ Rótulos e títulos explicativos.
2. Interatividade:
 o Adicionados filtros dinâmicos para que o usuário possa explorar diferentes perspectivas dos dados sem sair da interface principal.


Conclusão
 Este dashboard atende aos objetivos de análise, permitindo:
 • Identificar padrões temporais e geográficos de ataques.
 • Explorar interativamente os dados com filtros e drill-down.
 • Destacar ataques mais letais com ranking.
 O uso combinado de gráficos e operações OLAP proporciona uma experiência analítica rica, clara e focada, promovendo insights significativos sobre a complexidadedos eventos terroristas globais.
