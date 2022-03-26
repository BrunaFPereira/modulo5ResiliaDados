<h1 align="center">Análise Exploratória de Gastos dos Deputados Federais</h1>

## Introdução
&nbsp; Este notebook trabalha com dados referentes a **Cota para o Exercício da Atividade Parlamentar** de um total de **846 deputados**, incluindo **829 parlamentares** e **17 lideranças**. <br><br>
&nbsp;A CEAP é uma cota única mensal que é destinada ao custeio de gastos vinculados ao exercício da atividade parlamentar pelos deputados. Seu limite varia por estado. <br>
* Primeiro, filtrando e examinando os dados, foram verificados e corrigidos os seguintes problemas como: informações faltantes, inconsistências na formatação dos registros e títulos despadronizados. <br>
* Por fim, foram feitas as visualizações, investigações e aprofundamentos incluídos nos objetivos.

## Dados
Os *datasets* utilizados nesse notebook referentes a **Cota para Exercício da Atividade Parlamentar** foram extraídos da [Câmara dos Deputados](https://www2.camara.leg.br/transparencia/cota-para-exercicio-da-atividade-parlamentar/dados-abertos-cota-parlamentar), assim como o [dicionário de variáveis](https://www2.camara.leg.br/transparencia/cota-para-exercicio-da-atividade-parlamentar/explicacoes-sobre-o-formato-dos-arquivos-xml).

## Objetivos
[Confira a rubrica do projeto.](https://github.com/Viltoncio/modulo5ResiliaDados/blob/942ef3e88f0f6b64b68c84e74796c371fa4e0452/Documentos/Analise_de_Gastos_dos_Deputados_Federais.pdf)

## Análise dos Dados
* [Importação dos Dados.](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=Importa_o_dos_Dados)
* [Verificando a Integridade dos Dados.](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=An_lise_dos_Dados)
* [Tratamento e Normalização dos Dados.](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=Tratamento_e_normaliza_o_dos_dados)
* [Gerando um Relatório Geral dos Dados.](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=Gerando_um_relat_rio_geral_dos_dados)

### Questões
* [Resolvendo Questões Predefinidas](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=Resolvendo_Quest_es_Predefinidas)
 * 1. [Como se comportam os gastos com cotas parlamentares ao longo do tempo? Existe alguma tendência de aumento ou redução desse custo?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=1_Como_se_comportam_os_gastos_com_cotas_parlamentares_ao_longo_do_tempo_Existe_alguma_tend_ncia_de_aumento_ou_redu_o_desse_custo_)
 * 2. [Qual a média de gastos por parlamentar?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=2_Qual_a_m_dia_de_gastos_por_parlamentar_)
 * 3. [Quais foram os parlamentares que mais e que menos consumiram recursos?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=3_Quais_foram_os_parlamentares_que_mais_e_que_menos_consumiram_recursos_)
 * 4. [Quais são as categorias de despesas mais onerosas dentre os recursos destinados às cotas parlamentares?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=4_Quais_s_o_as_categorias_de_despesas_mais_onerosas_dentre_os_recursos_destinados_s_cotas_parlamentares_)
 * 5. [Quais são os trechos de viagem mais recorrentes entre as despesas de viagem?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=5_Quais_s_o_os_trechos_de_viagem_mais_recorrentes_entre_as_despesas_de_viagem_)
 * 6. [Qual a média de gastos por estado?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=6_Qual_a_m_dia_de_gastos_por_estado_)
 * 7. [Qual é o valor total de gastos por estado?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=7_Qual_o_valor_total_de_gastos_por_estado_)
 * 8. [Quais estados têm maior número de representantes?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=8_Quais_estados_t_m_maior_n_mero_de_representantes_)
 * 9. [Há alguma correlação entre a quantidade de parlamentares por estado e o valor total dos gastos?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=9_H_alguma_correla_o_entre_a_quantidade_de_parlamentares_por_estado_e_o_valor_total_dos_gastos_)
 * 10. [Qual a média de gastos por partido?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=10_Qual_a_m_dia_de_gastos_por_partido_)
 * 11. [Quais são os partidos que mais e que menos consumiram a cota parlamentar?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=11_Quais_s_o_os_partidos_que_mais_e_que_menos_consumiram_a_cota_parlamentar_)
 * 12. [Há alguma correlação entre a quantidade de parlamentares por partido e o valor total dos gastos?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=12_H_alguma_correla_o_entre_a_quantidade_de_parlamentares_por_partido_e_o_valor_total_dos_gastos_)
* [Questões Extras](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=Aprofundamentos_Quest_es_Extras_)
 * 1. [Extra: Como os resultados obtidos se relacionam com os limites permitidos por Estado?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=1_Como_os_resultados_obtidos_se_relacionam_com_os_limites_permitidos_por_Estado_)
 * 2. [Extra: Quais Lideranças tiveram mais gastos ao longo do tempo?](https://colab.research.google.com/drive/1Wu2AiQivAIBMHlUvtdok33ZEnsUtjf67#scrollTo=2_Quais_Lideran_as_tiveram_mais_gastos_ao_longo_do_tempo_)

## Referências Bibliográficas
*   [Informações e legislação sobre as cotas para o exercício da atividade parlamentar.](https://www2.camara.leg.br/transparencia/acesso-a-informacao/copy_of_perguntas-frequentes/cota-para-o-exercicio-da-atividade-parlamentar)
*   [Líder Partidário.](https://www2.camara.leg.br/comunicacao/assessoria-de-imprensa/guia-para-jornalistas/lider)

## Colaborações
<p align="left">
    Vitor Antunes <br>
    GitHub: <a href="https://github.com/Viltoncio">Viltoncio</a>
</p>
 
<p align="left">
    Pedro André <br>
    GitHub: <a href="https://github.com/pedroandre1712">pedroandre1712</a>
</p>
 
<p align="left">
    Samyr Ozibel <br>
    GitHub: <a href="https://github.com/ozibel">ozibel</a>
</p>
 
<p align="left">
    Bruna Pereira <br>
    GitHub: <a href="https://github.com/BrunaFPereira">BrunaFPereira</a>
</p>
      
<p align="left">
    Jônatas Hessel <br>
    GitHub: <a href="https://github.com/JonatasHesselTaveira">JonatasHesselTaveira</a>
</p>     
