# AlfaMCV Version 1.0

## Abstract

This is a software to calculate the behavior of reinforced concrete beam when it is submited a pontual load in the middle of the beam. Based on phisics-geometric structure characteristics, AlfaMCV is able to calculate some informations about the structure, when it is considering linear and nonlinear concrete in this stress-strain graphic. So, this case presents the real structure behavior. 
AlfaMCV is able to presents some informations about the structure, like: neutral axis for each step analysis, stress and strain in steel and concrete (in both cases, compression and tension), moment in the middle of the beam and their deflection.
Finally, the user is able to export the table to Excel software and create their own analysis and graphics.

## Introduction

Concrete is a weak material where the structure is calculated without the behavior of tension in concrete, i.e, only compression in concrete is considered. For the case of steel, both cases are considered, compression and tension. This region, Figure 1 shows areas where can see all efforts about concrete and steel.

<div>
<img src="Figures/Concrete_Graph.png" width="30%">
</div>
<p>
 <b>Figure 1:</b> Stress - Strain Concrete Configuration (Reis et al, 2017). 
</p>

Where A<sub>st</sub> is steel area in tension, F<sub>st</sub> is steel's force in tension, <i>&epsilon;</i><sub>cm</sub> is compression's strain in concrete, F<sub>cm</sub> is compression's force in concrete, k<sub>d</sub> is neutral axis and M<sub>k</sub> is characteristics moment.

About the compression behavior of concrete, it has well been known, like BAZANT (1984) and PFEIL (1969) presented in literature. Moreover, this type of behavior (the parabolic rectangular dyagramn) has used by NBR 6118:2014, like presents Figure 2.

<div>
<img src="Figures/Concrete_ABNT.png" width="40%">
</div>
<p>
 <b>Figure 2:</b> Stress - Strain Concrete Configuration in ABNT NBR 6118:2014 
</p>

Where f<sub>ck</sub> is the characteristic concrete compression resistence, f<sub>cd</sub> is the calculated concrete compression resistence, <i>&epsilon;</i><sub>c2</sub> is strain when concrete starts the plastic deformation and <i>&epsilon;</i><sub>cu</sub> is strain when concrete ruptures.

However, the behavior of tension in concrete is not used in design structures and studies by BAZANT (1984) presented that this area can contribute to the evolution of general structure's stifness, like Figure 3.

<div>
<img src="Figures/Concrete_Tension.png" width="30%">
</div>
<p>
 <b>Figure 3:</b> Stress - Strain Concrete Configuration in Tension (Reis et al, 2017)
</p>

Where f<sub>tk</sub> is characteristic concrete tension resistence, <i>&epsilon;</i><sub>tp</sub> is concrete strain in maximun concrete tension resistence, E<sub>c</sub> is Moduli's Young, <i>&epsilon;</i><sub>tf</sub> is concrete strain when tension stress is zero and E<sub>t</sub> is tangent Moduli.
