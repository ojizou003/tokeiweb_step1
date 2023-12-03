## 確率・統計 公式集

■スタージェスの公式
$N$をサンプルサイズ、$k$を階級数とすると、次のように計算することができる
$k = \log_2N + 1$

■分散$V = \frac{1}{n}\sum_{n=i}^n(x_i - \overline{x})^2$

■標準偏差$\sigma = \sqrt{分散}$

■変動係数$CV = \frac{\sigma}{\overline{x}}$

■順列$_nP_k = \frac{n!}{(n-k)!}$

■期待値
期待値とは、1回の試行で得られる値の平均値
得られうるすべての値と起こる確率の積を足し合わせたもの
$\Sigma_{k=1}^np_kx_k$

■ベイズの定理
$P(B_i|A) = \frac{P(A\cap B_i)}{P(A)} = \frac{P(B_i)P(A|B_i)}{P(A)}$

■二項分布の期待値と分散
$E(X)=np$
$V(X)=np(1-p)$

■ポアソン分布
二項分布でn→∞、p→０に近づけるとポアソン分布に近似する
ある期間に起こる「回数」に関する分布
$P(X=k) = \frac{e^{-\lambda}\lambda^k}{k!}$
$E(X) = \lambda$
$V(X) = \lambda$

■幾何分布
成功確率がｐである独立なベルヌーイ試行を繰り返すとき、初めて成功するまでの試行回数ｘが従う確率分布を「幾何分布」という
$P(X=k)=(1-p)^{k-1}P$
$E(X) = \frac{1}{p}$
$V(X) = \frac{1-p}{p^2}$

■超幾何分布
AとBで構成されるN個からなる集団があり、AがM個、BがN-M個であるとする
この集団から取り出されたn個の中に含まれるAの個数が従う確率分布を「超幾何分布」という
$E(X) = n･\frac{M}{N}$
$V(X) = n･\frac{M(N-M)}{N^2}･\frac{N-n}{N-1}$

■負の二項分布
成功確率がｐの試行において、ｋ回成功するまでにｘ回試行する確率は次の式で計算できる
$P(X=x) = _{x-1}C_{k-1}p^k(1-p)^{x-k}$
$E(X) = \frac{k}{p}$
$V(X) = k\frac{1-p}{p^2}$

■正規分布
$f(x) = \frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
$E(X) = \mu$
$V(X) = \sigma^2$

■標準正規分布
正規分布の中で、特に「平均$\mu=0$、分散$\sigma^2=1$」である正規分布を「標準正規分布」という

■指数分布
指数分布は、連続型確率分布の一つで、次に何かが起こるまでの期間が伴う分布
$f(x)=\lambda e^{-\lambda x}$
$E(X) = \frac{1}{\lambda}$
$V(X) = \frac{1}{\lambda^2}$

■指数分布の使い方
ある期間に平均して$\lambda$回起こる現象が次に起こるまでの期間を$x$としたとき、「期間$X$が$x$以下となる確率」すなわち「$x$までの累積分布関数$F(x)$」は次のようになる
$F(x) = P(X\leq x) = \int_{-\infty}^xf(t)dt = \int_0^x\lambda e^{-\lambda t}dt = 1-e^{-\lambda x}$

■離散一様分布
$P(X=k) = \frac{1}{N}$
$E(X)=\frac{N+1}{2}$
$V(X)=\frac{N^2-1}{12}$

■連続一様分布
$f(x) = \frac{1}{b-a}$
$E(X) = \frac{a+b}{2}$
$V(X) = \frac{(b-a)^2}{12}$

■2つの確率変数の期待値
$E(X+Y) = E(X) + E(Y)$
$E(XY) = E(X)E(Y)$

■2つの確率変数の分散
$V(X+Y) = V(X) + V(Y) + 2Cov(X, Y)$
$V(X-Y) = V(X) + V(Y) - 2Cov(X, Y)$

■２つの確率変数の共分散
$Cov(X, Y) = E[(X-\mu_x)(Y-\mu_y)] = E(XY)-\mu_x \mu_y$

■相関係数...共分散を標準偏差で割ったもの
$\rho = \frac{Cov(X, Y)}{\sqrt{V(X)V(Y)}}$

■標本分散
$S^2 = \frac{1}{n}\sum_{i=1}^n(x_i-\overline{x})^2$

■不偏分散
$s^2 = \frac{n}{n-1}\times \frac{1}{n}\sum_{i=1}^n(x_i-\overline{x})^2 = \frac{1}{n-1}\sum_{i=1}^n(x_i-\overline{x})^2$

■標準偏差
$s = \sqrt{s^2}$

■標準誤差
標準誤差(SE: standard error)は推定量の標準偏差
推定量そのもののばらつき(=精度)を表す
標準誤差は一般的に標本平均の標準偏差を意味する
$SE = \sqrt \frac{s^2}{n} = \frac{s}{\sqrt{n}}$

■母集団と標本の平均、分散記号
- 母平均$\mu$、標本平均$\overline{x}$
- 母分散$\sigma^2$、標本分散$s^2$

■t分布表
$t_\alpha(v)$
$v=n-1$

■母比率の信頼区間
$Z = \frac{\hat{p}-p}{\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}}$

■カイ二乗分布
$x^2 = Z_1^2+Z_2^2+･･･＋Z_k^2$

■母比率の検定
$z = \frac{\hat{p}-p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}$

■二項分布を用いた検定
$z = \frac{X-np}{\sqrt{np(1-np)}}$

■ポアソン分布を用いた検定
$z= \frac{X-n\lambda}{\sqrt{n\lambda}}$

■母比率の差の検定
$z = \frac{\hat{p_1}-\hat{p_2}}{\sqrt{\hat{p}(1-\hat{p})(\frac{1}{n_1}+\frac{1}{n_2})}}$

■相関係数
$r_{xy}=\frac{共分散_{xy}}{標準偏差_x \times 標準偏差_y}
= \frac{\frac{1}{n}\sum_{i=1}^n(x_1-\overline{x})(y_i-\overline{y})}{\sqrt{\frac{1}{n}\sum_{i=1}^n(x_i-\overline{x})^2}\times \sqrt{\frac{1}{n}\sum_{i=1}^n(yi-\overline{y})^2}}$

■無相関の検定
$t = \frac{|r|\sqrt{n-2}}{\sqrt{1-r^2}}$

■偏相関係数
$r_{xy･z} = \frac{r_{xy}-r_{xz}r_{yz}}{\sqrt{1-r_{xz}^2}\sqrt{1-r_{yz}^2}}$

■最小二乗法による$\beta_0$と$\beta_1$の求め方
$\hat{\beta_1} = \frac{\sum_{i=1}^n(y_i-\overline{y})(x_i-\overline{x})}{\sum_{i=1}^n(x_i-\overline{x})^2}$
$\hat{\beta_0} = \overline{y} - \hat{\beta_1}\overline{x}$

■母分散の比の信頼区間の求め方
$F = \frac{s_1^2/\sigma_1^2}{s_2^2/\sigma_2^2}$
上側信頼区間がF(n,m)の場合、下側信頼区間は$\frac{1}{F(m,n)}$

■Welchのt検定
Welchのt検定は、2標本t検定と同様に「平均値の差」の検定方法
$t = \frac{\overline{x_1}-\overline{x_2}}{\sqrt{\frac{s_1^2}{n_1}+\frac{s_2^2}{n_2}}}$