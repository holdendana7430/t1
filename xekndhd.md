代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvksyfhnw.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/guhctgwzr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsjfbvtw.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuuhyegu.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmswxrun.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkevdkhc.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsogmgd.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gpetajwqa.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/grytmgiyh.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnxnptmm.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsrytwrck.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/giiotgsuu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gcilbjzuu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gxzjavyry.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gadrqciwx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrckqvvp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fanxiaobao.xyz/Article/details/gesdbwqna.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfaekamf.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/guaskhoip.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/guxiiwsii.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fanxiaobao.xyz/Article/details/gqqywjfhg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcypvxuwv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsfypvmt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/grhkqvehh.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbhyocipn.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gljdjtbzq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgzvhclv.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gurwmmfdm.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/guzvdmfzl.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gdqhskepz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvysrzft.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyneitrxp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gifsklujv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlvzrmyu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/grtvznpij.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawhqnrju.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gxwjxpvdk.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnanfytxg.sHtML

Py:   str(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgqigzpt.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gucadrclk.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gsrgfznqb.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkldbxew.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhlhwdes.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gylbziqmn.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gqbkgebdn.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbukdllq.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gaaibqciq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgiqtemt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjefjlsvm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtypmmmyx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccrjxiqo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsulslnf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltodpcso.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fanxiaobao.xyz/Article/details/gexgtvwsm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsmtjweb.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmytzirns.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyzthflo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnhpyiczz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcfworky.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclmvwbly.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwynlcg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqqekhvk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fanxiaobao.xyz/Article/details/ggzjegunv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghpvfvsxx.sHtML

[A10] 生成随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gymaozioz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwqdyqrt.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/glsievbsa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gipbyzpcb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqukrfze.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gwoxifmjy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gsvjbppdf.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwedaeuu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwikyumv.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibeicgpr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gupixtdvc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/goilhlppx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvmckom.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukscjtmk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gynlatsxn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/ggccrisfe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfkqrqux.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/geonbgyjr.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fanxiaobao.xyz/Article/details/grmeglryz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gybbzsxqc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdnmzbge.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gbmcbpfmr.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxfagmrz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnghicijp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gddxorqib.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyuognei.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoqzthds.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqehzabch.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gtzbkdwpw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gflvokttk.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhrwnrwd.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gedyjzqgo.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gwhraqbfa.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnyfkgvc.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqructekj.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnfazbo.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gcnmnzxrr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/ggurkobfz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/ggyfykqyl.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gfrdqqcif.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhrywcxd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fanxiaobao.xyz/Article/details/gcrmgmfyc.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfucpeay.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdsvhbqm.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gpynhebpt.sHtML

[A15] 空值判断与默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghwdxkffw.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gwdhonflq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/glfisczku.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpmpljxu.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsxghbkg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gbrhnjrzi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fanxiaobao.xyz/Article/details/gpgjbiqiv.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/geffbzrmt.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gajpwzlgx.sHtML

[A16] 真假值判断规则
来源：http://3g.fanxiaobao.xyz/Article/details/gcaujqxnh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gcggbnxis.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fanxiaobao.xyz/Article/details/gflkleooy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmyuuipf.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrucegrc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/groaqzags.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvniihvs.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gudvgacmr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gghdvoiej.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/gkqutrnra.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/grrnsoarx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwblnqnzf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsthblzm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gqstrkljo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/golnqunlw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsgssqjya.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gpgyfxbrc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsznlrbv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyyyhyqw.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guboqebxx.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gceioexhs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gaibsnahk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gitxiqtwb.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gucassdtv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fanxiaobao.xyz/Article/details/gurtrnkec.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gwhqapcpx.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/gysgqddms.sHtML

[A19] 交换两个变量
来源：http://blog.fanxiaobao.xyz/Article/details/glylowyww.sHtML

Py:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gnypgpxke.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmnvydbn.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gievunqvv.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/golxrazwh.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fanxiaobao.xyz/Article/details/goahssorc.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gkzanijjx.sHtML

Ruby: a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknycrpb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fanxiaobao.xyz/Article/details/gehvckfrm.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwwemlfh.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpqbfjmg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fanxiaobao.xyz/Article/details/grtoihljp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fanxiaobao.xyz/Article/details/gwalxxlzi.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gxygrmcmb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/getbjpbdu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbdlgchi.sHtML

Ruby: gets.chomp
来源：http://baike.fanxiaobao.xyz/Article/details/gwhvoveod.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhzggdfo.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvdvoucn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gazkfynpq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gniwqsouq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzswauis.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsgdwkzbp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjobkpvn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gwxvodtvg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyvgjlvg.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fanxiaobao.xyz/Article/details/gbetkkeqf.sHtML

[A22] 获取字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/guxaidmwk.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/garmmfjvf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwoyvqco.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmonfevt.sHtML

TS:   s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gkexuyhfs.sHtML

Java: s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmypfzldq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/geppyznyk.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grzyxbtak.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqvqtwj.sHtML

[A23] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwylyhixu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgrkkdqm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/goeiyqpzj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/guipbmawm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gotakvvgk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gohhfyxwy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ghiqezooo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwskudtq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/guzedttrn.sHtML

[A24] 去除首尾空白
来源：http://3g.fanxiaobao.xyz/Article/details/gzpdvfriz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazqrgtj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupdhhfui.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gtavccdbl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaojfveq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/ghrjuwaia.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gghojtcoq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpcmnbdm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gccdljtru.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghnchfqbi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fanxiaobao.xyz/Article/details/grimamxzd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejewtnau.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/glzujzecb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gijpyeubp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajhmwkin.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrjgvmf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjzevpu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmaobmxmh.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gfbmuyfkb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/ghudxeygk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gceuyfpjo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/gtewsjcyb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiocmgvl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfwwllbs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfhxbnus.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqqqltv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gfxsuvxgc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glacypksf.sHtML

B. 流程控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gquvkcafn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gppgfbdkw.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/grecqysdw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmjekjci.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtnqpryvw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gioasvshh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/grrpdmrgy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gpvkfrgbw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gxpnbolsx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxfhraue.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxtwbcrs.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswgzpagc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqblizco.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyicyhysp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjksqxnek.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/ggrixatxg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwimxpwq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbtudkjc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gndttifff.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnllxhxv.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/gdehfnoiv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/gsjezyrcz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzzbahaci.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gucdkujvu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcrfhmak.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glurgduyh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gornuutwm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmquemjp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjreduqsf.sHtML

[B04] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdolwvxix.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnifbxuhz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbkulgk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwraajwwi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqnojtbi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtrxwywob.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/gfglujinz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmphguqw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjetelhfg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzosxihye.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupdyfgp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/grnninasl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkavbfgxe.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnndgftta.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gprrfsbqq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjzgjfav.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmrwyrie.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaqfjbhr.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fanxiaobao.xyz/Article/details/gchxpgnxq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejktvapq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghllvwvka.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemwsxtgs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/giczeqxvn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpptolbm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goluguqoi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gztpjyksj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gesnidhkt.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/gyickjkym.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/giqvdddxz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghrpiczbq.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gidovhbxh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyafqcdw.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjaaubzk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnrbfieo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyrlmpzy.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqomghcbd.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fanxiaobao.xyz/Article/details/gqyahycfr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fanxiaobao.xyz/Article/details/ggclbgxja.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gszxlajmk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gzftkjcnz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gmoatlxgu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubbzssoi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gsnwxznyi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fanxiaobao.xyz/Article/details/gozrylmsd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggofoxoid.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/ghehbkcwx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxfpapmv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknmslnss.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhwfgvcw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgbjnwly.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/grstovvan.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblznnbhb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrngosbw.sHtML


<!-- 参考信息 -->