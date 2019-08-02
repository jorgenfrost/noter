## Logistic Regression

Use-case: Hvis vi skal forudside et outcome af en binær variable. Fx. sandsynligheden for at få udstedt et lån på baggrund af FICO-score.

### Probability og odds:

- Probability er $\frac{\text{posibilities for success}}{\text{total possibilities}}$. Fx. P(1 eller 2) med alm. terning = $\frac{2}{6} = 0.333$. 

- Odds er $\frac{p(\text{success})}{p(\text{failure})}$. Fx odds for 1 eller 2 med terning = $\frac{2/6}{4/6} = 0.333/0.666 = 0.5$

- Odds ratio:  
  $$
  \text{odds ratio} = \frac{odds_1}{odds_0} = \frac{\frac{p-1}{1-p_1}}{\frac{p_0}{1-p_0}}
  $$

- Eksempel:

  Fair coin flip: 

  - P(heads) = $\frac{1}{2} = 0.5$. 
  - odds(heads) $\frac{0.5}{0.5} = 1$
  
  Loaded coin flip:
  
  - P(heads) = $\frac{7}{10} = 0.7$. 
  - odds(heads) $\frac{0.07}{0.3} = 2.333$
  
  Odds ratio:
  
  $$
  \text{odds ratio} = \frac{\frac{.7}{.3}}{\frac{.5}{.5}} = \frac{.7}{.3} \times \frac{.5}{.5} = 2.3333
  $$



Altså:  Odds for at få heads med en loaded coin er 2.333 højere end at for at få heads med en fair coin.