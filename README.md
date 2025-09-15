
### Hipóteses de Pesquisa

**H1**: **Maior tempo de tela à noite** (uso prolongado de redes sociais antes de dormir) está associado a **pior qualidade do sono**.

* Variáveis envolvidas:

  * `redes_horas` (tempo de redes sociais por dia)
  * `redes_antes_dormir` (uso até 2h antes de dormir)
  * `sono_qualidade` (percepção de sono leve/agitado)
  * `pontuacao` (caso seja uma escala de qualidade)



**H2**: **Uso de redes sociais após as 22h** eleva a probabilidade de apresentar **pior escore de sono**.

* Variáveis envolvidas:

  * `redes_antes_dormir` (proxy para uso após 22h)
  * `sono_horas` (duração média do sono)
  * `sono_tempo_adormecer` (latência do sono)
  * `pontuacao`



**H3**: **Fatores de confusão** (idade, trabalho, exercício físico, consumo de café/energéticos) modulam a relação entre tempo de tela e qualidade do sono.

* Variáveis de controle:

  * `idade`
  * `trabalho_modalidade` e `trabalho_horas`
  * `exercicio_freq`
  * `cafe_apos_18h`



### Estrutura para análise estatística:

* **H1** → Correlação (Pearson/Spearman) entre `redes_horas`/`redes_antes_dormir` e `sono_qualidade`/`pontuacao`.
* **H2** → Teste de diferença de médias (t-test ou Mann-Whitney) entre grupos (usa vs. não usa após 22h).
* **H3** → Regressão logística ou linear múltipla, incluindo fatores de confusão como variáveis independentes.


