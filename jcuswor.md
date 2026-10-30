代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gxgwshpfa.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/glfoggnae.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/glbfvqmkd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gojylkccr.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkryjqcev.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmneubwne.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/glnfieuct.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gkeizwebw.sHtML

Ruby: PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gsqnvsrdn.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsttpvsik.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsxloeyw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnenclufq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gobuathnv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gupejmrgg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnuzupwl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfuwwxsx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkepqszzl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/gabrobcuk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgsdpchj.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfbaphwp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvtedowkk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkpjxmtbs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpqtkhad.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzmgndtp.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gakeakrsl.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwgroilj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goggbvrqc.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzilncvw.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkorrlk.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gacqkcehi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhxezsiz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/guxpldekq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqouhfewy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gmtxdinoi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gioduytzt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gnxdchqau.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gainxftgu.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxfgnyxo.sHtML

Py:   str(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gkeaetayx.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gzvfwzzju.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gukfwfgaw.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginwisvha.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdftjmjec.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhantckf.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvqebbhk.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gcopjmyjf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqtfdawz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnysaeyke.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyagisbih.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzjamoge.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjzfzis.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gywdloozy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gndqpbijx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fanxiaobao.xyz/Article/details/gkzwjhets.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkmavowq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnuuskm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevxbpqdo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwuhpdtz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcprmhem.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsrkovrj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvijasou.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fanxiaobao.xyz/Article/details/glbzpumoa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fanxiaobao.xyz/Article/details/grjiynisq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxukuxog.sHtML

[A10] 生成随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyikshvsh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxxagnwf.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycjdxoqy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblcosmum.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/giqdgdzlq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsqvuwfd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gifcehrjm.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/gokxsprvb.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqevausqj.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/ggdjuwwtl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxpmcbxm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdteydef.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gesihyizu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gxgrqvmeo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmxknbpw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkscwklcr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gpwmrcvkr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkprgppe.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqladofnw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzoyeqtqg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbulrwcg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwfcigjo.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/gffrmuuwi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpldbtxm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gbhnrefhu.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gabbtbpww.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnrwfchq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fanxiaobao.xyz/Article/details/gpokouowk.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gewizvemr.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/ggxgzepse.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpybfihs.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdcntyyx.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gupzeouwp.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzwaqdgs.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gjhiduncx.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxytkin.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gltdzqssw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gyusgbwvy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gfczegzso.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/guqxmhkme.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ggikbjzdy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gmfaupugm.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzgjiuld.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/gxyxutllr.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/glnyvugda.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkhphbya.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/ggqykixjd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gsmyyhkct.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gepftovpk.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gauvgjnwg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmcasasa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxnatrsj.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fanxiaobao.xyz/Article/details/gyygykpqw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkinvlyon.sHtML

[A16] 真假值判断规则
来源：http://baike.fanxiaobao.xyz/Article/details/gebugzmvx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmabzvlv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/grgannrbv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfvvksj.sHtML

TS:   if (!x) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbjugpou.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnsuvesvq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqojtuots.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvloehoj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbbprjck.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhxpjzqz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvirbjys.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/geoalnqge.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuyifrtb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gfskbcfru.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctvfwrty.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjvwjnrm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalzmuuj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhevifxu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fanxiaobao.xyz/Article/details/gnqecqvnh.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fanxiaobao.xyz/Article/details/grpmzrokv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwugnrrvu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gencyrzuj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gwdtwpxvw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmfeyuhf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwewsvyae.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gmquoatef.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fanxiaobao.xyz/Article/details/gdxswpxaf.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giciyljsm.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/goynmfacc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gvmklbvdj.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxfmnnn.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqcthyjt.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxbimbmj.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpewnvrk.sHtML

Ruby: a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gtiozptrt.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/gxcozcsku.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxntwlda.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvabdbehv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fanxiaobao.xyz/Article/details/gjljrmrjh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fanxiaobao.xyz/Article/details/gnspimupl.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gzcnckkuc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdbwgnfd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrfljltv.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqwwjkmn.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcuitgyk.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsaoqgovc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghfxwtzyr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdcrztni.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxngyyjz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbvqtws.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgzwrcli.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwlrgiai.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/geysbxolb.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gticwalgy.sHtML

[A22] 获取字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsrqbzoga.sHtML

Py:   len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gamelgvpp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzgmkaz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/gnvmrbvot.sHtML

TS:   s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gllosajjr.sHtML

Java: s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gizfukfhd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopckwonr.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gckyxpdba.sHtML

C#:   s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztxtkfuq.sHtML

[A23] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gujbwrhrv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/ggwismycr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fanxiaobao.xyz/Article/details/grnnfptgo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gadihtpmm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gurmvaepv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqoavmw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpjyboyx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdoqlsed.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnxpvflg.sHtML

[A24] 去除首尾空白
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxizeokn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fanxiaobao.xyz/Article/details/giumkrvra.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gknoashyu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gccvwjgie.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/govjkmavo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/gtyctvlox.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfufvvoof.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fanxiaobao.xyz/Article/details/gikclrdpt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnqluhzf.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtkilwnju.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fanxiaobao.xyz/Article/details/gswgkshjo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmeyrjnh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemrzmjhe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/girnahpuk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejxpeqmx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggirlydqn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fanxiaobao.xyz/Article/details/gbvnbnyqz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnlywamf.sHtML

[A26] 类型转换总览
来源：http://baike.fanxiaobao.xyz/Article/details/gdmchrerv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrojyap.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fanxiaobao.xyz/Article/details/geyoihfen.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fanxiaobao.xyz/Article/details/guedycqpv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnmibsfs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvavhvxbe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fanxiaobao.xyz/Article/details/gsjdjxsoz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gxmevpxdv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwgxdyel.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gucpbdpvy.sHtML

B. 流程控制
来源：http://3g.fanxiaobao.xyz/Article/details/glevxhtpw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtqyrrqwe.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/gwckjzdhm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyzmoukb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxqhinbn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gcksofbln.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gnlkswkjb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmtdowmf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gknfzazed.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gkvizuvdk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzhtfyik.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzpeaktm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fanxiaobao.xyz/Article/details/gccwjrzvl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvtxsibcb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdfnurhs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gsaowghpl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqfxlfkp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/gwzpqelzh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fanxiaobao.xyz/Article/details/gexwcofyu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhfyvsop.sHtML

[B03] switch / match / case
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkpqdgia.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fanxiaobao.xyz/Article/details/geciskaur.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboibmpym.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxuzbbns.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gowbpcfhs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjzkbtgi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/glvlktnrz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fanxiaobao.xyz/Article/details/gbkjrfhxp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gfzjnxqoo.sHtML

[B04] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpzdcwfr.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsmbkwss.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnagenobr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/geoiromlo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gniddfrny.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/geenfxcwb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthnpotah.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fanxiaobao.xyz/Article/details/gybhdypuh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkiydfca.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gcksdopov.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gadmnbzbu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxqbxhfi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gstyadlvk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpupwdlsq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guesqjsvt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgjzsugu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggshtzzli.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghvxmxopa.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gprztdrkd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fanxiaobao.xyz/Article/details/gbmnjiqrh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaedywtb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnhkduix.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/geausyuqx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuwoifwe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxbmsyaa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgpbymzr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjddbsalm.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gyesfrkcd.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/guazaoszj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gseoythwa.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtpcapxpg.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfhueqau.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzeonlgnm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gnelfxwyw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/gvtwlihww.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwzfnwfa.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fanxiaobao.xyz/Article/details/gbriccuiw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/golgqvomw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfthxmznr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gapkzqygk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gubuxkhlx.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrhnnrtd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtvcnyml.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gflaalywa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcunrhhc.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmonjrevo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmsrwiwx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqrvvqttm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glixglhih.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/godqeugwm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdesvlthf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gruwdrzfs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpglerfww.sHtML


<!-- 参考信息 -->