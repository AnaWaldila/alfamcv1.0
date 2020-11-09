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

## Methodology

All methodology can see in REIS et al (2017) and BAZANT (1984).

## About the Software

AlfaMCV (Momento Curvature em Vigas de Concreto Armado, i.e, Curvature Moment in Reinforced Concrete Beams, in Portuguese), is a simple software where exists an interations between the programn and the user, i.e, exists a GUI interface. The software was developed with Visual Basic computational language and was used Microsoft Visual Studio 2017 platform. The software is in Portuguese.
The software shows a principal window where are presented four buttons: "Calcular" (Calculus), "Sobre o Software" (About the Software), "Ajuda" (Help) and "Sair" (Exit), like Figure 4.

<div>
<img src="Figures/Alfa_Principal.png" width="40%">
</div>
<p>
 <b>Figure 4:</b> AlfaMCV - Principal Window (Reis et al, 2017)
</p>

The button "Calcular" (Calculus) open a new window, where the user can input data about the structure phisics-geometrics characteristics. There are necessaire: "Altura Total - H (cm)" (total height H, cm), "Altura Útil Total - d (cm)" (total useful height d, cm), "Largura - B (cm)" (width B, cm), "Vão (cm)" (beam length, cm), "Resistencia à Compressão do Concreto - f<sub>ck</sub> (MPa)" (concrete compression resistence - f<sub>ck</sub> MPa), "Resistencia à Tração do Concreto - f<sub>tk</sub> (MPa)" (concrete tension resistence f<sub>ck</sub> MPa), "Modulo de Elasticidade do Concreto (MPa)" (concrete's Young Moduli MPa), "Área de Aço de Compressão - A'<sub>s</sub> (cm²)" (steel compression area A'<sub>s</sub>, cm²), "Área de Aço de Tração - A<sub>s</sub> (cm²)" (steel tension area A<sub>s</sub>, cm²), "Módulo de Elasticidade do Aço - Es (MPa)" (steel Young Moduli MPa) and "Escoamento do Aço - f<sub>y</sub> (MPa)" (yield steel f<sub>y</sub> MPa). All those characteristics can see in Figure 5.

<div>
<img src="Figures/Alfa_Calculus.png" width="80%">
</div>
<p>
 <b>Figure 5:</b> AlfaMCV - Calculus Window (Reis et al, 2017)
</p>

After input data, a new window is opened with all informations about the structure. The first tab "Regime Linear" (Linear Behavior), presents some informations about the structure, like "Altura da Linha Neutra (cm)" (neutral axis height, cm), "Deformação de Tração Máxima do Concreto" (maximum concrete tension strain), "Deformação de Compressão Correspondente à Tração Máxima" (concrete strain in compression when maximum tension is obtained), "Deformação de Compressão Máxima do Concreto" (maximum concrete compression strain), "Deformação do Aço de Tração" (steel tension strain)
