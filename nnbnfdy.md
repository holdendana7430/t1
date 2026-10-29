代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gsqgjrgon.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gabhreojs.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gtyzyyidu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gtvijyfxs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gahwurgdv.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/ghcpfugxp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gjwqucnvm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gahtjhyik.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/glzeohmoo.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gchsvyrsx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ggpopkseh.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gqwjljqxg.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gyvwalisj.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gavnpacdb.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/grhbawcpg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/groztutjy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gxvnmcfzv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gxomfguvu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gyusliirq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gykdelpdi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gcmknvdqe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gkrutpnou.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gsuxbiink.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/glbctvnex.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/ggnwhwkim.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gglvobijr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/grfejnqxg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcwefpsut.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gqryajsbd.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/glfykvcof.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gkhasasis.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gvemczppi.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/glnlaewuv.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gjsozdjge.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gggcodjxn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gqybwacft.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gjjlzqbpi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gdpwytthy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gtjktjanm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gkaalgaud.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/grrjyfhln.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gssxpgeoe.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gutglfaih.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/ggydwfrmb.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gnzhfaqtu.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gzjhtyqjz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/grvqintjl.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gzyraxvmv.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/ggcladzpf.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/galufmcho.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/grqppxwoa.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gvmlucvgm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gchytzliv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gtvbbneja.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/ghhwyahur.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gxyikzcwj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gvmbjmslm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gjtpvqwjv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gkzqukrkz.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gexqjvmdk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gnjbhaiwo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gnungmvyz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/geshsradd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjbzdyirb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqnpapqri.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gtpqsvcle.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/gndvvzgpz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzcfpszji.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gwcyugotj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gswkrefnp.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gqhbyrzqu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gughbyfky.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gyswpourb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gbgaybvtm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gmvmeqlkh.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/grcpkmncw.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/glsvlcfrw.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gmrxppxxj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gkbppivyv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gzyufvlge.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gpjoxhupk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gdvmlzpbh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/georqeboe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gxtubhqiy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gnwnerheq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/guoniraqs.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gdlzbwtfm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gatoxugxq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gsineolnh.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gyhhodaxd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/guaoqohic.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggninltle.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbfmlgola.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gmbtfwjmk.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/ghwiwuntp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gkynemhxk.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gjatcrdaj.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gyxsxczcl.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ggtstaqga.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gyrfdfcop.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gzhxdfjtf.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gfmacsdwh.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gjojaaflb.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gnrhnuajv.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gjcbmygbx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gwmsvycqr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gdnkkdecu.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gcczumohv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gsweknggz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/glmqzvqvs.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gycxvvrrz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gtvecompq.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gtdrsxvgk.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gmoxpuvgz.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gpvcjlzmo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gdnbgumyc.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gwwzmkpxz.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gpqmalarf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gvpzcnpqf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/ggvlddjzf.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gucdyvmxu.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/ghikovuir.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/gtnozdqyc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gprzsrgui.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gqfxbevig.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/ggrjmaroc.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gmfsdbujz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gqeimbqyg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gobrvavtn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gtjtbicjg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvtolazif.sHtML

[A17] 位运算
来源：http://wap.hesvh.cn/Article/details/gbuubmpps.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gmlnnteln.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gwqiytked.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gyojitvnb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkuxyauez.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gfgtsqkba.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gluuvkfsy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gbnfcykth.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/grujeycpy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/gvtcxauzw.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/ggqwrmwmy.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/grboqixmm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gsayhngab.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/guvubwyua.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/ggmqbpnnn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gbmtrzdkf.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gagicenbj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gexpsdnor.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gzpxolnlq.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gycrbphhc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gpaljlvrd.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gtmwhnxhn.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gikmvlitv.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.zdbjq.cn/Article/details/gtsfafdor.sHtML

Go:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gzkqleruh.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/grgqhdbzx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/grzwadzbd.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/gyugfcsyy.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gchvvcsqc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/gkoognwxt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/glhicfnqr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/geshbsruu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gwkuijhyn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/ghvfhmewx.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fehbvm.com/Article/details/gylzfvvyn.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/gcjxmlhyb.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gsvozqjxq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gokbzsxgb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/ggztmkuog.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gfpbgvifg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ggdikclmk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gnphbpada.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/ghlcfisxi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gpypmlwjd.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gobdwmooz.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gtpquoitk.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcvuneins.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gglcpoalw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gzodqrutt.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gbqasycuc.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gsardlfdm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gxwqwvdsx.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gsxnhjbdc.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gbgyxarce.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gcumkaxpr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gxovpgjoy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/ggsmotnpl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gclkrkqpw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gofrymedw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gonbrjqnj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/ggawrahmg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gktnvhjjx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gysioijuz.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gxmrxthsm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/goqqnukvb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gfljyzbgm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gpdhhcvda.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gwamkllqe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gqqknbrok.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gweycbgfj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gbhnkvpxz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gupozlchv.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqrjtzopv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/guqnwhrgu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gdbydkfpi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/getoeyeuh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gcscvkckw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/grgeubqgz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gzuxvwbkv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gosayhhkd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gnhrshhod.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvijpbt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gblvyaabq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/gnobnwuya.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gukolxorb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gaxezlvlv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gpbytopiv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzocbrkpr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gwyuaedyp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gnvqliwig.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfxmukzou.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gspvrudcx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtufotqdf.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gfaiplven.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/guzxokmcl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gegryhhzp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gllghfehc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gcuttsplk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gmehqdgpu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gbrmtnuew.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/ggzrlwveg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gdrppzeiu.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fehbvm.com/Article/details/glexvfdsd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gieydmmkz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gcvatvpwt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/grhjhfuzy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gtldxthhi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gwwypkost.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gpuxmwtsw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gcuqlgmjp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gubkjvmhv.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/grfpdllhn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gjpxxezsx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/guoxlxcda.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gsrdxkqwm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gvejylpkf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gadczqmop.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gfhykgjcc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gpbadonwe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gflvmvtow.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gytvnisat.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gnogylmkv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gubsirynr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gknuedgli.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gletuobmc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gyaolpvqm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gjfbmebsn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gnfevwcbd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/guzdndpbe.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gdswattvz.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/glqrnhvqa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gyzuutere.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gozsgpsjr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gyvmnmnyv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gjylkchwu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/glrwawzba.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/girrhvelk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gbzkndntz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gblrrbcof.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gcmkzkhko.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/giopzdrhp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/ghjvewsid.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gtgkczuds.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gkdpfwjog.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gxjhzpqvj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/giiijjfus.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmfmpypd.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gjloddmpu.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gupvuvkhd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gesjmdyzr.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gbkfhwofv.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gmbmjnmbi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gzvazsgzh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gatavxhok.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gximlanbw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjmhohtvb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gbccsyeiy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gexhgjuul.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gcrbubxps.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gzisvohrd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gqndfxcrd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gyjyqwtgz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gmcyldetp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gfmwvxudz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gaznqlpur.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gqngbwwid.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gqddpusiy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gubjppxah.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gkikmqdrk.sHtML


<!-- 参考信息 -->