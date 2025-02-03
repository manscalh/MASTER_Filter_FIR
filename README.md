# Projeto de Filtros FIR para Remoção de Ruído em Áudio

Este projeto demonstra a aplicação de filtros FIR (Finite Impulse Response) para remover ruído de um sinal de áudio. São utilizados diferentes tipos de janelas para projetar os filtros e comparar sua eficiência na redução do ruído, avaliada pela métrica SNR (Signal-to-Noise Ratio).

## Etapas do Projeto

1. **Carregamento e Visualização dos Dados:**

   - Carregamento dos arquivos de áudio: sinal limpo, sinal com ruído e ruído.
   - Normalização dos sinais para evitar distorções.
   - Exibição dos sinais de áudio original e com ruído no domínio do tempo.
   - Plotagem dos sinais no domínio do tempo para visualizar a contaminação por ruído.


2. **Análise no Domínio da Frequência:**

   - Cálculo da Transformada de Fourier dos sinais (limpo e com ruído) para visualizar os componentes de frequência.
   - Plotagem do espectro de frequência do sinal com ruído, mostrando as frequências presentes e a intensidade do ruído.
   - Comparação visual entre o espectro de frequência do sinal original e do sinal com ruído.


3. **Filtragem com Filtros FIR de Alta Passagem:**
   - Implementação de filtros FIR de alta passagem com diferentes janelas (Retangular, Triangular, Hanning, Hamming, Blackman).
   - Aplicação de cada filtro no sinal com ruído.
   - Cálculo do SNR original e do SNR após a filtragem para cada janela.
   - Plotagem do espectro de frequência do sinal filtrado, comparando com o espectro do sinal original e sinal com ruído.
   - Plotagem do sinal filtrado no domínio do tempo.
   - Salvar os sinais filtrados para cada janela em arquivos wav.
   - Reprodução do áudio original com ruído e os áudios filtrados.
   - Exibição da tabela de resultados com o SNR para cada tipo de janela.


4. **Filtragem com Filtros FIR de Passa-Banda:**
   - Processo similar ao passo 3, mas utilizando filtros FIR de passa-banda, para um determinado intervalo de frequências.
   - Os resultados (SNR, gráficos, áudio) são exibidos e salvos de forma semelhante ao passo anterior.


5. **Filtragem com Filtros FIR de Rejeição de Banda:**

    - Processo similar aos anteriores, mas desta vez com filtros FIR de rejeição de banda.
    - A finalidade é remover uma faixa de frequência específica onde o ruído é mais predominante.
    - Geração dos espectros, tabelas, e reprodução do áudio resultante.


6. **Comparação e Ranking:**
    - Comparação das diferentes janelas usadas em cada tipo de filtro baseado na melhora do SNR.
    - Ranking das janelas, indicando a mais eficiente para cada tipo de filtro baseado na melhoria de SNR.

## Resultados

Os resultados mostram a eficácia das diferentes janelas na redução do ruído, com algumas janelas apresentando melhores resultados que outras. 

O ranking da eficiência das janelas é exibido no final do notebook, indicando quais janelas geraram a maior melhora no SNR para cada tipo de filtro.
