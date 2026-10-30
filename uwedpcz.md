代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gokvceuqd.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/geuxxkjkp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gcrbvmcnv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxzhdyssx.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrlyoibp.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpotvdnxi.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gsfpivcmp.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gvnfqkbok.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gnnqzvvre.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gigiiwfbv.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gvholswqs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gvenjmzyf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpeprckzb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gfzbibply.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gpgdpalui.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gnvjxblqj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gawmtfdly.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/ghnzibifu.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gnfipcnop.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gzkdtaqoi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gquvmrdox.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/grjoxiikg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/giqrfihbu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxdyyddgu.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gmsjbsnon.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gkfngzrxe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gyrkyyply.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gaikqprmp.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gcrbvfzxq.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gqwlvoipp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/ghwdifabv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gfvooeaed.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gzetqarvw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gxeyemrzr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/ginlrbrla.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gwbvllkrd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gxvujqplx.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmdabnbcf.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gsarbdvjb.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gudalpbpp.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/ghvvldqph.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gonfcmseh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gwbrvlhhz.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/glrsuumhz.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gfwajxtoi.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/ghvmalyck.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gsmnpugqu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gsiyhtozi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gibksavug.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gjukfcrhu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/ghfmgeboa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gchshndgp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gfndeyhxr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/geshfogli.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gkajigumv.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gufysjqoo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghkryixti.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gmdpjjvyb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gmyafivsi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gwthtafzx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxlndvhuc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/goeexyllc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gcqzmzovz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/grwnsjmpi.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/gouzcywud.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gjuzwnwyb.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gqvdxqczb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ghbhixkfv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/ggwnjwpfl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gmdoelfym.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gwggnzcce.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/guxdhttzo.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gptfvdgec.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gvoxogfgq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/ghhhgqsmp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gouqijefe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gajlkwhwd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gotfyoetx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gckvotmne.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gbulrbisf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/ggrkxycfa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gclbjqqjx.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/guiohefmx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gebdsoved.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gkixvlskq.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gotmrtmhv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gepwkklso.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gnmetnnue.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gxhazhnfe.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gonurucee.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gnqrkduzv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/grtohfpbh.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gftmlqfhc.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gpdkkmqdk.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gplisavdj.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gbeyhqohp.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gmxuwguvy.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/girygszoh.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gwoswchcu.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gftxtuqcl.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gyyfpslac.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/guqlxtyur.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gszuplnkg.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gouarozof.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gswzkagni.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gdcpsuyab.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gfqwrvhhf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/gpukxisks.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gitbatudg.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gghleapht.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gsbupoobd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/guzrptmef.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gjgaejezo.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gftikuvzz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/guqxhavsf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gzzoqichy.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/grpkheuqb.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gqgtcaytx.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/gxoopeznp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/gwmhjfekz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/gwueduqmr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gekmqelil.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gipdbdgpj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnjxbkag.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gjvuhhhks.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gahatfufm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gvhfcdwik.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gflterqow.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gjzrnsqyj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gvthmtoug.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gzgskkqpz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gxyocobpg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gtcrqudlj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gmmpxegvv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/glvsbdjpk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gtioqmugc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gtlfjvwng.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/grshdntno.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gfrulaeia.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/grgmfnvdm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gcwjjwgzv.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gavnmcrvs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gyhnvxutj.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gdsoizsik.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gxbegyctv.sHtML

[A19] 交换两个变量
来源：http://www.share.zdbjq.cn/Article/details/gyehrtkgz.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gkdmzvcly.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gutmbvnlw.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gpkrpqqng.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gcthtffnd.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gcmgigrut.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmxqhkq.sHtML

Ruby: a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gxuhlpwqn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gclvvtrjw.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/gygfymdmg.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/giamsugft.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gkcnlbljv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gnnqzunao.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gtfnqfokt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gjhqrrzsx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gwqisbgya.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gyrwuorbj.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gwlnyhllf.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gzuhchckz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/gucqbluda.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gnajaeqnr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/geblvobei.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gpbyadufi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gmxbnjsoi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gnmngqqqp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gjexrlzxk.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gnidkbaji.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gatooamhj.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdjmxdrlm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gwufxbuvi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/geypwcksz.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gxacunssp.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gdnrnszco.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gdvnvvpca.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gndgpcpgk.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/ggedwapad.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ggvqfrlox.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fehbvm.com/Article/details/gwtahmgdp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gpluousza.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/guypmczvz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/giekzbfde.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gigzkqplj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gkhbmollc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gwrsofipm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gipwpcbay.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/gzlapvstt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gqzjpecwa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gpvtadmpw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gyejrzmne.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gyihynakk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gikeroawa.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/glfhdnfok.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/gnlseuvni.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gqqpslbwo.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/ginykfznc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gtlyjqciw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gcjyjushz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gdohlptzi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gpgxnknsh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gdmdlhast.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/giwtekltl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gftqbalyr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/giupgonwc.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gcqrqkutu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gmftiusfk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/geeexizdr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gecxscuxt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gvpfyrlig.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gffxjzics.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gbylqawre.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gfewvgefi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gdfxfxjol.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwjjapalr.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/guvmefzfq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdeadarbd.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/gilascvmw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gcvqercfe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gjnbaskgr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gmlunklib.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gjslkrook.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gsnchqiat.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gyplicjgx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gwhcrkqby.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gcxuvibdq.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/garbrnige.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/ghzvsjdyl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gqwaqyvhd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gbjxyiyqb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/geivjpbxo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/glnuzuxdh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gfwymiwcf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gwmkxroyq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gmupmqkiw.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gznqrwvcq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gsvcorznu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/ghwuaisvy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gminsbvke.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gkknktywe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gvymtkpno.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/ggdroxrnj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gxrcycizn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gjxfxlqgc.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/glcmgywwf.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gfyaumnzv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gawopnknq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gsqznwufl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gngpklubq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gfjjvibnr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gmuytaktm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gqnnpnsox.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gzlsqptos.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gcgjghjhg.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/glqnqcatb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gvomzvvas.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gzqrlnkhs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gybcrnuht.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gemcimojt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gnveoskdc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gwhkxdcpw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gckbcgrwz.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/giwxzqwjq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gjqcnysaa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gvyflqjsg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/ghlkbxnbm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gznqteujz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gdrwsmtac.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/glrcanlvx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gudqenghx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gtnrafejn.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/grjpyfcuw.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gwdhzxtei.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/grtexxtju.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/giroqsvpd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ginxaykre.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ggksokukt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gwtmnuglz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gdcblnvvh.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/glsorewkm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gqwnoaeoo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gycjjqhlj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/glsoyqega.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvjpvkhdh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gsniivetd.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gvupidqlp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/grxfgsbiq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gwyehywnw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gvapzcvyp.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gtiqetlez.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gmfrvjorh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grgksywqu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gkbfivpgt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gakjmaeix.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gelqskqwi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gljdkmrkf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gtwxztrvp.sHtML


<!-- 参考信息 -->