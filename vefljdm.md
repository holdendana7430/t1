代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gzytvlbqz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxlahia.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gxpypdisb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gfaggydbu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gjvhykcxx.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gopmygfle.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gshwanphb.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gptegzfmb.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkjxilhrf.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtbicrxaj.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gufiqbcov.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gafzmtypy.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gbbvdbaqb.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gutrglcfx.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gdbvloouo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gqgcumxad.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gnsuwqqxp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/giwaypnle.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/guzbfyjuo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gtmhycuzw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gshihcmkh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gzbjpqpfa.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gnbkglicl.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gpquufbpd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gxojggjfx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/grkgbwdek.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzjovnvzu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gimxpsqzr.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gsjhrogsp.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/guqpthzhh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gtchgmonv.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gnnozlpsz.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ggwdxzfvt.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gkvxbaamw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/ghicgtolf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gqaixbqux.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/guggjvrmv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gffbpfqra.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gahkckzcn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gvvtcktgo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gbxsoakor.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzpuzusnb.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gxtigmeem.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gfgjukyjm.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/giktxynes.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gvgtfrkfb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gfniaxhtw.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/gbhhhrmlx.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gpejqhgez.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gbkufeamk.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gzguihvnm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gqscrrdjw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gyfnamnju.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gsvtzjxoy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/grkhgruow.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gijidtcqf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdmwktdx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gzovmrzrz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gshwkuzhf.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gxhlhqxqe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxzzsiani.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/grikmdbac.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbtryvzgx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gcxdnyfle.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsgbqdhrd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/grzohzesy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gvinnqcua.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmzdhldxb.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gxbretyjc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/goyubvhnx.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gamogaqmc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gviqmruqc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gaxvkwywa.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/goperqkmi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gwmfyglto.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gpdqkyole.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gecuaauiz.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gpimvjahe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gwmffbmca.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gffqwbszf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/grwcunkie.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gkzoeqneo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gptqvhcuy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gwfyhaiot.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkcvtlvpr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gfabyjssg.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gmizbmelu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gbbgixojy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gkopijnyb.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/geoynzerp.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/grjcpqwps.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gtsxazbch.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/garuoklcc.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gzvyufyhg.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/goxzkcmor.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gsadsfpoj.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gzqmuwbkk.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gpbfamiql.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnqsxmeeh.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqkzghpzu.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjqzatoji.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gowyhbjqt.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/guyvxmrsn.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gozckdobl.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gmxfpuikk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gnkxpygdw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gducixetz.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gpjaxfqtt.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gwjfylrsz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/gifghnyrx.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gzxlzzqls.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/giqmuqdey.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gjygrfmqu.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gjgiqlfiq.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gwkgymbbm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gnqhmwmwj.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gjiqwnkpj.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gzwsfxmgi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gwxwlfefl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gwqrlnvva.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gxkwlezuw.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gtfpwxedj.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gtcfdahub.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/goadunmkv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gachtinne.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gnbqcmust.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/ginotxvrn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnhteclng.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gydztzakb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gypyzsgye.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/grrymlaxs.sHtML

[A17] 位运算
来源：http://wap.hesvh.cn/Article/details/gqwndsqec.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gzvigddjx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/glmqtgtpm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gxleobzwu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gdmwzzdyq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gfqhobnlv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/goeowrjwn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gdnetmxhw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gxhyftifq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gmzqsswkz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gofwclqke.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gnqutkloe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gbvydgkep.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gspijlcij.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/ggpfjolzz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gorglxjxj.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gntidrhax.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gudxwtwiv.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gesnbhonq.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/ghyyvogse.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/gzxuimbks.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gymxyzblq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gjfakxdvx.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.hesvh.cn/Article/details/gftkojmmc.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/grqctplyn.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gioypgwgj.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gmejrjhqf.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gxaimettm.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gxcgfrdva.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gutjyhmis.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gfugrxlln.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gfqvozdib.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gihsrdbhc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gbbgwvvkz.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gxfmimywf.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.hesvh.cn/Article/details/gkrhlkpok.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/gewdyawgw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fehbvm.com/Article/details/gqofzeeda.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gqrvotuik.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ghdtxykid.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/glbcjwmcs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/ghbbrcbly.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gpqcocynb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gawfiglug.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/gljqevqys.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gphfabcoo.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/ghcqcullc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gvidluriu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gaedzdjzb.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/ggkyohlsp.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gahvpvnit.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.hesvh.cn/Article/details/gdiimhcjo.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/gjrxujzbo.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gkbjttyhh.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/ghdqgguck.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gitvpjuap.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gvhjflbao.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gjpvulsna.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gddbhwvom.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/guulgorns.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gttsujjgr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gjksakpnl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.zdbjq.cn/Article/details/gmpysjlbt.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gspqmqdja.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gbqnwisny.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gqnqycpkj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gxdroyeas.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/grwmuamzz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/gmeynbzyb.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gklfurplo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gkwpksnie.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gmghbuqoo.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gyyytnckd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gftfxbkfd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/grxyrpcds.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gmiiilwhu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gdrppwcdt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gocojndvg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gxymgkfou.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gpcjgtgjt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gicbclejd.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gjarzptla.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gcjundgej.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.zdbjq.cn/Article/details/gvqeyswyq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/grljtusft.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/ggjfqcmiy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gmppioeza.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gwrnfikio.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gfqbylbkw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gzfuwbnhi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkjqnumti.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gyeawusfh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzjaeuvwo.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gvuzyzydm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/grspbmxhs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gggmvemdp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gvqspjjff.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gpqypqneq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gbriwutxe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gdpajsptl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gxjtqpthz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gnjydaqiz.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/gasotixlm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gqlbnmzuk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gzmucaksk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/ggorkzuel.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gmbpzeteg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gvozcntuq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gfvngiret.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gedtisgmu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gbxuierju.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gribhqlxh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/grbqmkjdz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gnwumyzvt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gandelywq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gqzdiagrn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gxyqilhau.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gnnoiqavf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gvlviedyh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gjuvrysyz.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gmzmfzeqx.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.hesvh.cn/Article/details/givpscasd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbaxatvwr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gbsuoyrqv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gxhdtblov.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gebpjniae.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gehvhjwxy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gzmwaknuc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gswushgbg.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gvmvdmakg.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gwmqgxxkd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gcnheyrzw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/guyoihmwp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gvefagnuu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gtyhrbpkd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gvpnblkay.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gexjornlj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gkugamqin.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gccyphcpk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gjxsbikqu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gglgbbrdh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gsgmthgsr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gshhehprh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gdvhoheas.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/geihaslhf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gqhcrsyig.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gqekcbbpy.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gxrfzeyug.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gorukchdb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/ggvdngyvn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvftnego.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/geubwcqlj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gfzqpzjpp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gnrqiwaqz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gclcuqopy.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxrerfxkk.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gguptropd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gjcxrmgwr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gwvrrvuhb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gcowwrpai.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gptfciwzi.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gxlhzlyaw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gniploilw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gxyramcxc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/geozwyxkg.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gcoswlryg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gxxzdurfo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gppyxmipq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gczubhgxk.sHtML


<!-- 参考信息 -->