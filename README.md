# Crime-Rate-Econometric-Analysis

## Introudction
Understanding the factors that influence crime rates is crucial for effective crime prevention and the development of evidence-based policies. One key area of research focuses on investigating the relationship between the probabilities of apprehension and punishment and crime participation rates. By studying the deterrence effect of the criminal justice system, we can gain valuable insights into the mechanisms behind criminal decision-making and inform policy interventions aimed at reducing crime. Researching the impact of these probabilities on crime participation rates has significant implications for policy and the allocation of resources within the criminal justice system. By understanding how variations in these probabilities influence criminal behaviour, policymakers can develop targeted strategies to enhance deterrence and reduce crime rates.

## RESEARCH QUESTION: Do the probabilities of apprehension and punishment affect crime participation rate?

## Methodology
The dataset provided to us is categorised as panel data, which comprises of information on crime in 90 counties in North Carolina, for the years 1981 through 1987. We select our OLS model as follows.

Model: Ln(crmrte)= β_0+ β_1Ln(prbarr)+ β_2Ln(prbconv)+ β_3 prbpris+µ

crmrte is crimes committed per person, this is our dependent variable.

prbarr is 'probability' of arrest, directly relates to the likelihood of a person being apprehended by law enforcement. It represents the chance that an individual will be arrested for a specific offense. We take the log as the distribution is log normal hence data will be concentrated in one part leaving a long tail, we take log to make it more normal.

prbconv is 'probability' of conviction, indicates the likelihood of a person being found guilty in court. It represents the chance that someone arrested will be convicted and held legally responsible for the offense. We take the log as the distribution is log normal hence data will be concentrated in one part leaving a long tail, we take log to make it more normal.

prbpris is ‘probability' of prison sentence, represents the probability of receiving a prison sentence if convicted. It signifies the likelihood of being punished with incarceration rather than alternative forms of punishment, such as fines or probation.

We expect these independent variables to be negatively related to crime rate or in other words we expect the coefficient of these independent variables to be less than zero.

Given that the data category is panel data it is very likely that simple OLS model will suffer from problem of endogeneity caused by unobserved Heterogeneity. “The unobserved dependency of other independent variable(s) is called unobserved heterogeneity and the correlation between the independent variable(s) and the error term (i.e. the unobserved independent variabels) is called endogeneity.”

There are five assumptions in simple linear regression:

1. Linearity
2. Exogeneity
3. (a) Homoskedasticity, and (b) Non-autocorrelation
4. Independent Variable are not stochastic
5. No Multicollinearity
Two of these assumptions can help us answer if we should be using Pooled OLS or Fixed Effect Model and Random Effect Model. If assumption 2 or 3 or both are violated then Fixed Effect and Random Effect are more suitable than Pooled OLS.
