# Variational-autoencoders-for-implied-volatility-surfaces-completion

Market data of non-liquid options is often incomplete. This project suggests a method based
on variational autoencoders inspired by ergeron et al’s research paper [[1]](#1) to complete missing
points on partially observed volatility surfaces without introducing static arbitrage. After
drawing a parallel between autoencoders and principal component analysis, we compare our
new variational autoencoder architecture to the architecture proposed in [[1]](#1). and we show its
utility in completing and generating arbitrage-free equity volatilities.

## References

Bergeron, M., Fung, N., Hull, J., Poulos, Z., and Veneris, A. Variational
autoencoders: A hands-off approach to volatility, 2022.
