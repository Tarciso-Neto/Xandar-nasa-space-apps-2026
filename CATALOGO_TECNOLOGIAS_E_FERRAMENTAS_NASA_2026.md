# MALETA DE FERRAMENTAS — NASA SPACE APPS CHALLENGE 2026

**Equipe:** NASA Space Apps Challenge — Vitória da Conquista, BA  
**Versão:** 2.0 — revisão ampliada · **Consulta às fontes:** 30/10/2026  
**Objetivo:** catálogo de escolha rápida de tecnologias, IA, dados, design, análise, matemática, APIs, visualização e apresentação, sem pressupor qual desafio será escolhido.

> **IMPORTANTE:** esta é uma lista de opções, não uma recomendação de usar tudo ao mesmo tempo. Para um hackathon curto, a ferramenta mais valiosa é aquela que o time já domina. Quando escolhermos o desafio, extrairemos daqui uma *stack mínima*. Preparação de contas, ambientes e materiais deve respeitar as regras sobre o que pode ser feito antes do início da competição; esta maleta não autoriza antecipar o desenvolvimento do projeto.

## Resultado da revisão — o que mudou nesta versão

A versão 2.0 mantém o catálogo anterior e amplia a cobertura de necessidades que estavam ausentes ou pouco explicadas. A revisão foi feita pelo **ciclo do projeto**, e não apenas acrescentando marcas: obter dados → validar → analisar → construir → publicar → proteger → demonstrar → documentar.

**Principais acréscimos:** leitura de formatos científicos; radar e astronomia; incerteza e unidades; agentes de programação e construtores de aplicativos com IA; IA no navegador; aplicativos móveis e funcionamento offline; sonificação; e-mail transacional; cache e automação; segurança; rastreabilidade e documentação.

| Ajuste relevante            | Orientação revisada                                                                                     | Fonte primária                                                                                |
| --------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| E-mails de autenticação     | Não presumir que Supabase Auth enviará mensagens a qualquer visitante sem configuração adicional        | [Supabase SMTP](https://supabase.com/docs/guides/auth/auth-smtp)                              |
| Banco temporário            | Render Postgres Free expira em 30 dias; não confundir com a hospedagem gratuita da API                  | [Render Free](https://render.com/docs/free)                                                   |
| Armazenamento Firebase      | Storage exige Blaze/faturamento; o plano gratuito de outro produto não se estende automaticamente a ele | [Firebase](https://firebase.google.com/docs/storage/faqs-storage-changes-announced-sept-2024) |
| Chaves e segurança          | Chave publicável de cliente não é chave secreta; a proteção dos registros depende das permissões/RLS    | [Supabase API keys](https://supabase.com/docs/guides/getting-started/api-keys)                |
| Biblioteca legada           | poliastro está arquivado; a escolha para um novo projeto exige cautela                                  | [Mantenedor](https://github.com/poliastro/poliastro)                                          |
| Gratuidade e colaboração    | Excalidraw inclui colaboração básica gratuita; serviço pago adicional é separado                        | [Excalidraw](https://github.com/excalidraw/excalidraw)                                        |
| Computação para demos de IA | Separar modalidade estática, computação comum e elegibilidade ZeroGPU                                   | [Hugging Face](https://huggingface.co/docs/hub/en/spaces-overview)                            |
| Proteção do orçamento       | Diferenciar orçamento apenas com alertas de bloqueio de gasto realmente configurado e suportado         | [Google Cloud Billing](https://docs.cloud.google.com/billing/docs/how-to/budgets)             |

**O que foi efetivamente revisado:** leitura integral da versão 1.1, pesquisa nas fontes dos fornecedores/mantenedores, conferência de condições sensíveis de hospedagem e acréscimo de recursos por necessidade. As cotas indicadas são as publicadas na consulta; prevalecem o contrato e a configuração da conta utilizada.

**Limite desta revisão:** não houve instalação de todas as bibliotecas, provisionamento das nuvens, teste das contas da equipe nem auditoria jurídica de cada dependência transitiva. O levantamento cobre famílias de desafios, mas não equivale à validação integral de cada enunciado de 2026: parte das páginas oficiais não pôde ser recuperada durante a consulta. A escolha final precisará conferir o desafio específico, seus dados e entregáveis.

### Mapa de cobertura da maleta

| Necessidade                                         | Onde procurar            |
| --------------------------------------------------- | ------------------------ |
| Dados NASA, fontes públicas e pesquisa              | Seções 1, 12 e 13        |
| Programação, notebooks e controle de versões        | Seções 2 e 12            |
| Matemática, estatística, otimização e incerteza     | Seções 3 e 14            |
| Mapas, satélites, radar e formatos geográficos      | Seções 4, 12, 13 e 18    |
| Gráficos, dashboards e relatórios                   | Seções 5 e 19            |
| Frontend, backend, APIs, banco, login e arquivos    | Seções 6, 11 e 18        |
| Hospedagem, VPS, containers e custo                 | Seção 11                 |
| IA de pesquisa, programação, imagem e áudio         | Seções 7, 8 e 15         |
| Jogos, 3D, física, astronomia e sensores            | Seções 9 e 13            |
| Aplicativos móveis, interface e uso offline         | Seção 16                 |
| Sonificação, narrativa visual e material do pitch   | Seções 8 e 17            |
| Automação, e-mails, cache e processamento periódico | Seção 18                 |
| Testes, acessibilidade, segurança e reprodução      | Seções 10 e 19           |
| Escolha da arquitetura e plano B                    | Seções 20 e 21           |
| Licenças, fontes, atribuição e entrega              | Seção 19 e blocos finais |

## Como ler esta maleta

- **Livre** = código aberto (licença de software; pode ser MIT, Apache, GPL, BSD etc.). **Grátis** = pode ser usado sem pagar em certas condições; não significa código aberto.
- **Free limitado** = créditos, cotas, modelo ou recursos podem variar. **Serviço/API** = condições e preço próprios, mesmo quando a biblioteca de integração é aberta.
- **Dado aberto** não significa livre de atribuição; nem garante que os serviços para acessar o dado sejam ilimitados.
- Links apontam para documentação, repositórios dos mantenedores ou páginas dos fornecedores. **Licenças e planos podem mudar**: confirmar a versão do pacote e as condições da conta antes da adoção.
- **Local não significa custo zero absoluto:** pode exigir computador, memória, GPU, energia ou servidor. **Plano gratuito não é teste promocional**, e **crédito não é infraestrutura ilimitada**.
- **Prioridade de escolha:** primeiro uma solução simples que a equipe conhece; depois serviço com plano gratuito adequado; por último crédito temporário, faturamento habilitado ou infraestrutura de administração complexa.
- **Atenção ao hackathon:** preferir opções que possam ser reproduzidas por juízes sem logins privados, segredos expostos, custos ou equipamentos especiais.

## Escolha rápida: maleta essencial

| Necessidade                            | Primeira opção                                                             | Alternativa                                                                |
| -------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Planejar arquitetura e tirar dúvidas   | ChatGPT (free)                                                             | Gemini / Claude                                                            |
| Programar                              | Python + VS Code + GitHub                                                  | JavaScript/TypeScript + VS Code                                            |
| Criar dashboard em poucas horas        | Streamlit + Plotly                                                         | Gradio / React + ECharts                                                   |
| Publicar site grátis                   | Cloudflare Pages / Vercel Hobby                                            | GitHub Pages / Netlify                                                     |
| Guardar dados e login facilmente       | Supabase Free, com RLS e fluxo de e-mail testados                          | Firebase, separando os produtos; Neon para PostgreSQL gerenciado           |
| Hospedar API Python                    | Render Free, aceitando suspensão e limites                                 | Execução local; Railway/Cloud Run apenas após conferir créditos e cobrança |
| Precisar de VPS real                   | Oracle Always Free, somente se cadastro e capacidade estiverem confirmados | VPS paga com orçamento; não tornar o cadastro uma dependência do evento    |
| Tratar CSV, Excel e séries científicas | pandas + NumPy                                                             | Polars + DuckDB                                                            |
| Fazer previsão tabular                 | scikit-learn                                                               | XGBoost / LightGBM                                                         |
| Processar imagens de satélite          | QGIS + Rasterio + xarray                                                   | Google Earth Engine (sujeito à elegibilidade)                              |
| Mapas interativos                      | Leaflet + OpenStreetMap                                                    | MapLibre / Folium                                                          |
| Globo terrestre e espaço 3D            | CesiumJS                                                                   | Three.js                                                                   |
| Criar API                              | FastAPI                                                                    | Flask                                                                      |
| Guardar dados do protótipo             | SQLite ou DuckDB                                                           | Supabase Free                                                              |
| Hospedar demo simples                  | GitHub Pages (estática)                                                    | Cloudflare Pages / Streamlit Community Cloud                               |
| Fazer protótipo visual                 | Figma Starter                                                              | Penpot                                                                     |
| Slides e material gráfico              | Canva Free                                                                 | LibreOffice Impress / Google Slides                                        |
| Gerar imagens explicativas             | ChatGPT Images (limitado)                                                  | Gemini Nano Banana no app (limites)                                        |
| Registrar vídeo demonstrativo          | OBS + Kdenlive                                                             | Shotcut                                                                    |
| Reunir dados oficiais                  | NASA Earthdata + NASA APIs                                                 | Copernicus / NOAA / INPE                                                   |
| Traduzir/revisar entrega em inglês     | DeepL / LanguageTool                                                       | ChatGPT / Gemini com revisão humana                                        |

## Como decidir após escolher o desafio

1. **Problema e entregável:** site, painel, modelo científico, jogo, mapa, visualização, hardware ou conteúdo educacional?
2. **Dado científico:** qual conjunto NASA responde à pergunta? Validar formato, disponibilidade, atualização, área, escala e licença.
3. **MVP de 48 horas:** escolher até **um frontend, um backend, um banco e uma ferramenta de análise** (ou menos).
4. **Demonstração offline:** manter CSV/GeoJSON e capturas de tela locais caso a rede ou API falhe.
5. **Teste de licenças/custos:** confirmar direitos de uso, atribuição, download e acesso dos avaliadores.
6. **Evidência:** métricas reais, limitações, método, fontes, README e vídeo curto.

---

## 1. Pesquisa científica, dados espaciais e fontes oficiais

| Ferramenta                   | Para que serve no projeto                                   | Custo / licença / cuidado                | Link                                                                            |
| ---------------------------- | ----------------------------------------------------------- | ---------------------------------------- | ------------------------------------------------------------------------------- |
| **NASA Earthdata Search**    | Descobrir e baixar observações da Terra (MODIS, VIIRS etc.) | Grátis; cadastro eventualmente exigido   | [Site oficial](https://search.earthdata.nasa.gov/)                              |
| **NASA Earthdata CMR API**   | Pesquisar coleções e granules via API                       | Grátis; autenticação conforme recurso    | [Site oficial](https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html) |
| **NASA Worldview**           | Explorar imagens de satélite por data e camadas             | Grátis                                   | [Site oficial](https://worldview.earthdata.nasa.gov/)                           |
| **NASA GIBS**                | Servir camadas globais de imagens de satélite               | Grátis; políticas de uso                 | [Site oficial](https://www.earthdata.nasa.gov/data/tools/gibs)                  |
| **NASA FIRMS**               | Identificar focos de calor e incêndios                      | Grátis; API pode exigir chave            | [Site oficial](https://firms.modaps.eosdis.nasa.gov/)                           |
| **NASA POWER**               | Meteorologia, radiação solar e séries temporais             | Grátis                                   | [Site oficial](https://power.larc.nasa.gov/)                                    |
| **NASA Open APIs**           | APOD, asteroides e outras APIs em manutenção                | Grátis; verificar endpoints ativos       | [Site oficial](https://api.nasa.gov/)                                           |
| **NASA NEO / JPL SBDB**      | Pesquisar asteroides e objetos próximos                     | Grátis                                   | [Site oficial](https://ssd-api.jpl.nasa.gov/)                                   |
| **NASA Exoplanet Archive**   | Dados de exoplanetas e estrelas                             | Grátis                                   | [Site oficial](https://exoplanetarchive.ipac.caltech.edu/)                      |
| **NASA PDS**                 | Dados de missões e superfícies planetárias                  | Grátis                                   | [Site oficial](https://pds.nasa.gov/)                                           |
| **NASA Horizons**            | Efemérides e posições de corpos celestes                    | Grátis                                   | [Site oficial](https://ssd.jpl.nasa.gov/horizons/)                              |
| **NASA ADS**                 | Buscar literatura astronômica                               | Grátis para pesquisa                     | [Site oficial](https://ui.adsabs.harvard.edu/)                                  |
| **NASA 3D Resources**        | Modelos tridimensionais de conteúdo espacial                | Grátis; checar direitos de cada item     | [Site oficial](https://nasa3d.arc.nasa.gov/)                                    |
| **Copernicus Data Space**    | Imagens Sentinel e APIs STAC/openEO                         | Grátis com cotas e contas                | [Site oficial](https://dataspace.copernicus.eu/)                                |
| **USGS EarthExplorer**       | Landsat, elevação e geociências                             | Grátis; cadastro                         | [Site oficial](https://earthexplorer.usgs.gov/)                                 |
| **NOAA Climate Data Online** | Dados históricos climáticos                                 | Grátis; chave conforme API               | [Site oficial](https://www.ncei.noaa.gov/cdo-web/)                              |
| **Open-Meteo**               | Previsão, histórico, qualidade do ar e elevação             | Grátis para uso não comercial; CC BY 4.0 | [Site oficial](https://open-meteo.com/)                                         |
| **INPE / TerraBrasilis**     | Dados brasileiros sobre desmatamento e queimadas            | Acesso público; verificar licenças       | [Site oficial](https://terrabrasilis.dpi.inpe.br/)                              |
| **IBGE APIs**                | Indicadores territoriais e socioeconômicos brasileiros      | Grátis; citar IBGE                       | [Site oficial](https://servicodados.ibge.gov.br/api/docs/)                      |
| **Our World in Data**        | Séries históricas e indicadores globais                     | Grátis; conferir licença por conjunto    | [Site oficial](https://ourworldindata.org/)                                     |
| **Zenodo**                   | Arquivar e citar datasets e versões de projeto              | Grátis; selecionar licença               | [Site oficial](https://zenodo.org/)                                             |
| **Google Dataset Search**    | Descobrir conjuntos de dados                                | Grátis; cada dado tem licença própria    | [Site oficial](https://datasetsearch.research.google.com/)                      |

## 2. Programação, editores e versionamento

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **Python** | Análise de dados, IA, automação e APIs | Livre / PSF | [Site oficial](https://www.python.org/) |
| **JavaScript / TypeScript** | Interfaces web e aplicações interativas | Linguagens gratuitas; ferramentas variam | [Site oficial](https://www.typescriptlang.org/) |
| **R** | Estatística e visualização de dados | Livre / GPL | [Site oficial](https://www.r-project.org/) |
| **Julia** | Cálculo numérico e simulações científicas | Livre / MIT | [Site oficial](https://julialang.org/) |
| **SQL / SQLite** | Consultas e base local leve | Grátis; SQLite domínio público | [Site oficial](https://www.sqlite.org/) |
| **Visual Studio Code** | Editar código, depurar e instalar extensões | Grátis; distribuição Microsoft e componentes com termos próprios | [Site oficial](https://code.visualstudio.com/) |
| **VSCodium** | Editor derivado do VS Code sem marca da Microsoft | Livre / MIT | [Site oficial](https://vscodium.com/) |
| **JupyterLab** | Notebooks reprodutíveis para ciência | Livre / BSD | [Site oficial](https://jupyter.org/) |
| **Google Colab** | Rodar notebooks Python no navegador | Grátis com GPU/TPU limitadas e sessões temporárias | [Site oficial](https://colab.research.google.com/) |
| **Kaggle Notebooks** | Experimentos Python com aceleradores | Grátis com cotas e filas | [Site oficial](https://www.kaggle.com/code) |
| **Git** | Controlar versões e voltar a estados anteriores | Livre / GPL | [Site oficial](https://git-scm.com/) |
| **GitHub** | Repositório, issues, PR, colaboração | Plano gratuito; atenção a segredo e visibilidade | [Site oficial](https://github.com/) |
| **GitLab** | Repositórios e CI/CD | Free limitado / opções self-hosted | [Site oficial](https://gitlab.com/) |
| **Docker** | Padronizar ambientes e dependências | Engine open source; Docker Desktop tem condições próprias | [Site oficial](https://www.docker.com/) |
| **Postman** | Testar endpoints de APIs | Plano gratuito limitado | [Site oficial](https://www.postman.com/) |
| **Bruno** | Testar APIs com coleções armazenadas em Git | Código aberto; funcionalidades comerciais podem variar | [Site oficial](https://www.usebruno.com/) |
| **Insomnia** | Testar APIs REST e GraphQL | Plano gratuito e recursos pagos | [Site oficial](https://insomnia.rest/) |

## 3. Matemática, estatística, otimização e ciência de dados

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **NumPy** | Vetores, matrizes e cálculo numérico | Livre / BSD | [Site oficial](https://numpy.org/) |
| **pandas** | Limpar, juntar e analisar tabelas CSV/Excel | Livre / BSD | [Site oficial](https://pandas.pydata.org/) |
| **Polars** | Processar tabelas grandes com alta velocidade | Livre / MIT | [Site oficial](https://pola.rs/) |
| **SciPy** | Otimização, integração e estatística | Livre / BSD | [Site oficial](https://scipy.org/) |
| **SymPy** | Álgebra simbólica e equações | Livre / BSD | [Site oficial](https://www.sympy.org/) |
| **statsmodels** | Regressões, séries temporais e testes estatísticos | Livre / BSD | [Site oficial](https://www.statsmodels.org/) |
| **scikit-learn** | Classificação, regressão e clustering | Livre / BSD | [Site oficial](https://scikit-learn.org/) |
| **XGBoost** | Modelos de previsão tabular | Livre / Apache 2.0 | [Site oficial](https://xgboost.readthedocs.io/) |
| **LightGBM** | Previsão rápida sobre grandes tabelas | Livre / MIT | [Site oficial](https://lightgbm.readthedocs.io/) |
| **PyTorch** | Redes neurais e visão computacional | Livre; ver licença do pacote/modelo | [Site oficial](https://pytorch.org/) |
| **TensorFlow** | Aprendizado de máquina e redes neurais | Livre / Apache 2.0 | [Site oficial](https://www.tensorflow.org/) |
| **OpenCV** | Processamento de imagens e vídeos | Livre / Apache 2.0 | [Site oficial](https://opencv.org/) |
| **OR-Tools** | Rotas, alocação, otimização combinatória | Livre / Apache 2.0 | [Site oficial](https://developers.google.com/optimization) |
| **PuLP** | Otimização linear e inteira em Python | Livre / MIT | [Site oficial](https://coin-or.github.io/pulp/) |
| **NetworkX** | Grafos, caminhos e redes | Livre / BSD | [Site oficial](https://networkx.org/) |
| **SimPy** | Simulação de eventos discretos | Livre / MIT | [Site oficial](https://simpy.readthedocs.io/) |
| **GNU Octave** | Cálculo matricial similar a MATLAB | Livre / GPL | [Site oficial](https://octave.org/) |
| **GeoGebra** | Gráficos matemáticos e geometria | Uso básico gratuito; licenças variam | [Site oficial](https://www.geogebra.org/) |

## 4. Mapas, geoprocessamento e sensoriamento remoto

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **QGIS** | Analisar camadas geográficas e produzir mapas | Livre / GPL | [Site oficial](https://qgis.org/) |
| **GeoPandas** | Cruzar tabelas com geometrias | Livre / BSD | [Site oficial](https://geopandas.org/) |
| **Rasterio** | Tratar imagens raster georreferenciadas | Livre / BSD | [Site oficial](https://rasterio.readthedocs.io/) |
| **xarray** | Tratar dados multidimensionais de clima e satélite | Livre / Apache 2.0 | [Site oficial](https://docs.xarray.dev/) |
| **rioxarray** | Operações geográficas sobre xarray | Livre / Apache 2.0 | [Site oficial](https://corteva.github.io/rioxarray/) |
| **GDAL** | Converter formatos e processar raster/vetores | Livre / licença estilo MIT | [Site oficial](https://gdal.org/) |
| **Folium** | Gerar mapas interativos em Python | Livre / MIT | [Site oficial](https://python-visualization.github.io/folium/) |
| **Leaflet** | Mapa interativo leve para web | Livre / BSD-2-Clause | [Site oficial](https://leafletjs.com/) |
| **MapLibre GL JS** | Mapas vetoriais modernos e 3D parcial | Livre / BSD-3-Clause | [Site oficial](https://maplibre.org/) |
| **OpenStreetMap** | Dados abertos de vias, cidades e pontos | Dados ODbL: atribuição e políticas de tiles | [Site oficial](https://www.openstreetmap.org/copyright) |
| **CesiumJS** | Globo 3D, terreno e visualizações espaciais | Código Apache 2.0; serviços de tiles podem ter cotas | [Site oficial](https://cesium.com/platform/cesiumjs/) |
| **Google Earth Engine** | Analisar grandes séries de satélite na nuvem | Uso não comercial elegível com cotas e registro | [Site oficial](https://earthengine.google.com/) |
| **Kepler.gl** | Visualização rápida de grandes volumes geográficos | Código aberto; conferir dependências e mapas base | [Site oficial](https://kepler.gl/) |
| **deck.gl** | Visualização geoespacial de alto desempenho | Livre / MIT | [Site oficial](https://deck.gl/) |
| **Turf.js** | Operações GIS no navegador | Livre / MIT | [Site oficial](https://turfjs.org/) |
| **SRTM / Copernicus DEM** | Modelar relevo e elevação | Dados com termos específicos | [Site oficial](https://dataspace.copernicus.eu/) |

## 5. Gráficos, dashboards e visualização

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **Matplotlib** | Gráficos científicos e imagens de análises | Livre / licença própria compatível | [Site oficial](https://matplotlib.org/) |
| **Seaborn** | Gráficos estatísticos rápidos | Livre / BSD | [Site oficial](https://seaborn.pydata.org/) |
| **Plotly** | Gráficos interativos 2D/3D | Plotly.py livre / MIT; serviços extras pagos | [Site oficial](https://plotly.com/python/) |
| **Altair** | Gráficos declarativos e exploração de dados | Livre / BSD | [Site oficial](https://altair-viz.github.io/) |
| **D3.js** | Infográficos customizados interativos | Livre / ISC | [Site oficial](https://d3js.org/) |
| **Apache ECharts** | Dashboards e séries temporais sofisticados | Livre / Apache 2.0 | [Site oficial](https://echarts.apache.org/) |
| **Chart.js** | Gráficos simples no navegador | Livre / MIT | [Site oficial](https://www.chartjs.org/) |
| **Recharts** | Gráficos para React | Livre / MIT | [Site oficial](https://recharts.org/) |
| **Streamlit** | Criar painel de dados rapidamente com Python | Livre / Apache 2.0; hospedagem depende do serviço | [Site oficial](https://streamlit.io/) |
| **Gradio** | Interfaces de demonstração para modelos de IA | Livre / Apache 2.0 | [Site oficial](https://www.gradio.app/) |
| **Observable Framework** | Relatórios de dados interativos publicados como site | Livre / ISC | [Site oficial](https://observablehq.com/framework/) |
| **Grafana OSS** | Monitoramento de séries temporais | Livre / AGPLv3 | [Site oficial](https://grafana.com/oss/grafana/) |
| **Metabase** | Dashboards com consultas sobre bancos de dados | Open source em implantação própria; nuvem paga | [Site oficial](https://www.metabase.com/) |

## 6. Aplicativos, sites, APIs e banco de dados

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **React** | Interfaces e aplicativos web | Livre / MIT | [Site oficial](https://react.dev/) |
| **Next.js** | Sites React e rotas de servidor | Livre / MIT; hospedagem pode ter custo | [Site oficial](https://nextjs.org/) |
| **Vite** | Iniciar frontend rápido | Livre / MIT | [Site oficial](https://vite.dev/) |
| **Tailwind CSS** | Estilizar sites com classes utilitárias | Livre / MIT | [Site oficial](https://tailwindcss.com/) |
| **FastAPI** | Criar API Python com documentação automática | Livre / MIT | [Site oficial](https://fastapi.tiangolo.com/) |
| **Flask** | Criar serviços web simples em Python | Livre / BSD | [Site oficial](https://flask.palletsprojects.com/) |
| **Django** | Backend mais completo com administração | Livre / BSD | [Site oficial](https://www.djangoproject.com/) |
| **Node.js** | Servidor JavaScript | Livre / MIT | [Site oficial](https://nodejs.org/) |
| **PostgreSQL** | Banco relacional robusto | Livre / PostgreSQL License | [Site oficial](https://www.postgresql.org/) |
| **DuckDB** | Consultas analíticas locais a CSV/Parquet | Livre / MIT | [Site oficial](https://duckdb.org/) |
| **Supabase** | Postgres gerenciado, autenticação e armazenamento | Free com cotas; projetos podem pausar por inatividade | [Site oficial](https://supabase.com/pricing) |
| **Firebase** | Autenticação e banco de dados gerenciados | Plano Spark gratuito com cotas; cobrança em outros usos | [Site oficial](https://firebase.google.com/pricing) |
| **GitHub Pages** | Publicar site estático e documentação | Grátis nos casos elegíveis; não executa backend | [Site oficial](https://pages.github.com/) |
| **Cloudflare Pages** | Publicar frontend e funções leves | Free com cotas e termos próprios | [Site oficial](https://pages.cloudflare.com/) |
| **Vercel** | Publicar aplicações frontend e Next.js | Hobby gratuito para projetos pessoais/não comerciais; limites | [Site oficial](https://vercel.com/docs/plans/hobby) |
| **Netlify** | Hospedagem de sites e funções | Free com limites; verificar políticas | [Site oficial](https://www.netlify.com/pricing/) |
| **Streamlit Community Cloud** | Hospedar painel público de Streamlit | Grátis com limites e políticas | [Site oficial](https://streamlit.io/cloud) |
| **Hugging Face Spaces** | Hospedar demos estáticas e de modelos | Gratuidade depende da modalidade e elegibilidade; ver distinção entre Static, Gradio/Docker e ZeroGPU na seção 11.2 | [Site oficial](https://huggingface.co/docs/hub/en/spaces-overview) |
| **Render** | Hospedar backend; experimentar banco | Plano gratuito com limitações diferentes por produto. O Postgres gratuito é temporário; ver seção 11 | [Documentação oficial](https://render.com/docs/free) |

## 7. IA para pesquisa, programação e agentes

| Ferramenta                | Para que serve no projeto                                   | Custo / licença / cuidado                                  | Link                                                      |
| ------------------------- | ----------------------------------------------------------- | ---------------------------------------------------------- | --------------------------------------------------------- |
| **ChatGPT**               | Ideação, pesquisa, revisão de código, documentação e testes | Plano gratuito com limites; API cobrada à parte            | [Site oficial](https://chatgpt.com/)                      |
| **Claude**                | Raciocínio, escrita e revisão de código                     | Plano gratuito com limites; API à parte                    | [Site oficial](https://claude.ai/)                        |
| **Google Gemini**         | Análise multimodal e suporte a programação                  | Acesso gratuito com limites; API depende do modelo         | [Site oficial](https://gemini.google.com/)                |
| **Google AI Studio**      | Prototipar prompts multimodais e integrar Gemini API        | Free tier em modelos elegíveis e cotas; atenção à cobrança | [Site oficial](https://aistudio.google.com/)              |
| **GitHub Copilot Free**   | Autocompletar e explicar código no editor                   | Grátis com cota mensal                                     | [Site oficial](https://github.com/features/copilot/plans) |
| **Google Colab AI**       | Assistência em notebooks e código                           | Disponibilidade/limites conforme conta                     | [Site oficial](https://colab.research.google.com/)        |
| **Perplexity**            | Pesquisar com links para fontes                             | Grátis limitado; conferir documentos originais             | [Site oficial](https://www.perplexity.ai/)                |
| **NotebookLM**            | Estudar PDFs, manuais e documentos com fontes               | Plano gratuito com cotas                                   | [Site oficial](https://notebooklm.google.com/)            |
| **Ollama**                | Executar modelos de IA localmente                           | Ferramenta local gratuita; licença depende do modelo       | [Site oficial](https://ollama.com/)                       |
| **LM Studio**             | Executar modelos locais por interface visual                | Uso gratuito local; observar termos                        | [Site oficial](https://lmstudio.ai/)                      |
| **Hugging Face Hub**      | Descobrir modelos/datasets e licenças                       | Catálogo gratuito; modelos podem ser restritos             | [Site oficial](https://huggingface.co/)                   |
| **Transformers**          | Aplicar modelos de linguagem, imagem e áudio                | Biblioteca livre / Apache 2.0; pesos variam                | [Site oficial](https://huggingface.co/docs/transformers)  |
| **sentence-transformers** | Busca semântica, embeddings e classificação                 | Biblioteca livre; licença dos modelos varia                | [Site oficial](https://sbert.net/)                        |
| **LangChain**             | Orquestrar fluxos com LLMs e ferramentas                    | Bibliotecas livres; modelos/APIs custam à parte            | [Site oficial](https://www.langchain.com/)                |
| **LlamaIndex**            | Consultar arquivos e construir RAG                          | Núcleo open source; provedores podem cobrar                | [Site oficial](https://www.llamaindex.ai/)                |
| **RAG local com FAISS**   | Pesquisar documentos por similaridade                       | FAISS livre / MIT; modelos variam                          | [Site oficial](https://github.com/facebookresearch/faiss) |

## 8. IA visual, áudio, vídeo e conteúdo

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **Nano Banana / Gemini Image** | Gerar imagens conceituais e elementos de apresentação | Acesso no app conforme conta; uso via API pode ser pago | [Site oficial](https://ai.google.dev/gemini-api/docs/image-generation) |
| **ChatGPT Images** | Gerar e editar ilustrações e imagens | Plano gratuito limitado | [Site oficial](https://chatgpt.com/) |
| **Canva AI** | Criar slides, gráficos, peças e materiais visuais | Grátis com cota; elementos premium restritos | [Site oficial](https://www.canva.com/pricing/) |
| **Figma AI / Figma Make** | Ideação e prototipação de interfaces | Starter com créditos limitados | [Site oficial](https://www.figma.com/pricing/) |
| **Adobe Firefly** | Gerar visuais e recursos de composição | Créditos gratuitos limitados; planos pagos | [Site oficial](https://firefly.adobe.com/) |
| **Stable Diffusion (modelos)** | Geração/edição local de imagens | Executável local em condições próprias; licença de cada peso varia | [Site oficial](https://huggingface.co/models?pipeline_tag=text-to-image) |
| **ComfyUI** | Montar fluxos visuais para geração de imagens | Software open source; modelos podem restringir uso | [Site oficial](https://www.comfy.org/) |
| **Whisper** | Transcrever narração e reuniões | Código e pesos com permissões próprias; execução local | [Site oficial](https://github.com/openai/whisper) |
| **Audacity** | Gravar, limpar e editar áudio | Livre / GPL | [Site oficial](https://www.audacityteam.org/) |
| **OBS Studio** | Gravar demonstração e tela do projeto | Livre / GPL | [Site oficial](https://obsproject.com/) |
| **Kdenlive** | Editar vídeo e legendas | Livre / GPL | [Site oficial](https://kdenlive.org/) |
| **Shotcut** | Editar vídeos para pitch | Livre / GPL | [Site oficial](https://shotcut.org/) |
| **Blender** | Modelar, animar e renderizar 3D | Livre / GPL; arte criada tem regime distinto | [Site oficial](https://www.blender.org/) |
| **Inkscape** | Criar ícones, diagramas e SVG | Livre / GPL | [Site oficial](https://inkscape.org/) |
| **GIMP** | Editar e tratar imagens | Livre / GPL | [Site oficial](https://www.gimp.org/) |
| **Krita** | Desenhos e ilustrações digitais | Livre / GPL | [Site oficial](https://krita.org/) |
| **Penpot** | Design de telas colaborativo open source | Plano gratuito e opção self-hosted | [Site oficial](https://penpot.app/) |
| **Excalidraw** | Esboçar fluxos e arquiteturas | Editor aberto e colaboração básica em tempo real gratuitos; Excalidraw+ é separado | [Fonte oficial](https://github.com/excalidraw/excalidraw) |
| **diagrams.net** | Desenhar arquitetura e fluxogramas | Grátis | [Site oficial](https://www.diagrams.net/) |
| **Screencast / Loom** | Gravar pitch de tela e explicação | Planos gratuitos com limites | [Site oficial](https://www.loom.com/) |
| **LibreOffice Impress** | Criar slides offline | Livre / MPL 2.0 | [Site oficial](https://www.libreoffice.org/) |
| **Google Slides** | Slides colaborativos | Grátis em conta pessoal; termos de serviço | [Site oficial](https://slides.google.com/) |

## 9. 3D, física, astronomia, simulação e educação

| Ferramenta | Para que serve no projeto | Custo / licença / cuidado | Link |
|---|---|---|---|
| **Three.js** | Modelos 3D no navegador | Livre / MIT | [Site oficial](https://threejs.org/) |
| **Babylon.js** | Cenas 3D e visualização interativa | Livre / Apache 2.0 | [Site oficial](https://www.babylonjs.com/) |
| **Godot Engine** | Protótipos imersivos e jogos educativos | Livre / MIT | [Site oficial](https://godotengine.org/) |
| **Stellarium** | Simular céu, estrelas e planetas | Livre / GPL | [Site oficial](https://stellarium.org/) |
| **Skyfield** | Posições astronômicas em Python | Livre / MIT | [Site oficial](https://rhodesmill.org/skyfield/) |
| **Astropy** | Unidades, coordenadas e tabelas astronômicas | Livre / BSD | [Site oficial](https://www.astropy.org/) |
| **poliastro — legado** | Consultar exemplos antigos de mecânica orbital | MIT; repositório arquivado em 14/10/2023. Não é primeira escolha para projeto novo; avaliar Orekit, Skyfield ou SpiceyPy conforme a tarefa, sem presumir equivalência | [Repositório oficial](https://github.com/poliastro/poliastro) |
| **Orekit** | Dinâmica de voo espacial | Livre / Apache 2.0 | [Site oficial](https://www.orekit.org/) |
| **GMAT (NASA)** | Modelar trajetórias e missões espaciais | Software gratuito; conferir termos próprios | [Site oficial](https://software.nasa.gov/software/GSC-17177-1) |
| **OpenRocket** | Simular foguetes amadores para educação | Livre / GPL | [Site oficial](https://openrocket.info/) |
| **FreeCAD** | Modelagem CAD e protótipos mecânicos | Livre / LGPL | [Site oficial](https://www.freecad.org/) |
| **Tinkercad** | CAD 3D simples para principiantes | Gratuito com conta | [Site oficial](https://www.tinkercad.com/) |
| **Arduino IDE** | Programar sensores e microcontroladores | Software open source; hardware pode custar | [Site oficial](https://www.arduino.cc/en/software) |
| **Wokwi** | Simular Arduino, ESP32 e sensores | Plano gratuito limitado | [Site oficial](https://wokwi.com/) |
| **PhET** | Simulações interativas para ensino | Grátis; conferir licença de cada componente | [Site oficial](https://phet.colorado.edu/) |

## 10. Testes, acessibilidade, qualidade e equipe

| Ferramenta                   | Para que serve no projeto                | Custo / licença / cuidado                   | Link                                                                  |
| ---------------------------- | ---------------------------------------- | ------------------------------------------- | --------------------------------------------------------------------- |
| **pytest**                   | Testar rotinas Python                    | Livre / MIT                                 | [Site oficial](https://pytest.org/)                                   |
| **Playwright**               | Testar automaticamente interfaces web    | Livre / Apache 2.0                          | [Site oficial](https://playwright.dev/)                               |
| **Lighthouse**               | Auditar performance e acessibilidade web | Livre / Apache 2.0                          | [Site oficial](https://developer.chrome.com/docs/lighthouse/overview) |
| **axe-core**                 | Auditar acessibilidade de páginas        | Livre / MPL 2.0                             | [Site oficial](https://github.com/dequelabs/axe-core)                 |
| **Ruff**                     | Revisar e formatar código Python         | Livre / MIT                                 | [Site oficial](https://docs.astral.sh/ruff/)                          |
| **Prettier**                 | Padronizar formatação do JavaScript      | Livre / MIT                                 | [Site oficial](https://prettier.io/)                                  |
| **ESLint**                   | Identificar problemas em JavaScript      | Livre / MIT                                 | [Site oficial](https://eslint.org/)                                   |
| **Sentry**                   | Monitorar falhas em aplicativo           | Free limitado; SDKs open source             | [Site oficial](https://sentry.io/pricing/)                            |
| **Trello**                   | Quadro de tarefas e responsáveis         | Plano gratuito limitado                     | [Site oficial](https://trello.com/)                                   |
| **Notion**                   | Documentação e gestão de tarefas         | Plano gratuito com limites                  | [Site oficial](https://www.notion.com/pricing)                        |
| **Google Drive**             | Compartilhar documentos e arquivos       | Grátis com espaço limitado                  | [Site oficial](https://drive.google.com/)                             |
| **Discord**                  | Comunicação e canais da equipe           | Grátis; extras pagos                        | [Site oficial](https://discord.com/)                                  |
| **GitHub Projects**          | Quadro kanban integrado ao repositório   | Free nos limites do GitHub                  | [Site oficial](https://github.com/features/issues)                    |
| **Zotero**                   | Organizar referências e bibliografia     | Livre; sincronização de arquivos tem cotas  | [Site oficial](https://www.zotero.org/)                               |
| **DeepL / Google Translate** | Revisar inglês de submissão e pitch      | Grátis com limites; revisar termos técnicos | [Site oficial](https://www.deepl.com/translator)                      |
| **LanguageTool**             | Revisar português e inglês               | Grátis limitado; opções open source         | [Site oficial](https://languagetool.org/)                             |

---

## 11. Infraestrutura, hospedagem, VPS, deploy, banco de dados e serviços de produção

> **Distinção essencial:** **Vercel não é uma VPS tradicional**: é uma plataforma gerenciada de hospedagem/deploy (frontend e funções). **VPS** fornece uma máquina virtual mais configurável, mas exige administrar servidor, atualizações e segurança. **Supabase** é um backend gerenciado que oferece PostgreSQL, autenticação, armazenamento e API. Para um hackathon de 48 horas, preferir plataformas gerenciadas se elas suportarem o protótipo.

**Legenda:** 🟢 plano grátis ou software livre; 🟡 grátis com limites, requisitos ou risco relevante; 🔵 pago/teste/créditos. Os limites são fotografia de **30/10/2026**; verificar novamente no cadastro. *Plano gratuito do serviço* não torna o software usado automaticamente open source.

### 11.1 Publicar sites e interfaces (frontend)

| Ferramenta           | Ideal para                                                                            | Custo e cuidado                                                                               | Site oficial                             |
| -------------------- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | ---------------------------------------- |
| **Vercel**           | Publicar Next.js, React e sites com deploy automático pelo GitHub; funções serverless | 🟢 Hobby US$ 0; **uso pessoal e não comercial**; limites de execução e funções. **Não é VPS** | https://vercel.com/pricing               |
| **Cloudflare Pages** | Sites estáticos, React/Vite, documentação e landing pages                             | 🟢 assets estáticos gratuitos; funções sujeitas à cota Workers; ótimo para demos              | https://developers.cloudflare.com/pages/ |
| **Netlify**          | Sites estáticos e frontend com deploy contínuo e formulários/funções                  | 🟡 plano gratuito e limites de recursos/créditos; conferir preços vigentes                    | https://www.netlify.com/pricing/         |
| **GitHub Pages**     | Site estático, documentação e protótipo sem servidor                                  | 🟢 gratuito para repositórios elegíveis; **não** executa backend Python ou Node persistente   | https://pages.github.com/                |
| **Firebase Hosting** | Site/app web com HTTPS e integração ao Firebase                                       | 🟡 uso sem custo sujeito a cotas; atenção ao App Hosting e recursos que exigem Blaze          | https://firebase.google.com/pricing      |
| **Surge**            | Publicação muito rápida de HTML/CSS/JS estáticos                                      | 🟢 opção básica gratuita; verificar limitações de domínio/recursos                            | https://surge.sh/                        |

### 11.2 Backends, APIs e aplicações Python

| Ferramenta | Ideal para | Custo e cuidado | Site oficial |
|---|---|---|---|
| **Render** | Hospedar FastAPI, Flask, Django, Node e sites | 🟡 web service Free adormece após 15 min sem tráfego; retorno pode levar ~1 min. Disco efêmero. **Postgres Free é outro produto e expira após 30 dias** | https://render.com/docs/free |
| **Railway** | Deploy rápido de API, Docker, serviços e bancos | 🟡 teste inicial de US$ 5 por até 30 dias; depois crédito Free de **US$ 1/mês** (verificar adequação) | https://docs.railway.com/pricing/free-trial |
| **Cloudflare Workers** | APIs leves, webhooks, edge functions e lógica de baixa latência | 🟢 Free: cota de requisições/dia; não substitui servidor Python tradicional | https://developers.cloudflare.com/workers/platform/pricing/ |
| **Google Cloud Run** | APIs em containers e workloads acionados por requisição | 🟡 pode caber nas cotas sem custo, mas requer atenção à conta de faturamento e outros serviços pagos | https://cloud.google.com/run/pricing |
| **PythonAnywhere** | Aplicações Python simples para testes | 🟡 contas free têm CPU, espaço e duração limitados; não ideal para serviço permanente | https://help.pythonanywhere.com/pages/FreeAccountsFeatures/ |
| **Streamlit Community Cloud** | Hospedar dashboards Streamlit sem configurar infraestrutura | 🟢 camada gratuita para apps comunitários; limites e suspensão de apps | https://streamlit.io/cloud |
| **Hugging Face Spaces** | Apresentar demos de IA e modelos interativos | 🟡 Static gratuito. Criar Gradio/Docker exige plano pago, com exceção de até **2 Gradio ZeroGPU** para contas pessoais gratuitas elegíveis. Confirmar acesso, filas e cotas na conta real | https://huggingface.co/docs/hub/en/spaces-overview |

### 11.3 Banco de dados acessível e armazenamento persistente

| Ferramenta | Tipo e aplicação ideal | Custo e limite prático | Site oficial |
|---|---|---|---|
| **Supabase** ⭐ | PostgreSQL + autenticação + arquivos + API; **melhor ponto de partida para app com usuários e dados** | 🟢 Free: **500 MB de banco**, **1 GB de arquivos**, **2 projetos ativos**, **50 mil usuários ativos/mês**; pausa após ~7 dias de pouca atividade | https://supabase.com/pricing |
| **Neon** ⭐ | PostgreSQL gerenciado; ideal quando precisa só de SQL e backend próprio | 🟢 Free: **1 GB por projeto**, computação e transferência limitadas; compute adormece quando ocioso | https://neon.com/pricing |
| **Firebase Firestore** | Banco NoSQL/documentos, tempo real, app web/mobile | 🟢 nível gratuito com **1 GiB**, 50 mil leituras/dia e 20 mil gravações/dia na edição Standard; autenticação/regras requerem configuração | https://firebase.google.com/pricing |
| **Turso** | Banco leve compatível com SQLite, sincronização e protótipos rápidos | 🟢 Free com cotas de armazenamento e operações; consultar preço atual por plano | https://turso.tech/pricing |
| **Cloudflare D1** | SQL/SQLite integrado a Workers/Pages | 🟡 limites free de tamanho e leituras/escritas; ótimo para API na Cloudflare | https://developers.cloudflare.com/d1/platform/pricing/ |
| **SQLite** | Arquivo de banco local, sem servidor; protótipo offline | 🟢 gratuito/public domain; **não armazenar arquivo SQLite no disco efêmero de Vercel/Render Free** | https://www.sqlite.org/ |
| **PostgreSQL** | Banco relacional robusto e espacial via PostGIS | 🟢 software open source; precisa de hospedagem ou computador | https://www.postgresql.org/ |
| **PocketBase** | Backend leve com SQLite, autenticação e painel de administração | 🟢 open source; requer hospedagem com disco persistente | https://pocketbase.io/ |
| **Appwrite** | Backend com auth, DB, storage e funções | 🟡 open source para self-hosting; cloud com plano/cotas próprias | https://appwrite.io/pricing |
| **MongoDB Atlas** | Documentos JSON e dados flexíveis | 🟡 cluster grátis sujeito a cotas e disponibilidade regional | https://www.mongodb.com/pricing |
| **DuckDB** | Consultas analíticas grandes em Parquet/CSV sem servidor | 🟢 gratuito e local; indicado para análises, não autenticação multiusuário | https://duckdb.org/ |

### 11.4 Arquivos, imagens, datasets e autenticação

| Ferramenta | Ideal para | Observação | Site oficial |
|---|---|---|---|
| **Supabase Storage** | Imagens, PDFs, arquivos CSV e datasets pequenos | Incluído nas cotas do Supabase; adotar política de acesso adequada | https://supabase.com/docs/guides/storage |
| **Cloudflare R2** | Armazenamento de objetos, arquivos e imagens | Camada gratuita com limites; conferir operações/armazenamento e faturamento | https://developers.cloudflare.com/r2/pricing/ |
| **Firebase Storage** | Imagens e arquivos de aplicações Firebase | **Exige Blaze e conta de faturamento**, conforme mudança em vigor desde 03/02/2026. Cotas sem custo não dispensam essa exigência; não confundir com Firestore no Spark | [Regra oficial](https://firebase.google.com/docs/storage/faqs-storage-changes-announced-sept-2024) |
| **GitHub Releases / Git LFS** | Distribuir versões ou arquivos do projeto | Não usar Git como banco de dados; LFS e banda têm limites | https://docs.github.com/ |
| **Supabase Auth** | Login por e-mail, senha e provedores externos | Configurar RLS e testar confirmação/recuperação. SMTP padrão não atende livremente usuários externos; ver seção 11.8 | https://supabase.com/docs/guides/auth/auth-smtp |
| **Firebase Authentication** | Login rápido de web e mobile | Provedores têm restrições/custos distintos; confirmar a modalidade | https://firebase.google.com/docs/auth |
| **Clerk** | Autenticação pronta com boa interface | Serviço proprietário; plano grátis limitado, validar termos | https://clerk.com/pricing |

### 11.5 VPS, containers, redes e operação

| Ferramenta | Ideal para | Custo e cautela | Site oficial |
|---|---|---|---|
| **Oracle Cloud Always Free** ⭐ | VPS real para Linux, API, banco e Docker | 🟡 recursos gratuitos com limites de CPU/RAM e disponibilidade regional; cadastro e cartão podem ser exigidos; **configuração técnica e segurança por conta da equipe** | https://www.oracle.com/br/cloud/free/ |
| **AWS EC2** | VPS Linux/Windows e infraestrutura completa | 🟡 elegibilidade free varia por tipo de conta/créditos; **risco de cobrança** fora das cotas | https://aws.amazon.com/free/ |
| **Google Compute Engine** | VPS gerenciável para workloads próprios | 🟡 nível gratuito limitado a regiões/tipos; cartão e faturamento podem ser exigidos | https://cloud.google.com/free |
| **Hetzner Cloud** | VPS Linux simples e de baixo custo | 🔵 pago; bom plano B se orçamento permitir | https://www.hetzner.com/cloud/ |
| **DigitalOcean Droplets** | VPS simples, tutoriais abundantes | 🔵 pago / créditos promocionais quando elegíveis | https://www.digitalocean.com/pricing/droplets |
| **Docker** | Empacotar API + dependências para reproduzir em qualquer servidor | 🟢 engine open source; avaliar termos do Docker Desktop conforme ambiente | https://docs.docker.com/ |
| **Docker Compose** | Subir API, banco e serviços locais em conjunto | 🟢 útil para validar stack antes de publicar | https://docs.docker.com/compose/ |
| **Coolify** | Painel de deploy self-hosted semelhante a PaaS | 🟢 software open source; **servidor VPS não é gratuito por consequência** | https://coolify.io/ |
| **Caddy** | HTTPS automático e proxy reverso em VPS | 🟢 open source; configuração simples | https://caddyserver.com/ |
| **Nginx** | Proxy reverso, cache e publicação em Linux | 🟢 open source; mais administração | https://nginx.org/ |
| **Uptime Kuma** | Monitorar se site/API estão disponíveis | 🟢 self-hosted; precisa de local para executar | https://github.com/louislam/uptime-kuma |
| **GitHub Actions** | Testes e deploy automático após commits | 🟡 gratuito dentro das cotas aplicáveis; não é um servidor always-on | https://docs.github.com/actions |
| **Sentry** | Registrar erros da aplicação em tempo real | 🟡 plano grátis com limites; avaliar dados enviados | https://sentry.io/pricing/ |

### 11.6 Guia rápido: qual infraestrutura usar?

| Se o projeto for... | Conjunto inicialmente recomendado | Complexidade |
|---|---|---|
| Site visual sem login e sem dados gravados | **Cloudflare Pages + GitHub** ou **Vercel Hobby + GitHub** | Muito baixa |
| Dashboard de dados da NASA | **Streamlit Community Cloud + pandas + Plotly** | Baixa |
| Site React com cadastro/login e registros | **Vercel + Supabase** ou **Cloudflare Pages + Supabase** | Baixa/média |
| API de ciência de dados em Python | **Render Free + Supabase/Neon** | Média; testar cold start |
| API JavaScript simples com banco SQL | **Cloudflare Workers + D1** | Média |
| Site com dados geográficos e arquivos | **Cloudflare Pages + Supabase/PostGIS + Supabase Storage ou R2** | Média |
| Simulação pesada, processamento contínuo, ferramentas Linux | **Oracle Cloud Always Free + Docker** (se conseguir provisionar); ou VPS paga | Alta |
| Protótipo offline, sem risco de internet | **Python + DuckDB/SQLite + dashboard local** e capturas/vídeo de demonstração | Baixa |

**Exemplo 1 — mapa de queimadas:** frontend React/Leaflet em Cloudflare Pages; dados NASA FIRMS processados com Python; Supabase para registros e histórico. **Exemplo 2 — quiz educacional:** Vercel para frontend, Supabase Auth/DB para perfis e resultados. **Exemplo 3 — previsão de chuvas:** Python/scikit-learn e Streamlit Community Cloud; para processamento mais pesado, separar treinamento offline e deploy apenas do modelo de inferência.

### 11.7 Checklist para não comprometer a demonstração

- [ ] Abrir o link público em janela anônima e em outro aparelho.
- [ ] Testar *cold start* do backend e entender se ele pode adormecer.
- [ ] Confirmar limites de requisição, banco, armazenamento, uploads e tráfego.
- [ ] Checar cartão/faturamento, cotas e bloqueio efetivo de consumo. Alerta de orçamento não equivale automaticamente a bloqueio de cobrança.
- [ ] Não expor senhas, tokens privados ou chaves secretas. Chaves publicáveis de cliente são uma categoria diferente e exigem políticas de acesso corretamente configuradas.
- [ ] Aplicar regras de acesso (RLS no Supabase) e não expor dados pessoais.
- [ ] Manter backup/exportação de dados, sobretudo se houver pausas ou expiração da camada gratuita.
- [ ] Validar compatibilidade entre licença do código e condições do provedor.
- [ ] Separar uso gratuito **para protótipos não comerciais** do eventual uso comercial posterior.
- [ ] Gravar vídeo e capturas da demo, mantendo plano B local se a internet cair.

**Fontes oficiais de cotas e termos (consulta de 30/10/2026):** [Vercel Hobby](https://vercel.com/docs/plans/hobby), [Supabase Free](https://supabase.com/pricing), [Supabase pausa](https://supabase.com/kb/faqs/platform/free-project-pausing), [Render Free](https://render.com/docs/free), [Railway Free Trial](https://docs.railway.com/pricing/free-trial), [Neon Free](https://neon.com/pricing), [Cloudflare Pages Functions](https://developers.cloudflare.com/pages/functions/pricing/), [Firebase](https://firebase.google.com/pricing), [Oracle Cloud Free](https://www.oracle.com/br/cloud/free/), [Turso](https://turso.tech/pricing), [Hugging Face Spaces](https://huggingface.co/docs/hub/spaces-overview).

### 11.8 Supabase na prática: banco, login e e-mail são decisões diferentes

Para um aplicativo com dados e usuários, Supabase continua sendo uma opção inicial conveniente, mas não basta criar o projeto e copiar a chave.

**E-mail:** o SMTP padrão é destinado a testes e restringe os destinatários aos membros autorizados da equipe do projeto, com limite publicado de **2 mensagens por hora**. Para confirmação de cadastro, recuperação de senha ou link mágico destinados ao público, configurar um provedor SMTP e testar entrega. A cota de usuários do Auth não é cota de e-mails. [Fonte: Supabase SMTP](https://supabase.com/docs/guides/auth/auth-smtp).

**Sugestão para a demonstração:** quando login não for parte do problema, oferecer uma área de consulta pública sem cadastro. Se for necessário autenticar, testar o fluxo escolhido com uma conta externa e verificar URLs de redirecionamento. Não remover proteções de um aplicativo público apenas para fazer a apresentação funcionar.

**Acesso aos dados:** chaves `publishable` destinam-se ao cliente; chaves `secret` e a antiga `service_role` ficam exclusivamente em componentes controlados pelo servidor. Usar permissões mínimas e RLS para definir o que cada usuário pode ler ou alterar. A antiga chave `anon` tem papel de cliente, não de segredo administrativo. [Fonte: Supabase API keys](https://supabase.com/docs/guides/getting-started/api-keys).

**Exemplo:** o visitante pode consultar indicadores ambientais públicos; somente o usuário autenticado pode alterar os próprios registros. Nunca conceder escrita irrestrita em todas as tabelas porque a página da demonstração precisa carregar.

### 11.9 Infraestrutura que não precisamos contratar automaticamente

| Recurso | Quando realmente faz falta | Caminho mais simples para o protótipo |
|---|---|---|
| Domínio próprio | Marca ou integração que o exija | Usar o subdomínio da hospedagem quando disponível; e-mail transacional pode exigir domínio verificado |
| VPS | Processo persistente, software específico ou necessidade de controle do sistema | Preferir hospedagem gerenciada ou cálculo local quando suficientes |
| Banco de dados | Dados mutáveis, vários usuários ou histórico que precise ser persistido | CSV, JSON ou Parquet versionado pode bastar para uma consulta demonstrativa |
| Login | Identidade, permissões ou informações privadas são essenciais | Área pública de leitura evita dependência de e-mail e senha |
| API própria | Segredos, processamento ou integração precisam ficar no servidor | Site estático com dados previamente tratados pode ser suficiente |
| GPU | Modelo escolhido exige aceleração para a tarefa e tamanho de entrada | Modelo menor, inferência em CPU ou resultados pré-calculados identificados |
| Fila de tarefas | Trabalho demorado precisa continuar fora da requisição web | Pré-processar um recorte do dado e apresentar o resultado de maneira transparente |
| Serviço pago de IA | IA em tempo de execução agrega valor demonstrável | Usar IA apenas como apoio à construção, ou modelo local compatível |

**Controle de gasto:** limites de banco, arquivos, tráfego, CPU, mensagens e IA são distintos. Um plano de US$ 0 pode exigir faturamento em determinado produto ou parar de funcionar quando a cota acabar. No Google Cloud, um orçamento configurado apenas para alertar **não bloqueia** gasto; recursos de *spend cap*, quando suportados, exigem configuração própria. [Documentação](https://docs.cloud.google.com/billing/docs/how-to/budgets).

**Regra de equipe sugerida:** ninguém habilita plano pago, recarga automática ou faturamento sem registrar responsável, limite aprovado e alternativa sem cobrança.

### 11.10 Vocabulário rápido para evitar escolhas erradas

**Frontend** é a interface; **backend** executa regras e integrações; **banco** guarda registros; **storage** guarda arquivos; **deploy** publica uma versão; **VPS** é um servidor virtual administrado pela equipe. **Serverless** não significa ausência de servidor nem execução ilimitada: o provedor administra a infraestrutura sob limites próprios. **Cold start** é a demora para um serviço inicialmente parado atender uma requisição.


---

## 12. Obter, ler, limpar e reproduzir os dados científicos

Um dado de satélite nem sempre chega em CSV. Esta seção cobre a passagem entre encontrar um conjunto e conseguir usá-lo corretamente. Começar com um recorte pequeno reduz risco de download, memória e processamento.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **earthaccess** | Buscar e baixar dados NASA Earthdata a partir de Python | Biblioteca aberta; pode exigir Earthdata Login. Credencial e token não devem entrar no repositório. | [Documentação / condições](https://earthaccess.readthedocs.io/en/stable/) |
| **PySTAC Client** | Pesquisar catálogos STAC por região, data e coleção | Código aberto; o acesso aos arquivos encontrados depende das condições do catálogo/provedor. | [Documentação / condições](https://pystac-client.readthedocs.io/en/stable/) |
| **h5py** | Ler arquivos HDF5 e selecionar partes de grandes matrizes | Aberto e local; conhecer grupos, atributos e unidades do produto. | [Documentação / condições](https://docs.h5py.org/en/stable/) |
| **netCDF4-Python** | Ler séries e grades científicas em NetCDF | Aberto e local; combina com xarray. Atenção a calendários, dimensões e valores ausentes. | [Documentação / condições](https://github.com/Unidata/netcdf4-python) |
| **Zarr-Python** | Organizar matrizes em blocos para leitura parcial e acesso em nuvem | Aberto; armazenamento remoto e operações podem ter custo. Validar compatibilidade de versão do formato. | [Documentação / condições](https://zarr.readthedocs.io/en/stable/) |
| **Apache Arrow / PyArrow** | Ler e gravar Parquet e trocar tabelas entre ferramentas | Aberto; útil para reduzir transferência de tabelas. Não substitui metadados científicos. | [Documentação / condições](https://arrow.apache.org/docs/python/) |
| **Dask** | Processar tabelas ou matrizes em partes e paralelizar tarefas | Aberto; não cria memória/CPU gratuitamente. Só adotar quando pandas/xarray simples não bastarem. | [Documentação / condições](https://www.dask.org/) |
| **OpenRefine** | Limpar nomes, categorias e inconsistências de tabelas visualmente | Gratuito e aberto, com execução local; guardar histórico das transformações. | [Documentação / condições](https://openrefine.org/) |
| **Pandera** | Testar colunas, tipos, intervalos e regras de qualidade em tabelas | Aberto, MIT; regras precisam refletir o significado dos dados. | [Documentação / condições](https://github.com/unionai-oss/pandera) |
| **uv** | Instalar dependências Python e reproduzir o ambiente com arquivo de trava | Aberto; registrar versão do Python e `uv.lock`. Não misturar gerenciadores sem necessidade. | [Documentação / condições](https://docs.astral.sh/uv/guides/projects/) |

### Que leitor escolher?

| O arquivo encontrado é… | Começar por… | Conferência essencial |
|---|---|---|
| CSV ou tabela pequena | pandas ou Polars | Separador, codificação, decimal, datas e identificadores com zeros iniciais |
| Parquet | DuckDB ou PyArrow | Tipos das colunas, partições e filtros |
| NetCDF | xarray com mecanismo de leitura compatível | Dimensões de tempo, nível, latitude/longitude, unidade e calendário |
| HDF5 | h5py; xarray quando o produto for compatível | Grupos e atributos; nem todo HDF5 é um NetCDF georreferenciado |
| GeoTIFF / COG | Rasterio ou QGIS | Sistema de coordenadas, resolução, NoData e escala |
| FITS | Astropy; Photutils para medições de fontes | Cabeçalho, calibração e coordenadas celestes |
| GeoJSON / GeoPackage | GeoPandas ou QGIS | Ordem das coordenadas, geometria válida e sistema de referência |
| Zarr | Zarr-Python / xarray | Versão, tamanho de blocos e custo de acesso remoto |

Fontes de formatos: [xarray — leitura e escrita](https://docs.xarray.dev/en/stable/user-guide/io.html), [h5py](https://docs.h5py.org/en/stable/), [Arrow](https://arrow.apache.org/docs/python/), [Rasterio](https://rasterio.readthedocs.io/), [Astropy](https://www.astropy.org/), [GeoPandas](https://geopandas.org/).

**Rotina sugerida:** registrar a fonte e versão; baixar uma amostra; inspecionar unidades e qualidade; executar a transformação em script/notebook; salvar uma saída pequena para a interface. Preservar o original e o código de transformação, em vez de editar manualmente o único exemplar.


## 13. Recursos especializados: radar, astronomia, biologia e física

Estas são opções especializadas, não dependências obrigatórias. Usá-las quando o problema e o conjunto científico justificarem; a interpretação do dado continua sendo responsabilidade da equipe.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **ASF Search / asf_search** | Encontrar e baixar produtos de radar/SAR do catálogo ASF | Acesso conforme o produto, normalmente com Earthdata Login. Processamento SAR exige conhecer o nível e a geometria do produto. | [Documentação / condições](https://docs.asf.alaska.edu/asf_search/basics/) |
| **NASA NISAR** | Localizar informações, produtos e documentação da missão de radar | Fonte científica; não é uma ferramenta que resolve a análise automaticamente. Conferir distribuição e produtos adequados. | [Documentação / condições](https://science.nasa.gov/mission/nisar/) |
| **MintPy** | Analisar séries temporais de interferometria SAR e deformação | Código aberto; especializado, com pré-processamento e entradas próprias. Não é a primeira opção para uma equipe sem experiência em InSAR. | [Documentação / condições](https://github.com/insarlab/MintPy) |
| **IRSA / SPHEREx** | Consultar produtos e documentação astronômica da missão SPHEREx | Acesso a produtos públicos conforme a liberação; citar versão e seguir orientações de calibração e uso. | [Documentação / condições](https://irsa.ipac.caltech.edu/Missions/spherex.html) |
| **astroquery** | Consultar arquivos e catálogos astronômicos via Python | Aberto; serviços consultados têm disponibilidade, limites e atribuição próprios. | [Documentação / condições](https://astroquery.readthedocs.io/en/latest/) |
| **Photutils** | Detectar fontes e medir brilho em imagens astronômicas | Aberto, integrado ao ecossistema Astropy; não confundir brilho instrumental com grandeza física já calibrada. | [Documentação / condições](https://github.com/astropy/photutils) |
| **SpiceyPy / NASA SPICE** | Calcular geometria de observação e relações entre corpos e sondas | Wrapper aberto; exige kernels apropriados, com origem e versões registradas. | [Documentação / condições](https://spiceypy.readthedocs.io/en/main/) |
| **SunPy** | Trabalhar com observações solares, coordenadas e séries temporais | Aberto; produto, instrumento, unidade e sistema de referência precisam ser conferidos. | [Documentação / condições](https://docs.sunpy.org/en/stable/) |
| **NASA OSDR** | Encontrar dados de biologia espacial e experimentos associados | Portal de dados; consultar acesso, metadados e restrições do estudo. Não usar para prometer diagnóstico individual. | [Documentação / condições](https://science.nasa.gov/biological-physical/data/) |
| **NASA Physical Sciences Informatics — PSI** | Localizar resultados de experimentos de ciências físicas em ambiente espacial | Recurso científico; disponibilidade e documentação dependem do experimento. | [Documentação / condições](https://science.nasa.gov/biological-physical/data/) |
| **Cantera** | Modelar termodinâmica, cinética química e transporte | Software aberto; uso avançado. Uma simulação simples não equivale a reproduzir todas as condições de microgravidade. | [Documentação / condições](https://www.cantera.org/) |

**Exemplos de combinação:** para imagens de céu, IRSA + Astropy + Photutils + Plotly; para exploração de radar, ASF + QGIS + Python; para experimento físico, dados PSI + NumPy/SciPy e, somente quando necessário, Cantera.

**Cuidados de interpretação sugeridos:** não misturar radar, imagem óptica e indicador derivado como se fossem a mesma medida; não inferir condição de saúde de astronauta a partir de uma visualização demonstrativa; identificar simulações e dados sintéticos como tais. Modelos avançados ficam como extensão, não como requisito artificial do primeiro protótipo.


## 14. Incerteza, unidades e validação dos resultados

Um gráfico convincente não basta: o projeto deve explicar o que calculou, com quais unidades e quais limitações. Esta seção complementa NumPy, SciPy, scikit-learn e statsmodels.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **Pint** | Controlar unidades físicas e conversões nos cálculos | Biblioteca aberta e local; declarar as unidades de entrada antes de operar. | [Documentação / condições](https://pint.readthedocs.io/en/stable/) |
| **PyMC** | Modelagem probabilística e estimativa de incerteza | Aberto; requer conhecimento estatístico e pode demandar bastante computação. Opcional para o MVP. | [Documentação / condições](https://www.pymc.io/projects/docs/en/stable/learn.html) |
| **SALib** | Avaliar quanto a saída de um modelo muda com seus parâmetros | Aberto; análise de sensibilidade pode exigir muitas execuções. Escolher método compatível com o orçamento computacional. | [Documentação / condições](https://salib.readthedocs.io/en/latest/) |

### Protocolo mínimo sugerido, sem depender de mais ferramentas

| Pergunta | Evidência a apresentar |
|---|---|
| O cálculo representa a grandeza correta? | Fórmula, unidade, origem e conversões |
| Existe referência simples para comparação? | Resultado de uma regra básica, histórico ou modelo de base |
| O modelo foi avaliado em dados diferentes dos usados no ajuste? | Separação documentada, respeitando a estrutura temporal/espacial quando pertinente |
| Um resultado ruim está sendo escondido? | Métrica, exemplos de erro e limitações |
| Os valores são observados, estimados ou inventados para simulação? | Identificação explícita de cada categoria |
| O dado é recente o suficiente? | Data de aquisição, processamento e consulta |
| A conclusão extrapola o alcance do teste? | Limite geográfico, período e público para o qual foi demonstrada |

**Exemplo:** em uma previsão demonstrativa, comparar o modelo com uma regra simples e mostrar os erros. Não chamar uma solução de “precisa” apenas porque a curva visualmente acompanha o histórico. Para o método de avaliação escolhido, consultar também a [documentação de avaliação do scikit-learn](https://scikit-learn.org/stable/modules/model_evaluation.html).


## 15. IA para construir aplicativos, trabalhar com documentos e executar modelos

Separar quatro situações: **IA usada para construir**, **IA integrada ao produto**, **modelo executado localmente** e **serviço pago por uso**. Gerar código com uma ferramenta não concede uso gratuito da API dela dentro do aplicativo.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **OpenAI Codex** | Editar código, investigar falhas e executar tarefas de desenvolvimento | Incluído nos planos ChatGPT, inclusive Free, com limites. Codex Cloud não está incluído em Free/Go; disponibilidade e modalidade variam. | [Documentação / condições](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan) |
| **Gemini CLI** | Apoio à programação e tarefas no terminal | Cliente aberto; cotas e cobrança dependem da autenticação e do provedor/modelo usados. | [Documentação / condições](https://github.com/google-gemini/gemini-cli/blob/main/docs/resources/quota-and-pricing.md) |
| **Aider** | Programar com IA dentro de um repositório Git | Ferramenta aberta; custo depende do modelo remoto ou do computador que executa o modelo local. | [Documentação / condições](https://aider.chat/docs/llms) |
| **Continue** | Integrar assistência de IA ao editor com modelos escolhidos pela equipe | Componentes abertos; conexão a modelo local ou provedor com condições próprias. | [Documentação / condições](https://docs.continue.dev/customize/model-providers/overview) |
| **v0** | Gerar e iterar interfaces e aplicações web a partir de instruções | Plano gratuito limitado; deploy, serviços conectados e execução de IA no produto devem ser avaliados separadamente. | [Documentação / condições](https://v0.app/pricing) |
| **Lovable** | Montar um protótipo web assistido por IA | Créditos gratuitos limitados; construção, nuvem, IA em execução e integrações não devem ser tratados como ilimitados. | [Documentação / condições](https://docs.lovable.dev/introduction/credits-and-usage) |
| **Bolt** | Criar e alterar aplicativos web no navegador | Plano gratuito sujeito a limites; verificar créditos, exportação, hospedagem e dependências antes de comprometer o projeto. | [Documentação / condições](https://support.bolt.new/building/quickstart) |
| **ONNX Runtime Web** | Executar modelos compatíveis no navegador | Runtime aberto; memória, desempenho, operadores e aceleração variam por dispositivo. Licença do modelo é separada. | [Documentação / condições](https://onnxruntime.ai/docs/tutorials/web/) |
| **Transformers.js** | Executar tarefas de linguagem, visão ou áudio no navegador | Biblioteca aberta; escolher modelos compatíveis e leves. Primeiro download pode depender de internet. | [Documentação / condições](https://huggingface.co/docs/transformers.js/index) |
| **Docling** | Converter documentos em estrutura utilizável para pesquisa e consulta | Código aberto; conferir modelos auxiliares, recursos computacionais e direito de uso do documento. | [Documentação / condições](https://github.com/docling-project/docling) |
| **pypdf** | Extrair texto de PDFs digitais e manipular páginas | Aberto; não é motor de OCR. PDF com texto mal estruturado pode exigir outra abordagem. | [Documentação / condições](https://github.com/py-pdf/pypdf) |
| **MLflow** | Registrar experimentos, parâmetros, métricas e modelos | Edição aberta executável pela equipe; armazenamento e serviços gerenciados podem ter custo. | [Documentação / condições](https://mlflow.org/docs/latest/) |
| **DVC** | Versionar referências a dados e modelos junto ao projeto | Aberto; o armazenamento remoto não fica gratuito por consequência. Para um pequeno CSV, Git comum pode bastar. | [Documentação / condições](https://dvc.org/doc) |

### Como escolher sem ficar dependente da IA

**Para programar:** usar um assistente principal e Git, com alterações revisadas. Evitar que dois agentes editem simultaneamente os mesmos arquivos. Começar por uma funcionalidade pequena que rode fora do editor da ferramenta.

**Para construir com v0, Lovable ou Bolt:** testar cedo a obtenção do código, instalação local, conexão ao banco e publicação na hospedagem escolhida. Um preview dentro da plataforma não comprova que o projeto funciona fora dela.

**Para colocar IA no produto:** definir entrada, saída, modelo, licença, tamanho máximo, limite por usuário e alternativa quando a cota acabar. Não enviar credenciais, dados pessoais ou material confidencial a planos de IA sem conferir os termos. A Gemini API diferencia condições por modalidade; a API da OpenAI tem faturamento separado do ChatGPT. [Gemini API](https://ai.google.dev/gemini-api/docs/pricing) · [ChatGPT e API](https://help.openai.com/en/articles/9039756-managing-billing-for-chatgpt-and-the-api-platform).

**Para a demonstração:** uma resposta pré-calculada pode ser plano B, mas deve ser claramente identificada como exemplo armazenado, nunca apresentada como execução ao vivo. Ferramentas de RAG ajudam a recuperar documentos; ainda é necessário conferir se a resposta é sustentada pela fonte.


## 16. Aplicativos móveis, interfaces e funcionamento offline

Para o hackathon, uma aplicação web responsiva costuma ser uma proposta inicial mais simples do que depender de publicação em lojas. Aplicativo nativo só deve entrar quando o problema justificar sensores, integração ou experiência específica.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **Expo / React Native** | Criar uma aplicação para celular com JavaScript/TypeScript | Ecossistema aberto; Expo Go permite testes, enquanto EAS possui cotas e serviços pagos. Testar no aparelho real. | [Documentação / condições](https://docs.expo.dev/faq/) |
| **PWA — Progressive Web App** | Oferecer experiência web instalável e recursos offline quando implementados | Abordagem baseada em tecnologias web; instalação e capacidades variam por navegador. Não fica offline automaticamente. | [Documentação / condições](https://web.dev/learn/pwa/) |
| **Workbox** | Implementar estratégias de cache e atualização em uma PWA | Bibliotecas abertas; definir o que pode ser armazenado e como atualizar dados. Não guardar informações sensíveis sem análise. | [Documentação / condições](https://developer.chrome.com/docs/workbox/) |
| **Astro** | Publicar site de apresentação, narrativa ou documentação com pouca lógica de servidor | Framework aberto; hospedar versão estática reduz dependências de backend. | [Documentação / condições](https://docs.astro.build/en/getting-started/) |
| **shadcn/ui** | Montar interface React com componentes que a equipe pode adaptar | Código de componentes aberto; a equipe continua responsável por testes, acessibilidade e compatibilidade. | [Documentação / condições](https://ui.shadcn.com/docs) |
| **Lucide** | Usar ícones consistentes na interface e no pitch | Licença ISC; preservar avisos exigidos. Ícone não substitui rótulo compreensível. | [Documentação / condições](https://lucide.dev/license) |
| **Google Fonts** | Escolher tipografia com arquivos e licenças identificáveis | Catálogo com fontes abertas; conferir a licença da família escolhida e documentar a atribuição exigida. | [Documentação / condições](https://github.com/google/fonts) |

**Teste de experiência sugerido:** abrir em um celular, percorrer a página com teclado, verificar contraste e legibilidade, mostrar estado de carregamento e erro, incluir rótulos nos formulários e não depender somente de cor para comunicar um resultado.

**Offline de verdade:** manter interface, amostra autorizada dos dados e dependências necessárias disponíveis localmente. Fazer um teste desconectado. Não prometer offline se a tela depende de mapas, fontes, autenticação ou modelo carregados apenas de um servidor externo.

**Mapa offline:** a licença dos dados OpenStreetMap não autoriza baixar em massa os tiles do servidor público para montar um cache offline. Usar dados/tiles cuja distribuição permita isso, com atribuição. [Política oficial de tiles](https://operations.osmfoundation.org/policies/tiles/).


## 17. Sonificação, áudio, vídeo, diagramas e narrativa

Sonificação significa associar valores dos dados a características do som. É diferente de gerar uma música decorativa. A regra de conversão deve ser explicada para que o público entenda o que está ouvindo.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **Tone.js** | Transformar dados em sequências sonoras interativas no navegador | Biblioteca aberta sobre Web Audio; testar início de áudio após interação do usuário e controle de volume. | [Documentação / condições](https://tonejs.github.io/) |
| **Web Audio API** | Sintetizar e processar áudio diretamente no navegador | Tecnologia nativa, sem contratar API de IA; verificar comportamento no navegador da demonstração. | [Documentação / condições](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) |
| **librosa** | Analisar características de áudio, espectrogramas e padrões musicais | Biblioteca aberta em Python; áudio de terceiros continua sujeito à própria licença. | [Documentação / condições](https://librosa.org/doc/) |
| **p5.js** | Criar arte generativa e experiências educativas visuais | Biblioteca aberta; combina dados, interação e desenho no navegador. | [Documentação / condições](https://p5js.org/) |
| **Piper** | Gerar fala a partir de texto localmente | Motor GPL-3.0; conferir separadamente a licença de cada voz/modelo e capacidade do computador. | [Documentação / condições](https://github.com/OHF-Voice/piper1-gpl) |
| **ElevenLabs** | Experimentar narração e outros recursos de áudio por IA | Plano gratuito com créditos, sem presumir licença comercial; a página de planos inclui licença comercial a partir de plano pago. Validar direitos antes de publicar. | [Documentação / condições](https://elevenlabs.io/pricing) |
| **Runway** | Gerar pequenos trechos visuais para explicar um conceito | Plano Free com créditos concedidos uma única vez, não renovação mensal ilimitada. Recursos e direitos do resultado devem ser conferidos. | [Documentação / condições](https://runway.com/pricing) |
| **FFmpeg** | Converter, comprimir e combinar áudio/vídeo para a entrega | Software aberto; licenciamento depende da compilação e componentes ativados. Conferir ao redistribuir binários. | [Documentação / condições](https://ffmpeg.org/legal.html) |
| **Mermaid** | Produzir diagramas de arquitetura e fluxos a partir de texto | Biblioteca aberta e editor disponíveis; serviços adicionais da plataforma têm condições próprias. | [Documentação / condições](https://mermaid.js.org/) |

### Exemplo prático de sonificação

Em uma série de temperatura, a equipe pode mapear valores maiores para notas mais agudas e períodos sem medição para uma indicação de ausência, sem inventar valores. Exibir simultaneamente o gráfico, explicar a escala usada e oferecer opção de silenciar. É uma **representação do dado**, não um som naturalmente emitido pela temperatura.

### Escolha simples para o pitch

**Gravação real da aplicação + OBS + Audacity + Kdenlive** é uma alternativa inicial sem depender de créditos de vídeo generativo. Usar imagens de IA como ilustração conceitual identificada, não como fotografia de fenômeno observado ou evidência científica. Para narração, a voz de um integrante com áudio bem captado pode ser suficiente.

Guardar a origem de músicas, vozes, imagens e modelos 3D. Uma licença do editor não licencia automaticamente os materiais importados. Não usar voz de terceiros sem autorização.


## 18. Integrações, serviços de apoio, automação e sensores

Esta camada costuma ficar esquecida entre “o site funciona” e “a demonstração funciona para outra pessoa”. Adotar somente o que resolve uma necessidade real; nem todo aplicativo precisa de fila, cache, automação e busca vetorial.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **HTTPX** | Consultar APIs em Python com tratamento de conexões e respostas | Biblioteca aberta; configurar timeout e lidar com falhas e limites do serviço externo. | [Documentação / condições](https://www.python-httpx.org/) |
| **Pydantic** | Validar o formato das entradas e saídas de uma API Python | Biblioteca aberta; validação de tipos não substitui regras de negócio nem autorização. | [Documentação / condições](https://docs.pydantic.dev/latest/) |
| **SQLAlchemy** | Acessar bancos SQL em Python de forma estruturada | Biblioteca aberta; banco e hospedagem continuam sendo decisões separadas. | [Documentação / condições](https://www.sqlalchemy.org/) |
| **Alembic** | Versionar alterações no esquema de um banco usado com SQLAlchemy | Aberto; revisar migrações e testar recuperação antes de mudanças destrutivas. | [Documentação / condições](https://alembic.sqlalchemy.org/en/latest/) |
| **PostGIS** | Executar consultas espaciais em PostgreSQL | Extensão aberta; conferir disponibilidade no serviço de banco escolhido. Útil para proximidade e interseção de regiões. | [Documentação / condições](https://postgis.net/) |
| **pgvector** | Armazenar vetores e consultar similaridade no PostgreSQL | Extensão aberta; embeddings e processamento do modelo têm custo/licença separados. Só incluir se houver busca semântica. | [Documentação / condições](https://github.com/pgvector/pgvector) |
| **PMTiles** | Distribuir mapas em um arquivo de tiles com leitura parcial | Formato/ecossistema aberto; hospedagem precisa atender o acesso esperado. Licença do mapa e dos dados é separada. | [Documentação / condições](https://docs.protomaps.com/pmtiles/) |
| **Resend** | Enviar e-mails de confirmação, recuperação ou notificações | Plano gratuito com cotas; envio público requer domínio próprio verificado, que pode ter custo. Não resolve automaticamente toda a configuração do Auth. | [Documentação / condições](https://resend.com/pricing) |
| **Upstash Redis** | Adicionar cache e contadores para limitar chamadas | Serviço gerenciado com plano gratuito limitado; usar apenas quando um cache simples não bastar. | [Documentação / condições](https://upstash.com/pricing/redis) |
| **APScheduler** | Agendar rotinas em uma aplicação Python | Aberto; precisa de processo/infraestrutura que permaneça disponível. Não garante execução em serviço suspenso. | [Documentação / condições](https://apscheduler.readthedocs.io/en/3.x/) |
| **Node-RED** | Conectar APIs, sensores e eventos por fluxos visuais | Aberto, Apache 2.0; hospedagem e credenciais das integrações precisam ser administradas. | [Documentação / condições](https://nodered.org/about/) |
| **n8n — opção com restrição de licença** | Automatizar integrações visualmente | Self-hosted sob Sustainable Use License, com usos permitidos e restrições; não classificar como licença OSI. Nuvem e infraestrutura podem ser pagas. | [Documentação / condições](https://github.com/n8n-io/n8n-docs/blob/main/docs/n8n-community-license/README.md) |
| **Eclipse Mosquitto** | Receber e distribuir mensagens MQTT de sensores | Broker aberto; requer instalação e configuração segura. Não publicar um broker irrestrito na internet. | [Documentação / condições](https://mosquitto.org/) |

### O que precisa estar combinado entre frontend, API e banco

Registrar o formato de cada resposta, o responsável pelo endpoint, autenticação, unidades, data dos dados e mensagens de erro. Definir uma resposta demonstrativa local para testes e uma estratégia de tentativas limitada; chamadas repetidas sem controle podem esgotar a cota do fornecedor.

Para uma consulta que demora, a proposta inicial mais simples pode ser **processar antecipadamente um recorte e servir o resultado**, identificando quando foi produzido. Para atualização periódica, confirmar onde o agendamento realmente executa; uma função que não está ativa não se transforma em serviço contínuo por possuir um agendador.

**Mapas e geocodificação:** a API pública Nominatim impõe limite de uso e não deve ser tratada como infraestrutura ilimitada para buscas do aplicativo. A documentação exige, entre outros cuidados, identificação e controle de requisições. [Política oficial](https://operations.osmfoundation.org/policies/nominatim/).

**E-mail:** verificar domínio, remetente, entrega em provedores externos e spam antes da apresentação. [Domínios no Resend](https://resend.com/docs/dashboard/domains/introduction).

**Hardware:** Wokwi e Tinkercad ajudam a demonstrar um circuito sem compra imediata. Se houver Arduino/ESP32 físico, listar sensor, alimentação, cabo de dados, driver e forma de comunicação. Testar o conjunto completo; simulação não comprova desempenho físico de um dispositivo.


## 19. Segurança, documentação, licenças e reprodução

A proposta abaixo é uma barreira básica de qualidade para o protótipo, não uma certificação de segurança. Manter os testes pytest/Playwright/Lighthouse da seção 10 e acrescentar verificações proporcionais ao projeto.

| Ferramenta ou recurso | Ideal para | Gratuidade e cuidado prático | Fonte oficial |
|---|---|---|---|
| **Gitleaks — linha de comando** | Procurar credenciais acidentalmente salvas no código e histórico Git | Ferramenta aberta; serviços/ações adicionais podem ter termos próprios. Uma varredura sem alerta não garante ausência de segredos. | [Documentação / condições](https://github.com/gitleaks/gitleaks) |
| **pip-audit** | Verificar vulnerabilidades conhecidas em dependências Python | Aberto; não detecta todo tipo de falha e não substitui atualização/testes. | [Documentação / condições](https://github.com/pypa/pip-audit) |
| **REUSE** | Organizar identificação de licença e autoria por arquivo | Ferramentas e especificação abertas; ajudam no inventário, mas não decidem compatibilidade jurídica por conta própria. | [Documentação / condições](https://reuse.software/) |
| **Quarto** | Publicar análise reprodutível, relatório e apresentação a partir de Markdown/notebooks | Aberto; ferramentas auxiliares podem ser necessárias conforme a saída. HTML é uma opção simples para consulta. | [Documentação / condições](https://quarto.org/) |

### Pacote mínimo sugerido para outra pessoa entender e executar

| Arquivo ou pasta | O que registrar |
|---|---|
| `README.md` | Problema, desafio, solução, instruções de execução, link da demo e limitações |
| `LICENSE` | Licença escolhida para o código original, compatível com as obrigações assumidas |
| `SOURCES.md` | Conjuntos de dados, versões, recortes, data de consulta, créditos e links |
| `THIRD_PARTY_NOTICES.md` | Avisos de bibliotecas, imagens, fontes, modelos, áudio e demais materiais |
| `AI_USAGE.md` | Ferramentas de IA, finalidade, partes assistidas e revisão realizada pela equipe |
| `pyproject.toml` + `uv.lock`, ou alternativa equivalente | Ambiente Python reproduzível |
| `package.json` + arquivo de trava correspondente | Dependências JavaScript e comandos de execução |
| `.env.example` | Somente nomes e valores fictícios; nunca credenciais reais |
| `data/sample/` | Amostra pequena cuja redistribuição seja permitida, ou script para obtê-la |
| `tests/` | Testes básicos de cálculo, carregamento de dados e fluxos essenciais |
| `MODEL_CARD.md`, quando aplicável | Modelo, licença, treinamento, avaliação, limitações e uso esperado |
| `demo/` | Capturas e vídeo de apoio, com indicação do que foi executado e do que é simulado |

**Esses nomes são uma organização sugerida, não uma lista de arquivos obrigatórios estabelecida pelo evento.**

### Testes de segurança prioritários

Testar acesso sem login e com dois usuários diferentes: um usuário não deve conseguir ler ou alterar registros privados do outro. Não usar dados pessoais reais quando dados públicos ou sintéticos identificados resolvem a demonstração. Limitar tamanho/tipo de uploads, evitar credenciais em logs e impedir que campos de texto executem comandos arbitrários.

Variáveis com prefixo de exposição pública do framework podem ser incorporadas ao navegador; colocá-las em `.env` não as torna secretas. Guardar segredos no ambiente do servidor e, se houver vazamento, revogar/trocar a chave — apagar a linha do último commit não basta. Usar as orientações do [Supabase sobre chaves e acesso](https://supabase.com/docs/guides/getting-started/api-keys) e um scanner como Gitleaks.

### Teste de reprodução e recuperação

Um integrante que não escreveu a funcionalidade deve seguir o README em um ambiente limpo, carregar a amostra e executar o fluxo principal. Exportar os dados importantes e **testar a restauração**; possuir um arquivo de backup ainda não prova que ele serve para recuperar o projeto.

Manter um registro simples de versões, fonte de dados e comandos executados é mais útil que instalar uma plataforma complexa de experimentos sem necessidade.

## 20. Escolha por problema: qual parte da maleta abrir?

A matriz abaixo é uma **proposta de arquitetura**, não uma lista de tecnologias obrigatórias ou uma confirmação de aderência a todos os enunciados. Depois de escolher o desafio, validar seus dados, requisitos, critérios e entregáveis na página oficial.

| Família de problema | Conjunto inicial sugerido | O que evitar no primeiro protótipo |
|---|---|---|
| Painel climático, ambiental ou agrícola | Fonte NASA adequada + pandas/xarray + Streamlit + Plotly | Banco, login e IA sem necessidade demonstrada |
| Mapa de focos de calor | FIRMS + Python + Folium/Streamlit; ou React/Leaflet para web própria | Prometer alerta operacional ou precisão não validada |
| Radar e mudanças da superfície | ASF/NISAR + QGIS + Python; MintPy somente para análise compatível | Processar o planeta inteiro ou começar por técnica desconhecida |
| Imagens e catálogos astronômicos | IRSA/arquivo NASA + Astropy + astroquery/Photutils + Plotly | Interpretar imagem sem conferir calibração e coordenadas |
| Órbitas e geometria espacial | Horizons + Skyfield/Astropy; SpiceyPy/Orekit quando necessários | Escolher biblioteca arquivada ou fazer simulação física sem hipótese explícita |
| Educação, jogo e narrativa | Dados/fontes NASA + Godot ou React/Three.js + OBS | Vários motores gráficos e funcionalidades sem relação com a aprendizagem |
| Sonificação de séries ambientais | Dados NASA + Python para preparar + Tone.js/Web Audio + gráfico | Trilha sonora decorativa apresentada como tradução científica dos dados |
| Saúde e biologia espacial | OSDR/fontes apropriadas + Python + painel com dados públicos ou sintéticos identificados | Dados pessoais desnecessários e alegações diagnósticas |
| Ciências físicas e microgravidade | PSI/dados do experimento + NumPy/SciPy; Cantera se justificado | Tratar um modelo simplificado como reprodução completa do fenômeno |
| Aplicativo com usuários e histórico | React/Vite + Supabase + hospedagem gerenciada compatível | VPS e API separadas se o backend gerenciado já resolver |
| Busca ou assistente sobre documentos | Documentos autorizados + extração + busca simples; embeddings/RAG só se agregarem valor | Chatbot sem fontes ou cobrança de IA sem controle |
| Sensor ou demonstrador de hardware | Arduino/ESP32 ou Wokwi + Node-RED/MQTT se necessário | Comprar equipamento antes de provar a utilidade e a integração |
| Consulta de campo com internet instável | PWA + amostra/cache autorizado + atualização identificada | Dependências externas escondidas sob a promessa de “offline” |

### 20.1 Critério de escolha da equipe

Para cada alternativa, registrar uma resposta curta a estas perguntas:

| Critério | Pergunta decisiva |
|---|---|
| Adequação | Ela resolve uma função necessária do projeto? |
| Conhecimento | Alguém da equipe consegue instalar, explicar e depurar? |
| Disponibilidade | A conta, a região, a API e os dados já estão acessíveis? |
| Custo | O uso esperado cabe no plano, inclusive durante a avaliação posterior? |
| Licença | Código, modelo, dado e material visual podem ser usados e publicados nas condições necessárias? |
| Demonstração | Existe alternativa quando internet, servidor ou crédito falhar? |

**Regra de corte sugerida:** uma ferramenta só entra na primeira versão se sua ausência impedir demonstrar a ideia central. Recursos “interessantes”, mas não essenciais, ficam numa lista de evolução.

### 20.2 Combinações prontas por tipo de desafio


#### A. Queimadas, desmatamento ou desastres
**NASA FIRMS + Python/GeoPandas + Streamlit/Folium**, ou **React/Leaflet** para uma interface web própria. QGIS e Worldview ajudam na inspeção. Não é necessário manter dois frontends. Usar dados com data, resolução e latência identificadas; focos de calor não devem ser apresentados automaticamente como perímetro ou área queimada. Complementar com INPE/Open-Meteo quando pertinente.

#### B. Mudanças climáticas, calor urbano ou agricultura
**NASA POWER + Copernicus/USGS + pandas/xarray + scikit-learn + Plotly + Streamlit.** Comparar históricos e criar mapas/curvas. Usar Earth Engine somente quando a elegibilidade e cotas estiverem confirmadas.

#### C. Órbitas, asteroides e exploração do espaço
**NASA JPL Horizons/SBDB + Astropy + Skyfield + NumPy + Three.js ou CesiumJS.** Ilustrar trajetória com intervalos físicos consistentes; apresentar incertezas de modelos.

#### D. Educação, acessibilidade e ciência para o público
**NASA dados oficiais + React/Vite + Leaflet/Three.js + Figma + Canva/OBS.** Criar experiência narrativa acessível, com elementos visuais legendados e dados citados.

#### E. Classificação de imagens com inteligência artificial
**Dados NASA/Copernicus + Rasterio/OpenCV + scikit-learn/PyTorch + Colab/Kaggle + Gradio.** Preferir modelo pequeno pré-treinado e conjunto de teste claro; confirmar licença dos pesos e não depender de GPU disponível no evento.

#### F. Otimização logística de resposta a emergências
**NASA FIRMS + Open-Meteo + OpenStreetMap + OR-Tools + FastAPI + Leaflet.** Explicitar que rotas simuladas não substituem dados viários operacionais nem orientação de segurança.

#### G. Solução sem programador experiente
**Google Sheets/CSV + ChatGPT/Gemini para apoio + Streamlit ou Gradio + Canva + OBS.** Construir uma prova de conceito enxuta e verificável, com código validado pela equipe.

## 21. Plano de demonstração, contingência e entrega

### 21.1 Plano B por tipo de falha

| Dependência que pode falhar | Preparação sugerida | O que informar ao público |
|---|---|---|
| Internet ou fonte de dados externa | Amostra local autorizada e identificada | Data do recorte; não afirmar atualização ao vivo |
| API de IA sem crédito ou indisponível | Fluxo sem IA, modelo local testado ou exemplo de resposta armazenada | Indicar quando não houve inferência ao vivo |
| Serviço suspenso ou inicialização lenta | Testar acesso de ponta a ponta; cópia local executável | Distinguir a demonstração local da instância pública |
| Banco pausado, expirado ou inacessível | Exportação e procedimento de restauração testado | Não fingir que uma gravação foi persistida |
| Confirmação de e-mail falhando | Área pública de leitura ou autenticação já validada | Esclarecer o fluxo que está sendo demonstrado |
| Mapa base ou tiles indisponíveis | Camada autorizada local ou visualização alternativa | Preservar créditos; não violar políticas de download |
| GPU ou memória insuficiente | Recorte menor, modelo leve ou resultado pré-calculado | Informar limites da execução |
| Áudio/vídeo não toca no equipamento | Arquivo local compatível, legendas e roteiro sem áudio | Manter a explicação compreensível sem efeito multimídia |
| Queda da hospedagem após o evento | Responsável por manutenção, monitoramento e cópia da entrega | Manter links acessíveis pelo período aplicável à avaliação |

### 21.2 Conferência final sugerida

- [ ] Desafio e entregável conferidos na fonte oficial, sem confundir esta maleta com o regulamento.
- [ ] Projeto abre em janela anônima, outro aparelho e conta não pertencente à equipe.
- [ ] Um usuário consegue concluir a ação principal; erros e ausência de dados têm mensagens compreensíveis.
- [ ] Datas, unidades, fontes, recortes e limitações científicas aparecem no projeto.
- [ ] Dados simulados, conteúdo de IA e resultados pré-calculados estão identificados.
- [ ] Login, confirmação, recuperação e regras de acesso foram testados quando utilizados.
- [ ] Segredos não constam no frontend, repositório, histórico, capturas ou logs compartilhados.
- [ ] Cotas, suspensão, expiração, faturamento e manutenção após o evento têm responsável.
- [ ] Há cópia recuperável de dados, código, vídeo, slides e materiais permitidos.
- [ ] A versão final foi identificada no Git; README e dependências refletem o código entregue.
- [ ] Fontes, licenças, modelos, imagens, vozes e bibliotecas estão documentados.
- [ ] A demonstração continua compreensível sem internet e sem áudio.
- [ ] Idioma, formato, duração e prazos da submissão foram conferidos nas regras aplicáveis.

### 21.3 Organização sugerida do trabalho

**Uma pessoa responsável por cada entrega**, mesmo que todos colaborem: dados/método; desenvolvimento/integração; experiência visual; infraestrutura/segurança; documentação/pitch. Isso não pressupõe cinco integrantes: acumular papéis conforme a equipe.

Antes de acrescentar uma ferramenta, testar o caminho completo de uma pequena função: dado entra → cálculo acontece → resultado aparece → outra pessoa consegue abrir. Depois ampliar. Ao final, estabilizar a versão da apresentação e evitar atualizações de dependências sem tempo para testar.

## Licenças e propriedade intelectual — regras práticas

- **MIT / Apache 2.0 / BSD:** geralmente permitem uso e adaptação inclusive comercial, desde que se preservem avisos pertinentes; Apache 2.0 contém disposições adicionais de patentes e NOTICE.
- **GPL / AGPL:** exigências de reciprocidade podem alcançar a distribuição do trabalho derivado e, na AGPL, uso por rede em determinadas condições. Não presumir que todo código GPL pode ser incorporado sem obrigações.
- **Bibliotecas Python:** verificar cada pacote em seu `LICENSE`, não apenas a licença da linguagem Python.
- **Modelos de IA:** licença de **código**, licença de **pesos**, termos de **API** e licença de **dataset** podem ser quatro coisas distintas. 'Disponível no Hugging Face' não significa 'domínio público'.
- **Dados NASA:** citar missão/instrumento, conjunto, URL e data de acesso; materiais de terceiros distribuídos na NASA podem ter copyright. Identificadores e logotipos da NASA possuem regras próprias; não sugerir endosso da agência.
- **OpenStreetMap:** mostrar `© OpenStreetMap contributors` e indicar a ODbL; checar políticas dos servidores de tiles. A ODbL não equivale a fornecer tiles ilimitados.
- **Open-Meteo:** dados sob CC BY 4.0 com atribuição; API hospedada gratuita principalmente para uso não comercial dentro das cotas. O código do servidor é AGPL.
- **Canva/Figma e imagens geradas:** uso gratuito da ferramenta não torna todos os templates, ícones, imagens ou fontes reutilizáveis sob licença aberta. Verificar direitos do elemento exportado.
- **IA gerando código:** revisar segurança, origem de dependências, qualidade e resultados. Documentar a ferramenta, mas não atribuir licença de software automaticamente ao serviço de IA.
- **Publicação:** usar a organização sugerida na seção 19. A licença do código original não altera a licença de dados, imagens, vozes, pesos de IA e componentes de terceiros.
- **Código disponível não é automaticamente open source:** n8n, por exemplo, utiliza Sustainable Use License com restrições; verificar usos permitidos. [Fonte do mantenedor](https://github.com/n8n-io/n8n-docs/blob/main/docs/n8n-community-license/README.md).
- **Narração e vídeo por IA:** plano gratuito, direitos comerciais e possibilidade de redistribuir os resultados são perguntas diferentes. Dar preferência a material próprio ou com licença expressamente compatível com a entrega.

### Checklist jurídico/técnico antes da entrega

- [ ] Todas as imagens, sons, fontes, modelos 3D e ícones têm origem e autorização documentadas.
- [ ] Dependências (inclusive de IA) com versões e licenças registradas.
- [ ] Referência exata aos datasets NASA e a seus instrumentos/serviços.
- [ ] Segredos apenas no servidor/cofre de segredos; `.env` privado fora do Git. Variáveis públicas incorporadas ao frontend não escondem valores.
- [ ] Termos de tiers gratuitos, cotas e uso não comercial verificados.
- [ ] Demo pode ser executada ou compreendida sem acesso pago.
- [ ] Links e fontes usados no pitch funcionam; dados são rastreáveis.
- [ ] O código original da equipe tem licença definida de acordo com o regulamento oficial.
- [ ] Traduzir/revisar conteúdos exigidos no idioma apropriado.
- [ ] Não apresentar respostas produzidas por IA como dados científicos observados sem validação.

## Riscos de custo e disponibilidade que merecem atenção (checados em 30/10/2026)

1. **Google AI Studio/Gemini API:** há tier gratuito em modelos elegíveis, mas **não** significa geração de imagens por API ilimitada ou gratuita; consultar preços do modelo antes da integração.
2. **Nano Banana:** é uma família de modelos de imagem do Gemini. O acesso pelo aplicativo e pelo endpoint de API têm limites/preços diferentes.
3. **Google Colab:** GPU/TPU gratuita não é garantida; sessões e quotas são dinâmicas.
4. **Google Earth Engine:** projetos não comerciais elegíveis têm cotas mensais e exigem verificação; alguns usos comerciais necessitam serviço pago.
5. **Vercel Hobby:** disponível gratuitamente para aplicações pessoais e não comerciais dentro das condições; para uso fora desse escopo, reavaliar hospedagem.
6. **Supabase Free:** projeto pode pausar por inatividade; manter banco e dados de demonstração em backup.
7. **Hugging Face Spaces:** não confundir custo do hardware com elegibilidade para criar um Space; aplicar as condições da seção 11.2, inclusive a exceção ZeroGPU.
8. **Open-Meteo:** uso não comercial gratuito dentro das cotas, com atribuição; produção comercial requer avaliar serviço.
9. **Figma/Canva:** tiers gratuitos têm restrições de publicação, colaboração e créditos de IA.
10. **NASA Open APIs:** há endpoints arquivados, como Mars Rover API. Confirmar disponibilidade e testar o endpoint escolhido; uma biblioteca antiga pode apontar para serviço descontinuado.

11. **E-mail transacional:** conta de autenticação e capacidade de entregar mensagens são recursos distintos; conferir domínio, remetente e SMTP.
12. **Arquivos e bancos:** separar disco efêmero, banco persistente e armazenamento de objetos; conferir expiração do serviço.
13. **Mapas:** dados abertos e bibliotecas gratuitas não significam tiles, geocodificação ou roteamento hospedados sem limite.
14. **Ferramentas com IA:** créditos para construir não garantem acesso gratuito à IA dentro do aplicativo publicado.
15. **Licença e manutenção:** verificar pacote, versão, dependências, modelo e situação do repositório; código arquivado pode continuar instalável, mas não é uma escolha sem risco.

## Links de referência oficiais usados para validar pontos sensíveis

- [NASA Space Apps Challenge 2026](https://www.spaceappschallenge.org/2026/)
- [NASA Open APIs e alertas de APIs arquivadas](https://api.nasa.gov/)
- [Earthdata CMR API](https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html)
- [Copernicus Data Space APIs](https://dataspace.copernicus.eu/analyse/apis)
- [NASA Media Usage Guidelines](https://www.nasa.gov/nasa-brand-center/images-and-media/)
- [Google Gemini API preços](https://ai.google.dev/gemini-api/docs/pricing)
- [Google Nano Banana — modelos de imagem](https://ai.google.dev/gemini-api/docs/image-generation)
- [Google Colab FAQ](https://research.google.com/colaboratory/faq.html)
- [Google Earth Engine quotas não comerciais](https://developers.google.com/earth-engine/guides/noncommercial_tiers)
- [GitHub Copilot planos](https://github.com/features/copilot/plans)
- [Figma Starter](https://help.figma.com/hc/en-us/articles/13838684089751-Starter-plan-overview)
- [Canva Free](https://www.canva.com/pricing/)
- [Vercel Hobby](https://vercel.com/docs/plans/hobby)
- [Supabase Free](https://supabase.com/pricing)
- [Hugging Face Spaces](https://huggingface.co/docs/hub/en/spaces-overview)
- [Open-Meteo](https://open-meteo.com/)
- [OpenStreetMap License & Attribution](https://www.openstreetmap.org/copyright)

### Referências adicionais da revisão

Os links de cada linha do catálogo são parte das referências. Para as condições operacionais mais importantes:

- [Supabase — SMTP e envio de mensagens](https://supabase.com/docs/guides/auth/auth-smtp).
- [Supabase — chaves publicáveis, segredos e RLS](https://supabase.com/docs/guides/getting-started/api-keys).
- [Render — serviços gratuitos, suspensão e expiração de banco](https://render.com/docs/free).
- [Firebase — exigência de Blaze para Storage](https://firebase.google.com/docs/storage/faqs-storage-changes-announced-sept-2024).
- [Neon — plano gratuito vigente](https://neon.com/pricing).
- [Railway — teste e créditos](https://docs.railway.com/pricing/free-trial).
- [Google Cloud — alertas e limites de gasto](https://docs.cloud.google.com/billing/docs/how-to/budgets).
- [OpenStreetMap — política de tiles](https://operations.osmfoundation.org/policies/tiles/).
- [Nominatim — política do serviço público](https://operations.osmfoundation.org/policies/nominatim/).
- [Resend — domínio verificado](https://resend.com/docs/dashboard/domains/introduction).
- [OpenAI — modalidades e limites do Codex](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan).
- [OpenAI — separação entre faturamento do ChatGPT e API](https://help.openai.com/en/articles/9039756-managing-billing-for-chatgpt-and-the-api-platform).
- [Expo — planos dos serviços EAS](https://docs.expo.dev/billing/plans/).
- [n8n — licença e restrições](https://github.com/n8n-io/n8n-docs/blob/main/docs/n8n-community-license/README.md).
- [poliastro — repositório arquivado](https://github.com/poliastro/poliastro).
- [Excalidraw — recursos da aplicação gratuita](https://github.com/excalidraw/excalidraw).
- [FFmpeg — licenciamento conforme componentes](https://ffmpeg.org/legal.html).
- [NASA — dados de ciências biológicas e físicas](https://science.nasa.gov/biological-physical/data/).
- [IRSA — produtos e documentação SPHEREx](https://irsa.ipac.caltech.edu/Missions/spherex.html).
- [NASA Space Apps — diretório de desafios de 2026](https://www.spaceappschallenge.org/2026/challenges/): consultar integralmente o desafio escolhido antes de definir o projeto.

## Modelo para registrar a escolha definitiva de ferramentas

| Campo | Preencher quando escolher o desafio |
|---|---|
| Desafio e problema | |
| Público-alvo e impacto | |
| Fonte NASA principal / data | |
| Ferramentas essenciais (até 8) | |
| IA utilizada e função | |
| Licenças e termos relevantes | |
| Custos, cotas e contas necessárias | |
| Alternativa offline para a apresentação | |
| Responsável técnico | |
| Comprovação / métrica de resultado | |
| Quem revisou o método científico e as unidades | |
| Necessidade real de login, banco, API e GPU | |
| Domínio/SMTP/URLs de redirecionamento, se usados | |
| Limite de gasto aprovado e modo de bloquear consumo | |
| Data de expiração/pausa e manutenção após o evento | |
| Teste da demo em outra conta/aparelho | |
| Responsável pelo backup e restauração | |
| Versão final do código e data de validação | |

**Nota editorial:** softwares e serviços estão descritos pelo uso recomendado e por uma indicação resumida de regime de acesso. Esta maleta não substitui a leitura do arquivo de licença da versão efetivamente usada, nem representa garantia de disponibilidade ou de elegibilidade do serviço na data de implementação.


**Registro de revisão:** versão 2.0, de 30/10/2026. Foram acrescentadas 70 entradas de ferramentas, tecnologias ou recursos nas seções 12 a 19, além de orientações operacionais e correções nas seções anteriores. Não somar linhas repetidas entre seções para interpretar isso como quantidade de produtos distintos. As escolhas definitivas ficam pendentes da seleção do desafio e dos testes da equipe.
