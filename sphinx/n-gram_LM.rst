N-gram Language Modelling
=========================

**Sample Corpus**:
 | This is **the house** that Jack built.
 | This is **the** malt
 | That lay in **the house** that Jack built.
 | This is **the** rat,
 | That ate **the** malt
 | That lay in **the house** that Jack built.
 | This is **the** cat,
 | That killed **the** rat,
 | That ate **the** malt
 | That lay in **the house** that Jack built.

What is the probability of **house** occurring given **the** before it?

Intuitively, we count,
    .. role:: raw-latex(raw)
        :format: latex html

    .. raw:: html

       <script type="text/javascript" src="http://localhost/mathjax/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

    :raw-latex:`\(Prob\,({ house \over the }) = { Count\,( the\,house ) \over Count\,(the) } \)`

Mathematically, the above formula can be writen as :raw-latex:`\(P({ B \over A }) = { P( A,\,B ) \over \,P(B) } \)`

What we have computed above is a **Bigram Language Model**:

:math:`Bigram\:Model : { p\,( W{t}|W{t-1} ) }`

**How do ngrams help us calculate the prob of a sentence?**:
 |  Sentence, S = 'A B'
 |  We know that, probability of this sentence 'A B' as,
 |  P (S) = Prob (A before B) = P(A , B) = Joint Probability of A and B = **P(B|A)* P(A)**
 |
 |  Let us assume a three word sentence, S = 'A B C'
 |  P(S) = Prob (A before B before C ) = P (A , B , C)
 |       = P(C | A , B) * P (A n B)
 |       = P (C| A , B) * P(B | A) * P (A)
 |
Even if there are more words, we could keep applying Conditional Probability and compute the prob of a sentence.
The above rule is called **`Chain Rule of Probability`**
    :raw-latex:`(P (
    :raw-latex:`\(Prob\,({ house \over the }) = { Count\,( the\,house ) \over Count\,(the) } \)`



