# 🫁 Breath2Vision

Um projeto de visão computacional para detecção de doenças respiratórias usando espectrogramas de sons pulmonares e modelos de aprendizado profundo.

## 📋 Índice

- [🫁 Breath2Vision](#-breath2vision)
  - [📋 Índice](#-índice)
  - [🔍 Visão Geral](#-visão-geral)
    - [Problema](#problema)
    - [Solução Proposta](#solução-proposta)
  - [📊 Dataset](#-dataset)
    - [ICBHI 2017 Respiratory Sound Database](#icbhi-2017-respiratory-sound-database)
  - [🔬 Metodologia](#-metodologia)
    - [Métricas de Avaliação](#métricas-de-avaliação)
  - [📚 Literatura](#-literatura)

## 🔍 Visão Geral

### Problema

O diagnóstico de doenças respiratórias (asma, pneumonia, DPOC) tradicionalmente depende da ausculta pulmonar por profissionais experientes. Este processo apresenta limitações:

- **Subjetividade**: Interpretação varia entre profissionais
- **Dependência de expertise**: Requer anos de experiência clínica
- **Acesso limitado**: Escassez de especialistas em regiões remotas
- **Variabilidade**: Condições ambientais podem afetar a ausculta

### Solução Proposta

Desenvolvimento de um sistema automatizado que:

- Converte sons respiratórios em espectrogramas
- Aplica redes neurais convolucionais para classificação
- Fornece diagnóstico objetivo e reproduzível
- Permite telemedicina e triagem automática

## 📊 Dataset

### ICBHI 2017 Respiratory Sound Database

Será utilizado o **ICBHI 2017 Respiratory Sound Database**, que contém 6.898 ciclos respiratórios de 126 pacientes, incluindo sons normais e patológicos (sibilos e estertores), relacionados a diversas doenças respiratórias.

Exemplo de dados no dataset:
![image](https://github.com/user-attachments/assets/53cb0b9a-ae19-465f-a503-7974d8a6dcb4)

[Mais informações sobre o ICBHI Dataset](https://www.researchgate.net/figure/ICBHI-respiratory-database-comprised-of-LS-from-various-pulmonary-pathologies_fig4_345978905?)

## 🔬 Metodologia

O projeto utilizará as seguintes abordagens:

- **Transformada Wavelet Packet**: para decomposição dos sinais e extração de características.
- **Espectrogramas**: conversão dos sinais de áudio em imagens para entrada em redes neurais.
- **Redes Neurais Convolucionais (CNNs)**: para classificar os espectrogramas.
- **Modelos como RespireNet**: otimizados para conjuntos de dados pequenos.

### Métricas de Avaliação

- **Acurácia Global**: Percentual de classificações corretas
- **Sensibilidade (Recall)**: Capacidade de detectar patologias
- **Especificidade**: Capacidade de identificar casos normais
- **F1-Score**: Média harmônica entre precisão e recall
- **Validação Cruzada**: Avaliação robusta do modelo
- **Score ICBHI**: Métrica específica do desafio

## 📚 Literatura

1. **Ausculta Pulmonar: Técnica e Importância**  
   Explica os principais tipos de sons respiratórios e sua importância clínica.  
   [Link para o artigo](https://med.estrategia.com/portal/conteudos-gratis/procedimentos/resumo-de-ausculta-pulmonar-tecnica-sons-e-muito-mais/)

2. **Análise de Sons Pulmonares com Wavelets e Entropia**  
   Uso de Wavelet Packet e entropia de Shannon na classificação de sons respiratórios.  
   [Link para o artigo](https://canal6.com.br/cbeb/2014/artigos/cbeb2014_submission_052.pdf)

3. **RespireNet: Detecção de Sons Pulmonares Anormais com Redes Neurais**  
   Rede neural convolucional simples com bom desempenho mesmo com poucos dados.  
   [Link para o artigo](https://arxiv.org/abs/2011.00196)

4. **CNN-MoE Framework para Classificação de Anomalias Respiratórias**  
   Arquitetura baseada em espectrogramas com desempenho superior em benchmarks.  
   [Link para o artigo](https://arxiv.org/abs/2004.04072?)

5. **Coswara: Banco de Dados de Sons Respiratórios para Diagnóstico de COVID-19**  
   Projeto colaborativo que coleta sons respiratórios, de tosse e fala para diagnóstico.  
   [Link para o artigo](https://arxiv.org/abs/2005.10548?)
