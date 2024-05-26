# Cryptography Protocol

Most secure sharing protocols necessitate multi-round peer-to-peer communication, posing challenges particularly when dealing with models containing billions of parameters, where completing such communication in a reasonable timeframe becomes impractical.

To address this issue, optimization on protocols are essential, notably focusing on garbled-circuites MPC protocols\cite{beerliova2008perfectly, maestre2009distributed}. A key optimization strategy involves the design of compilers tailored to generate fewer garbled-circuit gates, thereby reducing the size of data transmissions and alleviating the burden on network communication. However, by far, there is no practical method applied to large models.
