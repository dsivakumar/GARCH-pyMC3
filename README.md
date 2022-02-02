# GARCH-pyMC3
GARCH model introduced by Engle (1982) and Bollerslev (1986)
</br>
y<sub>t</sub> ∼ N (0, σ2 <sub>t</sub>)
</br>
σ<sup>2</sup>
<sub>t</sub> = α<sub>0</sub>+ α<sub>1</sub>y
<sup>2</sup>
<sub>t−1</sub> + βσ<sup>2</sup>
<sub>t−1</sub>
</br>
where σ<sup>2</sup><sub>t</sub> is the conditional variance at time t, y<sub>t</sub> is the (de-filtered) log-return at time t
</br>
Parameter constraints: α<sub>0</sub> > 0, α<sub>1</sub> + β < 1 and  α<sub>0</sub> + α<sub>1</sub> + β < 1
</br>
I searched for a pyMC3 implementation but didn't come across any, ad no coice but try my hands. </br>
Then I came across a STAN implementation http://blackwell.math.yorku.ca/MATH6635/2016/stan-reference-2.12.0.pdf that helped in putting together this notebook.
Please check
