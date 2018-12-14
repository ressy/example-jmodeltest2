# jModelTest2 Examples

## Assortment of Reference Information

 * Original Paper: <https://academic.oup.com/mbe/article/25/7/1253/1045159>
 * Version 2 Paper: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4594756/>
 * Example exercise, but with broken data link: <http://evomics.org/learning/phylogenetics/jmodeltest/>
 * Code Repository: <https://github.com/ddarriba/jmodeltest2>
 * Some documentation: <https://drive.google.com/drive/u/0/folders/0ByrkKOPtF_n_OUs3d0dNcnJPYXM>

Glossary of model names and suffixes found in Table 1 in [jModelTest 2 manual]
PDF, plus links to Wikipedia's entry and publications where I could find them:

Model  | Wikipedia  | Reference                | Free param. | Base freq. | Substitution rates | Substitution code |
 ----- | ---------- | ------------------------ | ----------- | ---------- | ------------------ | ----------------- |
JC     | [JC69]     | [Jukes and Cantor, 1969] | 0           | equal      | AC=AG=AT=CG=CT=GT  | 000000            |
F81    | [F81]      | [Felsenstein, 1981]      | 3           | unequal    | AC=AG=AT=CG=CT=GT  | 000000            |
K80    | [K80]      | [Kimura, 1980]           | 1           | equal      | AC=AT=CG=GT;AG=GT  | 010010            |
HKY    | [HKY85]    | [Hasegawa et al., 1985]  | 4           | unequal    | AC=AT=CG=GT;AG=GT  | 010010            |
TrNef  | [T93]      | [Tamura and Nei, 1993]   | 2           | equal      | AC=AT=CG=GT;AG;GT  | 010020            |
TrN    | [T93]      | [Tamura and Nei, 1993]   | 5           | unequal    | AC=AT=CG=GT;AG;GT  | 010020            |
TPM1   | ???        | =K81 [Kimura, 1981]      | 2           | equal      | AC=GT;AG=CT;AT=CG  | 012210            |
TPM1uf |            | [Kimura, 1981]           | 5           | unequal    | AC=GT;AG=CT;AT=CG  | 012210            |
TPM2   |            |                          | 2           | equal      | AC=AT;CG=GT;AG=CT  | 010212            |
TPM2uf |            |                          | 5           | unequal    | AC=AT;CG=GT;AG=CT  | 010212            |
TPM3   |            |                          | 2           | equal      | AC=AT;AG=GT;AG=CT  | 012012            |
TPM3uf |            |                          | 5           | unequal    | AC=CG;AT=GT;AG=CT  | 012012            |
TIM1   | ???        | [Posada, 2003]           | 3           | equal      | AC=GT;AT=CG;AG;CT  | 012230            |
TIM1uf |            | [Posada, 2003]           | 6           | unequal    | AC=GT;AT=CG;AG;CT  | 012230            |
TIM2   |            |                          | 3           | equal      | AC=AT;CG=GT;AG;CT  | 010232            |
TIM2uf |            |                          | 6           | unequal    | AC=AT;CG=GT;AG;CT  | 010232            |
TIM3   |            |                          | 3           | equal      | AC=CG;AT=GT;AG;CT  | 012032            |
TIM3uf |            |                          | 6           | unequal    | AC=CG;AT=GT;AG;CT  | 012032            |
TVMef  | ???        | [Posada, 2003]           | 4           | equal      | AC;CG;AT;GT;AG=CT  | 012314            |
TVM    |            | [Posada, 2003]           | 7           | unequal    | AC;CG;AT;GT;AG=CT  | 012314            |
SYM    | ???        | [Zharkikh, 1994]         | 5           | equal      | AC;CG;AT;GT;AG;CT  | 012345            |
GTR    | [GTR]      | =REV [Tavare, 1986]      | 8           | unequal    | AC;CG;AT;GT;AG;CT  | 012345            |

[jModelTest 2 manual]: https://drive.google.com/drive/u/0/folders/0ByrkKOPtF_n_OUs3d0dNcnJPYXM

[JC69]:  https://en.wikipedia.org/wiki/Models_of_DNA_evolution#JC69_model_(Jukes_and_Cantor_1969)
[F81]:   https://en.wikipedia.org/wiki/Models_of_DNA_evolution#F81_model_(Felsenstein_1981)
[K80]:   https://en.wikipedia.org/wiki/Models_of_DNA_evolution#K80_model_(Kimura_1980)
[HKY85]: https://en.wikipedia.org/wiki/Models_of_DNA_evolution#HKY85_model_(Hasegawa,_Kishino_and_Yano_1985)
[T93]:   https://en.wikipedia.org/wiki/Models_of_DNA_evolution#TN93_model_(Tamura_and_Nei_1993)
[GTR]:   https://en.wikipedia.org/wiki/Models_of_DNA_evolution#GTR_model_(Tavar%C3%A9_1986)

[Tavare, 1986]:          http://www.damtp.cam.ac.uk/user/st321/CV_%26_Publications_files/STpapers-pdf/T86.pdf
[Kimura, 1980]:          https://doi.org/10.1007/BF01731581
[Kimura, 1981]:          https://www.ncbi.nlm.nih.gov/pmc/articles/PMC319072/
[Felsenstein, 1981]:     https://doi.org/10.1007/BF01734359
[Hasegawa et al., 1985]: https://www.ncbi.nlm.nih.gov/pubmed/3934395
[Zharkikh, 1994]:        https://www.ncbi.nlm.nih.gov/pubmed/7932793
[Posada, 2003]:          https://doi.org/10.1002/0471250953.bi0605s00

Possible suffixes on model names:
 * "+I": with invariable sites
 * "+G": with rate variation among sites
 * "+I+G": with both

Other acronyms and abbreviations:

 * AIC: Akaike Information Criterion
 * AICc: Akaike Information Criterion, corrected
 * BIC: Bayesian Information Criterion
 * DT: Decision Theory (criterion)
 * -lnL: negative log likelihood
