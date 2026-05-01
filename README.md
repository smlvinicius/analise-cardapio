# 📊 Análise de Cardápio - Restaurante Detroit
Este projeto tem como princípio analisar o cardápio de um restaurante, com o objetivo de extrair insights sobre preços e distribuição de produtos por categoria.

A análise busca responder perguntas como:

Qual categoria possui os produtos mais caros?
Onde estão concentrados os produtos?
Existe equilíbrio entre preço e quantidade?

# Objetivo 

Transformar dados brutos de cardápio em informações estratégicas, utilizando Power BI para:

> Criar indicadores chave (KPIs)    
> Visualizar padrões por categoria    
> Gerar insights acionáveis    
> Desenvolver dashboard profissional


# Coleta de Dados (Web Scraping)

Os dados utilizados neste projeto não foram coletados manualmente. Foi desenvolvido um processo de web scraping para extrair informações de um cardápio online.

Tecnologias utilizadas:

Python    
Pandas    
Requests    
BeautifulSoup

Etapas realizadas:

Requisição HTTP para obter os dados da página    
Conversão da resposta em JSON    
Estruturação dos dados em DataFrame    
Seleção dos campos relevantes (produto, preço, categoria)    

Esse processo permitiu simular um cenário real de ingestão de dados a partir de uma fonte externa.

# Processo de ETL

Foi implementado um fluxo simples de ETL para preparar os dados antes da análise.    


🔹 Extração    

Dados obtidos via API/web scraping

<img width="908" height="173" alt="image" src="https://github.com/user-attachments/assets/c1bc6e1c-53b7-412f-99b0-5e49c5d2177e" /> 


🔹 Transformação   

Limpeza de dados inconsistentes    
Conversão de tipos (preço → numérico)    
Padronização de categorias    
Remoção de duplicidades    

<img width="1088" height="529" alt="image" src="https://github.com/user-attachments/assets/55c946bf-c8f1-45ec-8470-b132a00928b0" />

🔹 Carga    

Exportação dos dados tratados para arquivo CSV    

<img width="797" height="69" alt="image" src="https://github.com/user-attachments/assets/d2fd9600-b705-4541-8525-c4fe5852cd71" />



# Modelagem de Dados    

Criação de medidas em DAX:

Preço Médio = AVERAGE(preco)    
Preço Máximo = MAX(preco)    
Preço Mínimo = MIN(preco)    
Total de Produtos = COUNT(product_name)    

Essas medidas alimentam os KPIs e gráficos do dashboard.

# Visualização

O dashboard foi estruturado com:    

KPIs:    

Preço médio    
Produto mais caro    
Produto mais barato    
Total de produtos    

Gráficos:    

Média de preço por categoria    
Comparação entre preço e quantidade    

Elementos adicionais:    

Ícones visuais    
Insights destacados    
Layout organizado e profissional    

Foco em clareza, leitura rápida e storytelling.    

<img width="2556" height="1385" alt="dashboard" src="https://github.com/user-attachments/assets/653375fd-c23d-4602-a351-afea2db04bda" />

# 🧠 Pipeline de Dados


O fluxo completo do projeto foi estruturado da seguinte forma:    

Coleta de dados via web scraping    
Tratamento e limpeza com Python (pandas)    
Exportação para CSV    
Importação no Power BI    
Modelagem com DAX    
Criação do dashboard    
Geração de insights    

Esse pipeline simula um fluxo real de engenharia e análise de dados.





