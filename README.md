# breath2vision
A computer vision project for detecting respiratory diseases using spectrograms of lung sounds and deep learning models.

## Seção I. Introdução e Revisão Bibliográfica

### Problema

O diagnóstico de doenças respiratórias, como asma, pneumonia e DPOC, frequentemente depende da ausculta pulmonar realizada por profissionais de saúde. No entanto, essa prática é subjetiva e requer experiência significativa para identificar sons anormais, como sibilos e estertores. Além disso, em áreas com acesso limitado a especialistas, o diagnóstico pode ser atrasado ou impreciso.

Com o avanço da tecnologia, surge a oportunidade de aplicar visão computacional para analisar sons respiratórios, transformando-os em representações visuais (espectrogramas) que podem ser interpretadas por algoritmos de aprendizado de máquina, visando uma detecção mais objetiva e acessível de doenças respiratórias.

---

### Literatura

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

---

### Dataset

Será utilizado o **ICBHI 2017 Respiratory Sound Database**, que contém 6.898 ciclos respiratórios de 126 pacientes, incluindo sons normais e patológicos (sibilos e estertores), relacionados a diversas doenças respiratórias.

- [Mais informações sobre o ICBHI Dataset](https://www.researchgate.net/figure/ICBHI-respiratory-database-comprised-of-LS-from-various-pulmonary-pathologies_fig4_345978905?)
- Exemplo de dados no dataset
![image](https://github.com/user-attachments/assets/53cb0b9a-ae19-465f-a503-7974d8a6dcb4)


---

### Métodos

O projeto utilizará as seguintes abordagens:

- **Transformada Wavelet Packet**: para decomposição dos sinais e extração de características.
- **Espectrogramas**: conversão dos sinais de áudio em imagens para entrada em redes neurais.
- **Redes Neurais Convolucionais (CNNs)**: para classificar os espectrogramas.
- **Modelos como RespireNet**: otimizados para conjuntos de dados pequenos.

---

### Avaliação

A performance dos modelos será avaliada por meio de:

- **Métricas**: Acurácia, Sensibilidade, Especificidade, F1-score.
- **Validação cruzada**: com técnica de *k-fold* para melhor robustez.
- **Benchmarks**: comparação com resultados de referência como os do desafio ICBHI 2017.

---
