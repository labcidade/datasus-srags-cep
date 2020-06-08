Hospitalizações por Síndrome Respiratória Aguda Grave na RMSP
============
*Dados e documentação produzidos pelo Laboratório Espaço Público e Direito à Cidade da Faculdade de Arquitetura e Urbanismo da Universidade de São Paulo - [LabCidade FAUUSP](http://www.labcidade.fau.usp.br/)*

**Equipe:** Pedro Mendonça
**Financiamento:** Fundação Ford
**Data:** 28/05/2020, atualização não prevista
**Licença de compartilhamento:** CC Atribuição (CC BY 3.0 BR) (ver arquivo LICENÇA.txt)

## Conteúdo
Hospitalizações por Síndrome Respiratória Aguda Grave (SRAG), inclusive Covid-19, na Região Metropolitana de São Paulo, de 23/02 a 18/05/2020, georreferenciadas por CEP e heatmaps de estimativa de densidade kernel e agregados por quinzena 

São parte deste conjunto de dados:

    DATASUS_SRAGs_CEP_18-05.dbf
    DATASUS_SRAGs_CEP_18-05.shp
    DATASUS_SRAGs_CEP_18-05.shx
    DATASUS_SRAGs_CEP_18-05.cpg
    DATASUS_SRAGs_CEP_18-05.prj
    Q5_HC.tif
    Q5_HS.tif
    Q5_HT.tif
    CUM_HC_Q5.tif
    Q6_HC.tif
    Q6_HS.tif
    Q6_HT.tif
    CUM_HC_Q6.tif
    Q7_HC.tif
    Q7_HS.tif
    Q7_HT.tif
    CUM_HC_Q7.tif
    Q8_HC.tif
    Q8_HS.tif
    Q8_HT.tif
    CUM_HC_Q8.tif
    Q9_HC.tif
    Q9_HS.tif
    Q9_HT.tif
    CUM_HC_Q9.tif
    Q10_HC.tif
    Q10_HS.tif
    Q10_HT.tif
    CUM_HC_Q10.tif
    TOT_HC.tif
    TOT_HS.tif
    TOT_HT.tif
    TOT_OC.tif
    TOT_OS.tif
    TOT_OT.tif

## Metodologia
Os casos de hospitalização foram selecionados no banco de dados sobre SRAG no DataSUS, a partir da data do primeiro sintoma de Covid-19 (23/02). Os dados foram agregados para casos confirmados de Covid-19, outros registros de SRAG e para o total de hospitalizações. Esses valores foram agregados por CEP e ponderados por comprimento dos logradouros a partir de dados do Centro de Estudos da Metrópole, separando as ruas cujos lados têm CEPs distintos em alinhamentos únicos. Os resultados tabulares foram unidos ao shapefile de logradouros com CEP, resultando em geometrias lineares. Para criação dos heatmaps de estimativa de densidade kernel, foram interpolados pontos equidistantes sobre as linhas de CEP. Foi utilizada uma função kernel gaussiana com raio de 1 quilômetro.

Como o georreferenciamento depende de CEPs específicos por logradouro, excluímos os municípios da RMSP com CEP único. Foram mantidos os municípios de Barueri, Carapicuíba, Cotia, Diadema, Embu das Artes, Ferraz de Vasconcelos, Francisco Morato, Franco da Rocha, Guarulhos, Itapecerica da Serra, Itapevi, Itaquaquecetuba, Jandira, Mauá, Mogi das Cruzes, Osasco, Poá, Ribeirão Pires, Santana de Parnaíba, Santo André, São Bernardo do Campo, São Caetano do Sul, São Paulo, Suzano e Taboão da Serra. 


## Finalidade
Acompanhamento de políticas públicas relacionadas à pandemia de Covid-19

## Dados externos
- [DataSUS](https://opendatasus.saude.gov.br/dataset/bd-srag-2020)
- [Centro de Estudos da Metrópole](http://centrodametropole.fflch.usp.br/pt-br/download-de-dados?f%5B0%5D=facets_temas%3Asistema%20viario)
