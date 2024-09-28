与えられた電流の式は次の形をしています：

$$
i(t) = A\left( e^{\lambda_1 t} - e^{\lambda_2 t} \right)
$$

これの二乗 $ i(t)^2 $ を積分します。

### 積分の式
$$
\int_0^{t_1} i(t)^2 dt = \int_0^{t_1} \left[ A \left( e^{\lambda_1 t} - e^{\lambda_2 t} \right) \right]^2 dt
$$

まず、電流の二乗を計算します。

### 1. 電流の二乗
$$
i(t)^2 = A^2 \left( e^{\lambda_1 t} - e^{\lambda_2 t} \right)^2
$$

展開すると、
$$
i(t)^2 = A^2 \left( e^{2\lambda_1 t} - 2e^{(\lambda_1 + \lambda_2)t} + e^{2\lambda_2 t} \right)
$$

したがって、積分は次の形になります：
$$
\int_0^{t_1} A^2 \left( e^{2\lambda_1 t} - 2e^{(\lambda_1 + \lambda_2)t} + e^{2\lambda_2 t} \right) dt
$$

### 2. 定数を外に出す
定数 $ A^2 $ を積分の外に出します：
$$
A^2 \int_0^{t_1} \left( e^{2\lambda_1 t} - 2e^{(\lambda_1 + \lambda_2)t} + e^{2\lambda_2 t} \right) dt
$$

### 3. 各項の積分
それぞれの項を個別に積分します。

1. $ \int_0^{t_1} e^{2\lambda_1 t} dt $

$$
\int e^{2\lambda_1 t} dt = \frac{1}{2\lambda_1} e^{2\lambda_1 t}
$$

したがって、積分範囲 $ 0 $ から $ t_1 $ で評価すると：

$$
\int_0^{t_1} e^{2\lambda_1 t} dt = \frac{1}{2\lambda_1} \left( e^{2\lambda_1 t_1} - 1 \right)
$$

2. $\int_0^{t_1} e^{(\lambda_1 + \lambda_2) t} dt $

$$
\int e^{(\lambda_1 + \lambda_2) t} dt = \frac{1}{\lambda_1 + \lambda_2} e^{(\lambda_1 + \lambda_2)t}
$$

したがって、積分範囲 $ 0 $ から $ t_1 $ で評価すると：

$$
\int_0^{t_1} e^{(\lambda_1 + \lambda_2) t} dt = \frac{1}{\lambda_1 + \lambda_2} \left( e^{(\lambda_1 + \lambda_2)t_1} - 1 \right)
$$

3. $ \int_0^{t_1} e^{2\lambda_2 t} dt $

$$
\int e^{2\lambda_2 t} dt = \frac{1}{2\lambda_2} e^{2\lambda_2 t}
$$

したがって、積分範囲 $ 0 $ から $ t_1 $ で評価すると：

$$
\int_0^{t_1} e^{2\lambda_2 t} dt = \frac{1}{2\lambda_2} \left( e^{2\lambda_2 t_1} - 1 \right)
$$

### 4. 結果をまとめる
これらの結果を組み合わせると、最終的な積分は次のようになります：

$$
A^2 \left[ \frac{1}{2\lambda_1} \left( e^{2\lambda_1 t_1} - 1 \right) - \frac{2}{\lambda_1 + \lambda_2} \left( e^{(\lambda_1 + \lambda_2)t_1} - 1 \right) + \frac{1}{2\lambda_2} \left( e^{2\lambda_2 t_1} - 1 \right) \right]
$$

これが、指定された範囲での $ i(t)^2 $ の積分結果です。