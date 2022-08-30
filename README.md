# RSVD
randomized singular value decomposition


Code to generate a randomized SVD approximation to a full SVD of a matrix H of size m by m.

This is done through the use of a matrix Omega of size m by l with random normal contents,
and the projection of H onto the orthonormal basis obtained from a QR decomposition
of a matrix Y, which is a m by l sized sketch of H.

In the calculation of the randomized SVD, we avoid using the matrix H itself
and instead use its inverse J.

For more information on the method please refer to
    Ribeiro, Yeh, and Taira arXiv 2019 and Halko, Martinsson and Tropp 2009.

For details regarding the linear algebra involved I cannot recommend
Trefethen and Bau's book highly enough.
