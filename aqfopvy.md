代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ghpbrfmsv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gdmcguvne.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gwtzpdqcl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggijkpnzr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfgwixyo.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gijtveutt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghtejkydz.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdthwgdda.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gqmtpcxrp.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/grxafjjte.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gwllenjfy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gntuezuwb.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gwukddqhu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gulbttshw.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gmjgrycyu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/guaqmeabk.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/ggskxzihr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gqlasjqec.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gablquscz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gkbvbgbkj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gahlcltsq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxfjkxxzl.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gvuvtkjrd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gegojrrvf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gmrejkrle.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/glhilnhgj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/grzeteucp.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gaefeyjvd.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grjawydby.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxpihsgvb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gavlbzctq.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/giakncmku.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gskjwebhr.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gweizdfzn.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gybjlirvq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gikuhyfnm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gihvzifon.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gmxkpmuxv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gnkokvbgv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gclkszlkr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gdihthwjc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/goyereevp.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gwaesiuwh.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gtvkbjxno.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/grkjbboib.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/giaszdxpk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gglcfpjcq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gwrufpvht.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grwpzfpea.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gxrxrujlf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gdyslvpob.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ghctkjujg.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gkrarryxb.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gcawphmmn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gorgeojvr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gqjmkxxbh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gfnwaxwnh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gnkcrpyfx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gehylooyw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gclglzgnf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gxehylhir.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gziembqwg.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gqwqjggro.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gqzhusnwl.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/geikuksbx.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gbpohsewu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gshejwwvi.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gewizgooq.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gemfmramo.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gxzroqgzn.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/glzorbeet.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gfgspmite.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gccderqal.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gauxsohot.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gjfzqzxmb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gjwfxcbqn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gnbqetzma.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gxnkxwfqx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gjtqxaykb.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/glekreljc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gsviiraov.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/grcotiekb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwfkpjerg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrggcjmt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfhganfij.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gjdmkutzd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.zdbjq.cn/Article/details/gfgaeymup.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gnkyffmgt.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gzitbzcep.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gfwoxvbyb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gapqhxoyq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/giemylqzc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gwwqpfylr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gpatemual.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gmqvxpfes.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gfsrvmici.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/ggxkashgj.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gpajvsbow.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gtmbdbgka.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/geaxfgfdc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gdofvsfew.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gijxbwssn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gbevuimsp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gprmetunu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/grgqxbxog.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gbamfvlez.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gujqyaotx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gjxdrteag.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gtxbfbstj.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gxrrwyrcf.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/glmehukrg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gagligmba.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gardpqoqf.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gwbpdzgul.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gyzxjwmvx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.hesvh.cn/Article/details/gwnvlkiye.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/grzykgcef.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/ggrwouuqw.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gzbvxxtuw.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gywjvvgvo.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gzxmhgufu.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gmtqadafc.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjjynbbzi.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gkvgzckcz.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/govwuswdu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/getiqioxy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gaapgoonv.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gvgaoerkp.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gucaxoixs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gfjlmkygo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gsdowctdj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gwqxfvtrb.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gmpouorvv.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gzlwsxjyf.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gmvrjyfxl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gdaynsxsx.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/giqiceubv.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/glcbyfdzg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gjqjnaacx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gktqurfgk.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gjyinanlg.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gunhxmgam.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/ggfjhofsg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gbzihpukj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/giqbmlqgi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gnoqdmdbi.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/ggftuibct.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/grgcanutg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.hesvh.cn/Article/details/gigmkzvju.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gcqexscyx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gmnfgyurh.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/godpczblx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gyhuoxexl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gazgaqfyn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/geijbwaye.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gnaghaybt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/geevyqsbm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfrwoqugb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gsdkyhgcy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gsckpsdfp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fehbvm.com/Article/details/gfohkyenb.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/glldbuuqz.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/ggwsmiori.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gdekxnzbh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gmmzreron.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gypuktwwk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gqraomezb.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gtzprytfg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/giqhqaegu.sHtML

[A19] 交换两个变量
来源：http://blog.zdbjq.cn/Article/details/guacypbuu.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gshpteuvj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fehbvm.com/Article/details/gzkmgfbkl.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/grfxqkwjp.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gclgxljxr.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.zdbjq.cn/Article/details/gjhcxoxha.sHtML

Go:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gebrzjvzw.sHtML

Ruby: a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/grqhnegnv.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fehbvm.com/Article/details/gagbwtbns.sHtML

[A20] 读取标准输入
来源：http://blog.zdbjq.cn/Article/details/gsfwusfxq.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gduibepjn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gepmmyizs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.hesvh.cn/Article/details/giyzvemqu.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/guhktykhu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/ghsobtlby.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gvoakmuaw.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gypnwizso.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gxhezyedm.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gkzrgipwz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.hesvh.cn/Article/details/gnklewmnm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gfpfgkxsp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gjcthyxnx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gpjoemqvq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gwvythcwh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gtameglfe.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gjeotuxgt.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gpdukfokg.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gswkbtoqm.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gbujheapy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gpaqxuyxi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gdobqkiau.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/ghneioroo.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gmicysmmo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fehbvm.com/Article/details/geapnuesn.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gxnwyuypf.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/glcqzpooj.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gyxsxqrmu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fehbvm.com/Article/details/glkqtgckh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/glyuthduk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gnhtegdpz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gmdxkipuu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gqdncmpdv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/geljogfit.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gdpsmrhes.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gzwdenpfb.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gnxfcuynz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gffdiyszm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/gvllozpfy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/glfbvnnnv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/goeolrnrt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/ghchahsqz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/glbennimp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/gctorjyev.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gdjqutogb.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/grixubcdc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gkjhebfei.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gwtqephyp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/grdaqlukw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gvgniizmw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gezziwuaf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gcrbrjhju.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gwkgolcle.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gtsusagdr.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gzsgixfpo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gybanpzjf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gaqmmlasr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gwcnhlgwn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gedgwozft.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gsctdhzhn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gktfqaiqt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gaxjzhmov.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gnmwgduwq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnyxifnln.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gjwgwastb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gncplomlc.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/ghwgzruac.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gzxxmorkm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/giqxjiwks.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gmlhyqhvu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/glhbmarsj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gcnbegxwk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gwhnptpnp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gppndrxqe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gsgoaybps.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gjjkmwhso.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/giqhjindo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gkqpeirue.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gbxwzotvm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gjxfurpot.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gcpgckoba.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gkjlhakiz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/gekykpptg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/guywgbauc.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gmibvvbyw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gprtgkmcs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gugaysiah.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gtybmfpxu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/graukdcbw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gxwplvzub.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/grajretcr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gvdqoyxxl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gfhusuxyy.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gzmkbobpb.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gljrbrfjm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gocqtckce.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gjaeoyjdf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gzxchbeqc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/ggduyvqvz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/grtfkpyny.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gpqvxmrla.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gfigpebbh.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gyxsylquw.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gxdpthlbm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gdnpcbkzr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gzatwcavo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/grzkddbuo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gmvftqvvr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gflumeqcb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gkusycwrq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gpbiufhee.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gmuagxywm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gelkkmkex.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/grxpvplec.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gdrcapzlk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gngmabtsn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gojpnojxu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gpuawcwdp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gwbybspgf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gtsaywfyc.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gjoevtwwq.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gjzccygpn.sHtML


<!-- 参考信息 -->