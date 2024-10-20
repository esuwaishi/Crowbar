銅線の抵抗率は温度によって変化します。特に、温度が上昇すると抵抗率も増加します。これは、温度が上がると金属中の自由電子の運動が乱され、電子が原子と衝突する頻度が増すためです。この関係は次の式で表されます。

### 抵抗率の温度依存性の式

金属の抵抗率 $ \rho(T) $ は温度 $ T $ に対して以下の式で表すことができます。

$$
\rho(T) = \rho_0 \left( 1 + \alpha (T - T_0) \right)
$$

- $ \rho(T) $: 温度 $ T $ における抵抗率
- $ \rho_0 $: 基準温度 $ T_0 $ （通常は20℃）での抵抗率
- $ \alpha $: 抵抗率の温度係数（銅の場合、典型的に約 $ 0.0039 \, \text{K}^{-1} $）
- $ T $: 実際の温度（ケルビンまたは摂氏）
- $ T_0 $: 基準温度（通常は20℃）

### 銅の抵抗率

銅の抵抗率は基準温度（通常は20℃）で次のような値です。

- **20℃における銅の抵抗率** $ \rho_0 $: 約 $ 1.68 \times 10^{-8} \, \Omega \cdot m $

### 温度依存性の具体例

例えば、温度が20℃から50℃に上昇した場合、銅の抵抗率は次のように計算できます。

1. 基準温度（20℃）での抵抗率 $ \rho_0 = 1.68 \times 10^{-8} \, \Omega \cdot m $
2. 温度係数 $ \alpha = 0.0039 \, \text{K}^{-1} $
3. $ T = 50^\circ C $
4. 式に代入すると、抵抗率 $ \rho(50^\circ C) $ は以下の通りです。

$$
\rho(50^\circ C) = 1.68 \times 10^{-8} \, \Omega \cdot m \times (1 + 0.0039 \times (50 - 20)) = 1.68 \times 10^{-8} \, \Omega \cdot m \times 1.117
$$

$$
\rho(50^\circ C) = 1.88 \times 10^{-8} \, \Omega \cdot m
$$

このように、温度が上昇すると銅の抵抗率は増加します。高温になるほど、この影響が大きくなります。

### 温度係数 $ \alpha $ の意味

銅の温度係数 $ \alpha $ は、抵抗率が1℃の温度変化によってどれだけ変わるかを示します。銅の場合、この値は約 $ 0.0039 \, \text{K}^{-1} $ であり、これは1℃上昇すると抵抗率が約0.39%増加することを意味します。

### 実用上の影響

- **高温環境での銅の使用**: 高温になる環境で銅線を使用する場合、抵抗が増えることで電力損失が大きくなるため、電気機器の効率が低下します。
- **温度補正**: 実際の測定で抵抗率を使用する際には、温度補正を行う必要があります。