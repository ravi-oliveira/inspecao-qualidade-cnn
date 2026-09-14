# Inspeção de Qualidade com Visão Computacional e CNN

Mini-Projeto Avaliativo desenvolvido para automatizar a detecção de falhas em peças de fundição metálica (Casting Defect Detection). O pipeline transita entre técnicas de Processamento Clássico de Imagens e Inteligência Artificial.

## Estrutura do Repositório
- `data/raw/`: Imagens brutas divididas entre peças OK e Defeituosas.
- `notebooks/`: Contém o pipeline de execução e documentação visual (`01_analise_exploratoria.ipynb`).
- `venv/`: Ambiente virtual isolado (não versionado) contendo as dependências otimizadas.
- `requirements.txt`: Mapeamento restrito de versões de pacotes do ecossistema.

## Tecnologias Utilizadas
- **OpenCV & Matplotlib:** Análise exploratória clássica (Grayscale, Gaussian Blur, Limiarização, Canny Edge Detection, Operações Morfológicas).
- **TensorFlow & Keras:** Ingestão de dados otimizada, Data Augmentation dinâmico e arquitetura profunda (CNN).
- **Git:** Versionamento do projeto estruturado através de branches (Sprints).

## Metodologia e Sprints
1. **Configuração de Ambiente:** Isolamento de dependências.
2. **OpenCV Filtros Básicos:** Remoção de ruídos de textura metálica natural.
3. **OpenCV Morfologia:** Isolamento da trinca através da detecção de quebra brusca de intensidade de pixels.
4. **Data Augmentation:** Imunização da IA contra variações luminosas e rotações físicas na esteira de produção.
5. **Arquitetura CNN:** Extração hierárquica de características em tensores multidimensionais, finalizando em uma camada Densa de classificação binária (Sigmoid).
6. **Auditoria:** Representação gráfica atestando um aprendizado saudável (sem overfitting agressivo) ao cruzar métricas de Treino e Validação.