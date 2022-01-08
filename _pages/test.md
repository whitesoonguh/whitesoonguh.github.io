---
title: "Interest"
layout: splash
classes: wide
author_profile: false
permalink: /Interest/
excerpt: 'Interesting Cryptography!'
header:
  overlay_image: /assets/images/seoul.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
---

<details open>
    <summary style="font-size:1.2rem; font-weight:bold;">
        Verifiable Computation
    </summary>
    <br>
    <p>In page of "Verifiable computing" of wikipedia, Verifiable computing (or verified computation or verified computing) enables a computer to offload the computation of some function, to other perhaps untrusted clients, while maintaining verifiable results. The other clients evaluate the function and return the result with a proof that the computation of the function was carried out correctly. The introduction of this notion came as a result of the increasingly common phenomenon of "outsourcing" computation to untrusted users in projects such as <A href="https://en.wikipedia.org/wiki/SETI@home">SETI@home</A> and also to the growing desire of weak clients to outsource computational tasks to a more powerful computation service like in cloud computing.</p>
    <details>
        <summary>
            What is the NIZK?
        </summary>
        Interactive Proofs (IPs) and Arguments
        <ul type="square">
            <li><p>Prover <i>P</i> and Verfier <i>V</i><br>
                1. <i>P</i> solves a problem on a given input.<br>
                2. Tells <i>V</i> the answer.<br>
                3. Then <i>P</i> proves to <i>V</i> that the answer is correct.</p>
                <ul type="none">
                    <li><p>Requirements:<br>
                        <u>Completeness</u>: If the answer is true, the honest <i>V</i> will be convinced of this fact by an untrusted <i>P</i> (honest <i>P</i> in ZKP).<br>
                        <u>Soundness</u>: If the answer is false, no <i>P</i> (no cheating <i>P</i> in ZKP) can convince the honest <i>V</i> that it is true, except with some small probability.</p>
                    </li>
                </ul>
            </li>
            <li><p>Difference of IPs and Arguments<br>
                The difference is that the prover is restricted to be a polynomial-time algorithm for an interactive arguement, whereas no such restrictions on the prover apply for an interactive proof.</p>
            </li>
        </ul>
        Zero-Knowledge Proof (ZKP) and Non-Interactive Proofs
        <ul type="square">
            <li><p>Zero-Knowledge Proof<br>
                ZKP is one of the IPs and is a method by which <i>P</i> can prove to <i>V</i> that they know a secret, without conveying any information apart from the fact that they know the secret.<br></p>
                <ul type="none">
                    <li><p>More requirement for ZKP:<br>
                        <u>Zero-knowledge</u>: If the answer is true, no <i>V</i> learns anything other than the fact that the answer is true.</p>
                    </li>
                </ul>
            </li>
            <li><p>Non-Interactive Proofs<br>
                Non-Interactive Proofs require no interaction between the <i>P</i> and <i>V</i>.</p>
            </li>
        </ul>
        Therefore, Non-interactive zero-knowledge proofs (also known as NIZK, zk-SNARK) are zero-knowledge proofs that require no interaction between the <i>P</i> and <i>V</i>.
    </details>
</details>

<br>

<details open>
    <summary style="font-size:1.2rem; font-weight:bold;">
        Secure Machine Learning (Cryptographic Approach)
    </summary>
    <br>
    <p>With the successful development of deep learning, biometric authentication technology based on convolutional neural networks has remarkably advanced.<br>
    <A href="https://arxiv.org/abs/1801.07698/">ArcFace</A> based on <A href="https://arxiv.org/abs/1512.03385">Residual neural network</A>, one of the convolutional neural networks, is the recent state-of-the-art face recognition system and outputs highly discriminative feature templates for face authentication using additive angular margin loss.<br>
    However, when face recognition system become able to compress well into feature template from face image more and more, leakage of face templates is more serious threat to user privacy. For example, face images can be reconstructed from face feature templates using <A href="https://arxiv.org/abs/1703.00832">neighborly de-convolutional neural network</A> and this is serious threat to user privacy.</p>
    Therefore we develop a modular architecture <A href="https://openaccess.thecvf.com/content/CVPR2021/html/Kim_IronMask_Modular_Architecture_for_Protecting_Deep_Face_Template_CVPR_2021_paper.html">Ironmask</A> for protecting face feature templates that can be combined with any face recognition system that using angular distance metric such as <A href="https://arxiv.org/abs/1704.08063">SphereFace</A>, <A href="https://arxiv.org/abs/1801.09414">CosFace</A>, <A href="https://arxiv.org/abs/1801.07698">ArcFace</A>.
    <br>
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/CVPR.jpg" alt="">
</details>

<br>

<details open>
    <summary style="font-size:1.2rem; font-weight:bold;">
        Functional Encryption
    </summary>
    <br>
    <p>Functional Encryption (FE) is a new public key encryption system that extends the existing public key encryption concept more flexibly. It is a public key encryption that allows the decryption condition of a cipher text to be specified as an arbitrary function. At this time, Functional Encryption guarantees complete privacy by not exposing unnecessary information related to the cipher text to not only system outsiders but also system insiders.<br>
    The purpose of ongoing research (Research on Functional Encryption Technique Design, Analysis and Implementation Technology, supported by IITP) is to obtain the important source technologies of FE that is considered to be next-generation public-key encryption and to study the extended technologies of FE for cloud computing. In addition, this research studies techniques of other cryptographic primetives like Lattices.</p>
    
</details>