# 附录
## 一、乘法附注1、2的数学证明

1. 任何一个 \\( n \\) 位数乘以一个 \\( m \\) 位数，其结果将是一个 \\( n+m \\) 位数或 \\( n+m-1 \\) 位数。

证明：设

\\[ a_i (i = 1、2、3....n) \\]
\\[ b_j (j = 1、2、3....m) \\]

分别表示一个数的某位数字，并设 \\( a_1 \neq 0 \\)，\\( b_1 \neq 0 \\) 则一个 \\( n \\) 位数可表示为 \\( \sum_{i=1}^n a_i 10^{n-i} \\) 
 ，一个 \\( m \\) 位数可表示为 \\( \sum_{j=1}^{m} b_j 10^{m-j} \\) 。

因为 

\\( 10^{n-1} \leq \sum_{i=1}^{n} a_i 10^{n-i} < 10^n \\) ………… ① 

\\( 10^{m-1} \leq \sum_{j=1}^{m} b_j 10^{m-j} < 10^m \\) ………… ②

所以，将①②两式相乘得

\\( 10^{m+n-2} \leq \left(\sum_{i=1}^n a_i 10^{n-i}\right) \left(\sum_{j=1}^n b_j 10^{m-j}\right) < 10^{m+n} \\) ………… ③

设乘积 \\( \left( \sum_{i=1}^n a_i 10^{n-i} \right) \left( \sum_{j=1}^m b_j 10^{m-j} \right) = \sum_{k=1}^p c_k 10^{p-k} \\)

\\( p \\) 为乘积的位数，而

\\( 10^{p-1} \leq \sum_{k=1}^p c_k 10^{p-k} < 10^p \\)
………… ④

式④与式③比较可得

\\( p-1=n+m-2 \\)

所以 \\( p=n+m-1 \\) 或 \\( p=n+m \\)

若 \\( m=1 \\) ，即乘数是个一位数 \\( b_1 \\) ，则乘积的位数 \\( p=n \\) 或 \\( n+1 \\) 。

2. \\( \frac{1}{b} \\) 是乘数为 \\( b \\) 时的进位单位

设被乘数为 \\( \sum_{i=1}^n a_i 10^{n-i} \\) ，乘数为 \\( b \\) ，则 \\( \left( \sum_{i=1}^n a_i 10^{n-i} \right)·b \\) 是一个 \\( n \\) 位数或 \\( n+1 \\) 位数。为了说法统一，而便利于联系其他计算工具，我们约定把 \\( n \\) 位数也当作 \\( n+1 \\) 位数，而第一位是"0"。

这样 \\( \sum_{i=1}^n a_i 10^{n-i} \\) 与 \\( b \\) 的积可以表示为 \\( \sum_{j=1}^{n+1} c_j 10^{n+1-j} \\)

于是我们得到

\\[ \left( \sum_{i=1}^n a_i 10^{n-i} \right)·b = \sum_{j=1}^{n+1} c_j 10^{n+1-j} \\]

下面的问题就是要从积的第一位数 \\( c_1 \\) 开始，逐位求出积的任何一位数字 \\( c_x \\) 。

我们把被乘数分成三部分：

\\[ \sum_{i=1}^n a_i 10^{n-i}= \sum_{i=1}^{x-2} a_i 10^{n-i} + a_{x-1} 10^{n-x+1} + \sum_{i=x}^n a_i 10^{n-1} \\]

于是

\\[ \sum_{j=1}^{n+1} c_j 10^{n+1-i} = \left(\sum_{i=1}^{x-2} a_i 10^{n-i}\right)·b + (a_{x-1} 10^{n-x+1})·b + \left( \sum_{i=x}^{n} a_i 10^{n-i} \right)·b \\]

用 \\( 10^{n-x+1} \\) 除等式两边得

\\[ \sum_{j=1}^{n+1} c_j 10^{n-i} = \left( \sum_{i=1}^{x-2} a_i 10^{x-1-i} \right)·b + (a_{x-1})·b + \left( \sum_{i=x}^{n} a_i 10^{x-1-i} \right)·b \\]

\\( c_x \\) 就是 \\( \sum_{j=1}^{n+1} c_j 10^{x-j} \\) 的个位数。

根据普通乘法规律，我们知道 \\( c_x \\) 是由 \\( (a_{x-1})·b \\) 的个位数与 \\( \left( \sum_{i=x}^{n} a_i 10^{x-1-i} \right)·b \\) 进到个位的数相加而得到。

\\( \left( \sum_{i=x}^n a_i 10^{x-1-i}\right)·b \\) 要能进位到个位数，必须满足 
\\( \left( \sum_{i=x}^n a_i 10^{x-1-i} \right)·b \geq 1 \\) ，

即 \\( \left( \sum_{i=x}^{n} a_i 10^{x-1-i} \right)·b \geq \frac{1}{b} \\)

显然，\\( \frac{1}{b} \\) 就是乘数为 \\(b\\) 时的进位单位。

当 \\( 2\left(\frac{1}{b}\right) \leq R < 3\left(\frac{1}{b}\right) \\) 时，就进2； \\( 3\left(\frac{1}{b}\right) \leq R < 4\left(\frac{1}{b}\right) \\) 时，就进3；依此类推。


## 二、个律表

<table>
  <tr>
    <td rowspan="2">被乘数</td>
    <td colspan="5">偶数</td>
    <td colspan="5">奇数</td>
    <td rowspan="2">个律找法<br>以被乘数(本)为准</td>
  </tr>
  <tr>
    <td>0</td>
    <td>2</td>
    <td>4</td>
    <td>6</td>
    <td>8</td>
    <td>1</td>
    <td>3</td>
    <td>5</td>
    <td>7</td>
    <td>9</td>
  </tr>
  <tr>
    <td>0</td>
    <td rowspan="2">0</td>
    <td rowspan="2">0</td>
    <td rowspan="2">0</td>
    <td rowspan="2">0</td>
    <td rowspan="2">0</td>
    <td>0</td>
    <td>0</td>
    <td>0</td>
    <td>0</td>
    <td>0</td>
    <td>0</td>
  </tr>
  <tr>
    <td>5</td>
    <td>5</td>
    <td>5</td>
    <td>5</td>
    <td>5</td>
    <td>5</td>
    <td>偶0，奇5</td>
  </tr>
  <tr>
    <td>1</td>
    <td rowspan="2">0</td>
    <td rowspan="2">2</td>
    <td rowspan="2">4</td>
    <td rowspan="2">6</td>
    <td rowspan="2">8</td>
    <td>1</td>
    <td>3</td>
    <td>5</td>
    <td>7</td>
    <td>9</td>
    <td>自身</td>
  </tr>
  <tr>
    <td>6</td>
    <td>6</td>
    <td>8</td>
    <td>0</td>
    <td>2</td>
    <td>4</td>
    <td>偶自身，奇 ±5 (或取偶同)</td>
  </tr>
  <tr>
    <td>2</td>
    <td rowspan="2">0</td>
    <td rowspan="2">4</td>
    <td rowspan="2">8</td>
    <td rowspan="2">2</td>
    <td rowspan="2">6</td>
    <td>2</td>
    <td>6</td>
    <td>0</td>
    <td>4</td>
    <td>8</td>
    <td>自加</td>
  </tr>
  <tr>
    <td>7</td>
    <td>7</td>
    <td>1</td>
    <td>5</td>
    <td>9</td>
    <td>3</td>
    <td>偶自加，奇自加 ±5 (或取偶同)</td>
  </tr>
  <tr>
    <td>3</td>
    <td rowspan="2">0</td>
    <td rowspan="2">6</td>
    <td rowspan="2">2</td>
    <td rowspan="2">8</td>
    <td rowspan="2">4</td>
    <td>3</td>
    <td>9</td>
    <td>5</td>
    <td>1</td>
    <td>7</td>
    <td>偶补倍，奇倍凑</td>
  </tr>
  <tr>
    <td>8</td>
    <td>8</td>
    <td>4</td>
    <td>0</td>
    <td>6</td>
    <td>2</td>
    <td>补倍</td>
  </tr>
  <tr>
    <td>4</td>
    <td rowspan="2">0</td>
    <td rowspan="2">8</td>
    <td rowspan="2">6</td>
    <td rowspan="2">4</td>
    <td rowspan="2">2</td>
    <td>4</td>
    <td>2</td>
    <td>0</td>
    <td>8</td>
    <td>6</td>
    <td>偶补，奇凑</td>
  </tr>
  <tr>
    <td>9</td>
    <td>9</td>
    <td>7</td>
    <td>5</td>
    <td>3</td>
    <td>1</td>
    <td>取补</td>
  </tr>
</table>


## 三、几点说明
### 1.偶同数
两数同乘以一个偶数，个律相同，这两数互称偶同数。共有0与5、1与6、2与7、3与8、4与9五对。可以看出，偶同数相差5，±5等于取偶同数。

### 2.补数
凡两数之和是10，则这二数互为补数。共有1+9=10、2+8=10、3+7=10、4+6=10、5+5=10五对。其中4与6就互为补数，余同。

### 3.凑数
凡二数之和的个位是5，则这二数互为凑数。共有1+4=5、2+3=5、5+0=5、6+9=15、7+8=15五对。其中1与4就互为凑数，余同。
