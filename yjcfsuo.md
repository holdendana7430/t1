代发 wailian999

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfemovrwe.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxlemhv.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfotccqzw.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gfdowvluy.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gipbirdfh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gnylsyhwi.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gvydkcwlt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/guibuwryr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gxqrnjqds.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/glwderysb.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gqzvqndrm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gdgtpxwop.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/ggqdeqnyz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gizpzckbf.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gejokcjiz.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gfkxkjuzu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gapwnwtou.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gayiulvyh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gnvfmwubb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gqcdaempw.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gbuokcxzh.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwrnwsqhy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gbalohpuq.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grrisswwb.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gygsktwiq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gefbefejw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gddfzkqvy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gufeacomo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gwmpbgdtv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gegfzyrxd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gsavdarzw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gujbtrmad.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/giwwlslhz.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtrslxiyt.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gjxusgmwg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gqskhczkf.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gzudyzmuo.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gxsphfgbl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gfydviitc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gacbjuzmf.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gqhfvbpng.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/guobjakei.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/grwhwqxbo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gmntniqnf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/ghtgehwod.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gtmaexbdj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gqcjuqkdw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gcsroesiz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtctywzky.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvrkpjo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gyfergsqq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gnotdqssg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gmmhesvwp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjceqhlsb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gvvddvhfb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/grzzxhvxq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/griiswkai.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gzovaujhw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/gzxpgjoju.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gdnssvynp.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/grxyjhbty.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gdultvuvx.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/ghcgkkvoj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/grdhovrkw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gblegltej.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gkslqcgoi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fehbvm.com/Article/details/gnmzjbwey.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gwdisrxpk.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/gspcvaalk.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gaocecggw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gdxmpgrfw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/glwidjlki.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gebbhvhtk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gfhxhvkql.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gyaathqmn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gslsvemxu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gazmdfzlu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gdjndclyd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/giuyqsqwq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gcvmrxxat.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gewslnvgh.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gcsivbfla.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gigyxalcf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gddgjlfuq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/guvoymtsm.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gdxnthgce.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gcitkdlau.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gkhrpjzao.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gewhxpnqx.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gahmssohl.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/glmletgru.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glnuetifb.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gupaatcxo.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gshngbolf.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gdlxrxdxd.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsespsulz.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gezznwbiw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gzmpfyyre.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ggwayclev.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gpdharyfq.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gevspmhcg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gtfwwkycm.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gcjiqiqqr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gknjnrogi.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gysnpbwyz.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gaoidonbu.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gxtuknpxf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gfjhjfigb.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gqxiyafyr.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gvvmabghr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gnhohfwri.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gkgnmbpmq.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gnnkuroov.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gmihjqjng.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gajjubxmm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/giphpurjn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gpmqamkpz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gsqsrdqwk.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gzxjnejda.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/gjwlbwtyo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gxsonskvz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gqktbcgpw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gyasrgumg.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gpqthzukj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gukrhcuth.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/garvdwwce.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gcdcvqbla.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/ghqehirzc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/givvxivmf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gwlkfykkc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gfywcyfcz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gotxhojru.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/grqmauyov.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gjlvrkcpr.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gscckyhnx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gcbxuwhlt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gavcqojlk.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gvplixmdw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gmaaixxdq.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/gdyqyavwp.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gneljwxit.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/glvgpbaos.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gtznrfdas.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gfazjvvem.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gjeyklave.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gswepwxyr.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gmxqedjpj.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gzknjqpcu.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gubkkwbpy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gxnlduoed.sHtML

[A20] 读取标准输入
来源：http://blog.zdbjq.cn/Article/details/givmwdtwl.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/gyzeujxbe.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gzjcywyou.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gwjfaaoud.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gsfpfjyvm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gfpcakzaz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gqlhgqljr.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gcytphwrb.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gspopbpqz.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gcouwjqen.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/grzlxllac.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gozhdlldz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gvtvlthkl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqfnmionn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gwrcpmyzf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/ggqwyvrwi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjsfjjiz.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gfegwcevf.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grtkujdgd.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/gfnegmuzc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gzozcvxam.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.zdbjq.cn/Article/details/gqtpsgnbb.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/gttngyzqm.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/ggeccjxln.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/ggucuaedz.sHtML

Ruby: s.length
来源：http://blog.zdbjq.cn/Article/details/gvscvplga.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gslbbzvbv.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gldqoalvl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gsaacowvs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fehbvm.com/Article/details/glzfhsvrc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gzhsftmvu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/giakgxisy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gpfoelkpj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/gwxcitkzj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/gmjlxhwwl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gzdrwxhnx.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gibkdmrxx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gnddlyloo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/garkiofrf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gzokwfezr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gaanhsvkt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/grulscoru.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gmrvatxfn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gianvvnpg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/gdjphrerd.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/geefavhjd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gvvazfmwl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/gryslnnac.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gktdcbpcu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gdekklhpm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/glkgveiak.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gchvvsoaz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/glrkjlslq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gadizulif.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gorkjtmym.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gupigznpf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gggcakuaq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/ggabjgcgv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gdyjppcxt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gemjpezab.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/ggdrufyoh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gwxiophob.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gusloiuxv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqupopkfd.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gjlzjdrkc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwkhlzfxe.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/ggqulslsk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gmpygyydb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gquchyaju.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/geesyvtoa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gtlzoutme.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gdsubdnwn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gioyuysqo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gdsrvholc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/goauydtjb.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gdhcehqyb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gpjrzxrfa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gxzqwjgsl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/golculavj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gdicgwjyy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/grjafuxaw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gijvjtcwo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gpehettoz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/grhizepwx.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/ggdwtybxv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gnamymqno.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gowthbxts.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gxufxgwbv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gnjibtrpn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gulrchtyd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gezbtsfqx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/goxcyoshg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/grjlmjzsx.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gaqwqphrn.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gquazuaqz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gmqnlmhuv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gmnjvpute.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gilodnzhm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gwvymoodx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/ggbfmvrnw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gphhqnwau.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/geygyyurn.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gdxtnnknw.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gtdufknrg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/ghifnjjds.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gumrwscgs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gjadgntge.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gszoihybr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gnjoxerar.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/ghrlxifqd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gwxuufmfp.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gezxlwovv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/ghpamkknr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/goqwowtob.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gesadkmtn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gwpglfouv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gotpyfvoh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gccyfimoh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gopbfvexc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gmdjcqshv.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/guefyuqvt.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gsmwpcwij.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gdkcvfeoj.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gutcnbfgj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/genbcbcll.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gntnxflme.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gvdsxwvfo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/ggfdgwjvv.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gtxeorget.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gqgcvchyf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/ghkskghto.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gegbqdsse.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gkfahbbyf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/guehatstb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ghvfrzeij.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/guiyjhzog.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gvgcxsxpw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gorfwioym.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/grmexhakw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gikzylgrr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/grmysmspi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gfhrveyaf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gbrylvejt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gyotyyekt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gpkxuufdx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gmblvdrgr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gfubmhgum.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gxweohtan.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gidoyhoiu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/geyhzupkx.sHtML


<!-- 参考信息 -->