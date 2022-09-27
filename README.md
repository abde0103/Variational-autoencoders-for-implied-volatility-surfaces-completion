# Variational-autoencoders-for-implied-volatility-surfaces-completion

Market data of non-liquid options is often incomplete. This project suggests a method based
on variational autoencoders inspired by Bergeron et al’s research paper [[1]](#1) to complete missing
points on partially observed volatility surfaces without introducing static arbitrage. After
drawing a parallel between autoencoders and principal component analysis, we compare our
new variational autoencoder architecture to the architecture proposed in [[1]](#1). and we show its
utility in completing and generating arbitrage-free equity volatilities.

This document covers my work during the first two months of my six-month internship
at Marex Solutions in London. In this report, I studied in-depth the ability of variational
autoencoders to reproduce implied volatility surfaces without creating any static arbitrage.
In this work, I suggested a new variational autoencoder architecture dedicated to learning
how to generate and complete arbitrage-free implied volatility surfaces.


**Section 1:** A brief introduction of the evolution of implied volatility models and the
emergence of deep learning in finance.\

**Section 2:** A definintion of deterministic and variational autoencoders with *a proof* that
I elaborated to show the relationship between autoencoders and principal component analysis
(PCA).\

**Section 3:** A definition of delta implied volatility surfaces and a characterization of
static arbitrage in terms of delta instead of usual characterizations in terms of log-forward
moneyness.\

**Section 4:** The data interpolation method that I opted for to have a fixed size implied
surface from listed options. A presentation of the new architecture that I suggested to improve
the results of the cited paper [[1]](#1).\

**Section 5:** All the numerical results of the new architecture and a comparison to the
results yield by Bergeron et al’ variational autoencoder architecture on our internal data sets.\

**Section 6:** Our method to complete missing points on partially observed implied volatility
surfaces on illiquid options.\

**Section 7:** A summary of our findings and ideas for further work that can be done
beyond the scope of this project.

## References
<a id="1">[1]</a> 
Bergeron, M., Fung, N., Hull, J., Poulos, Z., and Veneris, A. Variational
autoencoders: A hands-off approach to volatility, 2022.
