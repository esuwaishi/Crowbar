ワイヤーの温度を上げるために必要な熱量は、周囲へのエネルギーの損失がゼロであれば、内部エネルギーの変化に等しくなります。したがって、

$$
dq = dU = m C(T) dT
$$

ここで、$ dq $ は熱エネルギーの微小な変化、$ dU $ は内部エネルギーの微小な変化、$ m $ はワイヤーの質量、$ C(T) $ は比熱容量、そして $ dT $ は温度の微小な変化です。ここでは、ワイヤーの加熱が非常に短い時間内に行われ、システムが断熱的であると仮定しています。質量 $ m $ に $ ρ lA $ （ここで $ ρ $ は密度、$ A $ は断面積、そして $ l $ は長さ）を代入し、積分すると、式（1）は次のようになります

$$
\Delta U = \rho l A \int^{T_f}_{T_0} C(T) dT
$$

ここで、$T_0$ は周囲温度、$T_f$ はワイヤの溶融温度である。比熱容量は冪級数で近似でき、$\Delta U$はワイヤーの内部エネルギーの変化である。この系に熱力学第一法則を適用する、

$$
dE = dQ - dW
$$

ここで、$dE$、$dQ$、$dW$は、それぞれエネルギー、ワイヤーからの熱伝達、ワイヤーにかかる仕事の増分変化である。システムが断熱的であるという仮定の下で、式3は次のようになる：

$$
dE = -dW
$$

ここで、$-dW$は$P dt$に等しい（ここで、$P$はワイヤーに散逸する電力、すなわち$i^2(t)R(t)$または$v(t)i(t)$）。
ワイヤの運動エネルギーや位置エネルギーには変化がないため、$dE=dU$となる。したがって、式1、2、4から、次のことがわかる：

$$
P dt = \rho l A C(T) dT
$$

両辺を積分して

$$
\int^{T_f}_{T_0} P dt = \rho l A \int^{T_f}_{T_0} C(T) dT
$$




When modeling the wire, current values were chosen such that the time to fuse was kept under 1 ms. This allowed the adiabatic approximation to still be valid under experimental conditions to insure as little error as possible. The results of these experiments are given Table I. The data shows that equation 3 is a valid means of obtaining a good engineering approximation of the dimensions of the wire that requires a designated amount of energy to fuse. Plots of the experimental and calculated energy for a 35 gauge wire is given in Figures 3 and 4. Table I and Figures 3 and 4 show that the energy to fuse the wire is dependent only on the volume.

ワイヤーをモデル化する際、溶断までの時間が1ms以下になるような電流値を選んだ。これにより、実験条件下でも断熱近似が有効であり、誤差をできるだけ小さくすることができた。これらの実験結果を表Iに示す。このデータから、式3は、ヒューズに指定されたエネルギー量を必要とするワイヤーの寸法について、工学的に優れた近似値を得る有効な手段であることがわかる。35ゲージ・ワイヤーの実験値と計算値のプロットを図3と4に示す。表Iと図3、4から、ワイヤーを溶断するエネルギーは体積にのみ依存することがわかる。

Although the energy constraints of the klystron are met by specifying the volume of the wire, modeling the arc voltage in addition to the energy would be a more complete way to test the crowbar. The voltage across an arc in a klystron can be approximated as a constant voltage drop for currents less than 1 kA.3 Since the wire resistance increases as its temperature increases, a wire will not produce a constant voltage drop for a constant current. However, if the current through the arc or through the test wire decreases with time, then the voltage across the wire may be relatively constant. A wire volume can be chosen such that it meets the energy constraints as well as meeting the initial arc voltage drop.

クライストロンのエネルギー制約は、ワイヤーの体積を指定することで満たされますが、エネルギーに加えてアーク電圧をモデル化することが、バールをテストするのにより完全な方法となります。クライストロンのアークを横切る電圧は、1 kA 未満の電流に対して一定の電圧降下として近似することができます。しかし、アークを流れる電流または試験ワイヤを流れる電流が時間と共に減少する場合、ワイヤを横切る電圧は比較的一定になる可能性がある。ワイヤ体積は、エネルギー制約を満たすと同時に、初期のアーク電圧降下を満たすように選択することができます。

Klystron arc voltage drops are determined by the internal structure of the klystron. This voltage along with an estimate of the initial arc current can be used to determine the cold resistance of the test wire as


クライストロンのアーク電圧降下は、クライストロンの内部構造によって決定されます。この電圧と初期アーク電流の推定値を用いて、テストワイヤーの冷間抵抗を以下のように決定することができます。



where V,,, is the arc voltage and I,,, 0 is an estimated value of the initial arc current.
Equation 10 and equation 3 can be used to create simultaneous length us. area curves where the intersection point is the volume needed to meet the energy constraint and the length and area to meet the arc voltage requirement. A graph showing the length vs.wire gauge (function of the wire area) is given in Figure 5. Three possible arc voltages imply three different length curves. These curves are simultaneously graphed against a length curve for a test wire with a 20 J fusing energy. From these curves it is possible to choose a wire gauge and length needed to sufficiently test the crowbar.

ここで、V,,, はアーク電圧、I,,, 0 は初期アーク電流の推定値である。
式 10 と式 3 を使用して、エネルギー制約を満たすために必要な体積と、アーク電圧要件を満たすための長さと面積を交点とする、長さ対面積の曲線を同時に作成することができます。長さ対ワイヤー・ゲージのグラフ（ワイヤー面積の関数）を図 5 に示す。3種類のアーク電圧が3種類の長さ曲線を意味します。これらの曲線は同時に、溶断エネルギー 20 J のテストワイヤーの長さ曲線に対してグラフ化されています。これらの曲線から、バールを十分に試験するために必要なワイヤーゲージと長さを選択することができます。

The constraints on the klystron amplifiers used on LEDA and to be used on APT have changed from restrictions on the action to the energy of a klystron arc. A different method for determining test wire dimensions was developed and tested. This method is based on equating the klystron arc energy to the wire fusing energy while at the same time equating the arc voltage to the initial test wire voltage drop.

LEDAで使用され、APTで使用されるクライストロンアンプの制約は、クライストロンアークのエネルギーに対する作用の制約から変化した。テストワイヤーの寸法を決定するための異なる方法が開発され、テストされました。この方法は、クライストロンアークのエネルギーをワイヤーの溶断エネルギーと等しくすると同時に、アーク電圧を初期のテストワイヤー電圧降下と等しくすることに基づいています。