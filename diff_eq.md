この微分方程式

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = L_3 \frac{di_c(t)}{dt} + R_i i_c(t)
$$

を解くために、まず $ i_c(t) $ を与えられた形で表すと

$$
i_c(t) = A \left( e^{\lambda_1 (t+t_1)} - e^{\lambda_2 (t+t_1)} \right)
$$

です。この式を時間で微分して $ \frac{di_c(t)}{dt} $ を求めます。

$$
\frac{di_c(t)}{dt} = A \left( \lambda_1 e^{\lambda_1 (t+t_1)} - \lambda_2 e^{\lambda_2 (t+t_1)} \right)
$$

次に、この式をもとの微分方程式に代入します。

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = L_3 \left( A \left( \lambda_1 e^{\lambda_1 (t+t_1)} - \lambda_2 e^{\lambda_2 (t+t_1)} \right) \right) + R_i A \left( e^{\lambda_1 (t+t_1)} - e^{\lambda_2 (t+t_1)} \right)
$$

この式を簡略化して整理します。

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = A \left( L_3 \lambda_1 e^{\lambda_1 (t+t_1)} - L_3 \lambda_2 e^{\lambda_2 (t+t_1)} + R_i e^{\lambda_1 (t+t_1)} - R_i e^{\lambda_2 (t+t_1)} \right)
$$

次に、この線形微分方程式を解くために、与えられた初期条件 $ i_s(t_1) = I_0 $ を使います。この時点では具体的な解法にはいくつかのアプローチがありますが、たとえば、定数変化法やラプラス変換を用いることが可能です。ラプラス変換を使う場合、方程式を変換し、変数の代入後に逆変換を行うことで、時間領域での解を得ることができます。

より詳細な解法については、方程式を具体的に変換・解く必要がありますが、ここまでで初期式の代入と整理が行われました。


この微分方程式

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = L_3 \frac{di_c(t)}{dt} + R_i i_c(t)
$$

を、次の与えられた $ i_c(t) $ の形で解きます。

$$
i_c(t) = A \left( e^{\lambda_1 (t+t_1)} - e^{\lambda_2 (t+t_1)} \right)
$$

まずは、 $ i_c(t) $ を時間 $ t $ で微分して、 $ \frac{di_c(t)}{dt} $ を求めます。

$$
\frac{di_c(t)}{dt} = A \left( \lambda_1 e^{\lambda_1 (t+t_1)} - \lambda_2 e^{\lambda_2 (t+t_1)} \right)
$$

これを微分方程式に代入して展開します。

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = L_3 \left( A \left( \lambda_1 e^{\lambda_1 (t+t_1)} - \lambda_2 e^{\lambda_2 (t+t_1)} \right) \right) + R_i A \left( e^{\lambda_1 (t+t_1)} - e^{\lambda_2 (t+t_1)} \right)
$$

ここで、右辺を整理します。

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = A \left( (L_3 \lambda_1 + R_i) e^{\lambda_1 (t+t_1)} - (L_3 \lambda_2 + R_i) e^{\lambda_2 (t+t_1)} \right)
$$

### 1. 同次解の求解

まずは、微分方程式の同次部分

$$
L_2 \frac{di_s(t)}{dt} + R_s i_s(t) = 0
$$

を解きます。これは、定数係数の1次の微分方程式です。この形式の解は次の形になります。

$$
i_s^{(h)}(t) = C e^{-\frac{R_s}{L_2} t}
$$

ここで $ C $ は定数です。

### 2. 非同次解の求解

次に、右辺が非ゼロの微分方程式を解きます。右辺が指数関数項の線形結合になっているため、特解は次の形を仮定します。

$$
i_s^{(p)}(t) = B_1 e^{\lambda_1 (t+t_1)} + B_2 e^{\lambda_2 (t+t_1)}
$$

これを元の非同次方程式に代入します。

$$
L_2 \left( B_1 \lambda_1 e^{\lambda_1 (t+t_1)} + B_2 \lambda_2 e^{\lambda_2 (t+t_1)} \right) + R_s \left( B_1 e^{\lambda_1 (t+t_1)} + B_2 e^{\lambda_2 (t+t_1)} \right)
$$

この左辺を展開すると

$$
\left( B_1 (L_2 \lambda_1 + R_s) e^{\lambda_1 (t+t_1)} + B_2 (L_2 \lambda_2 + R_s) e^{\lambda_2 (t+t_1)} \right)
$$

右辺の係数と比較します。

$$
A \left( (L_3 \lambda_1 + R_i) e^{\lambda_1 (t+t_1)} - (L_3 \lambda_2 + R_i) e^{\lambda_2 (t+t_1)} \right)
$$

これにより、係数の一致条件から $ B_1 $ と $ B_2 $ が決定されます。

$$
B_1 (L_2 \lambda_1 + R_s) = A (L_3 \lambda_1 + R_i)
$$

$$
B_2 (L_2 \lambda_2 + R_s) = -A (L_3 \lambda_2 + R_i)
$$

これを解くことで、 $ B_1 $ と $ B_2 $ が求まります。

$$
B_1 = \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s}
$$

$$
B_2 = \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s}
$$

### 3. 一般解の構成

同次解と特解を組み合わせることで、微分方程式の一般解が求まります。

$$
i_s(t) = C e^{-\frac{R_s}{L_2} t} + \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{\lambda_1 (t+t_1)} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{\lambda_2 (t+t_1)}
$$

### 4. 初期条件の適用

初期条件 $ i_s(t_1) = I_0 $ を適用して、定数 $ C $ を決定します。

$$
i_s(t_1) = C e^{-\frac{R_s}{L_2} t_1} + \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{\lambda_1 (t_1+t_1)} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{\lambda_2 (t_1+t_1)}
$$

これを解くことで $ C $ を求め、最終的な解を得ます。

微分方程式の一般解を

$$
i_s(t) = C e^{-\frac{R_s}{L_2} t} + \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{\lambda_1 (t+t_1)} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{\lambda_2 (t+t_1)}
$$

としました。この解に初期条件 $ i_s(t_1) = I_0 $ を適用して $ C $ を求めます。

### 初期条件の適用

$ t = t_1 $ のとき、$ i_s(t_1) = I_0 $ なので、これを代入します。

$$
I_0 = C e^{-\frac{R_s}{L_2} t_1} + \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{\lambda_1 (t_1+t_1)} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{\lambda_2 (t_1+t_1)}
$$

ここで、指数項を計算します。$ e^{\lambda_1 (t_1 + t_1)} = e^{2\lambda_1 t_1} $ および $ e^{\lambda_2 (t_1 + t_1)} = e^{2\lambda_2 t_1} $ なので、

$$
I_0 = C e^{-\frac{R_s}{L_2} t_1} + \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{2\lambda_1 t_1} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{2\lambda_2 t_1}
$$

### $ C $ の解法

この式を $ C $ について解きます。

$$
C e^{-\frac{R_s}{L_2} t_1} = I_0 - \left( \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{2\lambda_1 t_1} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{2\lambda_2 t_1} \right)
$$

両辺を $ e^{-\frac{R_s}{L_2} t_1} $ で割って $ C $ を求めます。

$$
C = \left( I_0 - \left( \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{2\lambda_1 t_1} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{2\lambda_2 t_1} \right) \right) e^{\frac{R_s}{L_2} t_1}
$$

### 最終的な解

これで $ C $ が求まったので、最終的な解 $ i_s(t) $ は次のようになります。

$$
i_s(t) = \left( I_0 - \left( \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{2\lambda_1 t_1} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{2\lambda_2 t_1} \right) \right) e^{-\frac{R_s}{L_2} (t - t_1)} 
$$
$$
+ \frac{A (L_3 \lambda_1 + R_i)}{L_2 \lambda_1 + R_s} e^{\lambda_1 (t+t_1)} + \frac{-A (L_3 \lambda_2 + R_i)}{L_2 \lambda_2 + R_s} e^{\lambda_2 (t+t_1)}
$$

これが求める解です。