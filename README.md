<h1 align="center">Awesome 3D Face Reconstruction (Kor.)</h1>

<p align="center" style="font-size:small">주요한 논문을 한 줄로 정리합니다.</p>

## Papers
<p style="font-size:small">시간 역순 정렬</p>

**[RingNet]() (Sanyal et al., CVPR 2019)**<br>
Learning to Regress 3D Face Shape and Expression from an Image without 3D Supervision<br>
*Soubhik Sanyal, Timo Bolkart, Haiwen Feng and Michael J. Black*<br>
NoW benchmark를 함께 제안.

**[3DMM](https://dl.acm.org/doi/10.1145/311535.311556) (Blanz et al., 1999)**<br>
A morphable model for the synthesis of 3d faces<br>
*Volker Blanz, Thomas Vetter*<br>
*SIGGRAPH 1999*
<details>
    <summary>사람의 3D 모델링 방법으로, shape & texture를 vector space에서 표현하며, bases의 linear combination으로 표현 가능.</summary>

    $$
    \mathbf{S} = \mathbf{S}(\boldsymbol{\alpha, \beta}) = \bar{\mathbf{S}} + \mathbf{S}_{id} \boldsymbol{\alpha} + \mathbf{S}_{exp} \boldsymbol{\beta}
    $$
</details>
