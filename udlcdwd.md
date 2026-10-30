代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkygxtgc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grjawjqns.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gmcucuypi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gthnaifjo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhppeeyq.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/grnjrbrol.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzsjjhoi.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxjsyebqo.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbuwultl.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/glehoujzy.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gydhyasfo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/gizznosnr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgwfsqfk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdbheffj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjulqnzu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gdoionnqg.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqoutyqm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpepuckcn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfvloqjc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhnoraqo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/grlgdjclu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gfylygeeo.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/geqcgebcx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzgrnxst.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmrelykn.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfixrlmfo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdggooyl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzjvbqtb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gegrcvjuy.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghjtonlyj.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkifwis.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gshxbgslg.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfozibcc.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grfcijlyb.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzfnbtwst.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/glscwjgjm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocyogdes.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gcrbhtqxe.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjhinkbk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqramwkvx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunnpmqyh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmemwcl.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gfotyvria.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gbvctjjyi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ganuhmgwl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuhnqzzf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gczzdskgk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxhphjzr.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/govwkbacb.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gsxwleibd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gaqwwjgcw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifbqzut.sHtML

[A06] 字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gpnfetwpt.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkachjtln.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gbuaocpuv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/grmxwjvrm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/grwqiamse.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gnqcxwlkg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghajmcnwl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczayexpr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/germeefia.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwhrkcrz.sHtML

Py:   str(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhqznsrz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjzllzlp.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzopehqkg.sHtML

TS:   String(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gclqcqbki.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gnealxpcb.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjesjqxe.sHtML

Ruby: 42.to_s
来源：http://www.share.fanxiaobao.xyz/Article/details/gokexaubx.sHtML

C#:   42.ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/galkdocib.sHtML

[A08] 取整与四舍五入
来源：http://baike.fanxiaobao.xyz/Article/details/gpkqhgelo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gvjqplygv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaebzvzba.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gskghwymd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fanxiaobao.xyz/Article/details/gmflelyom.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfuentke.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrzpsdtw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gqhzqpaos.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpstbsvru.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gfcisagfh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfeiuviu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gasqcuksq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguamhdfc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwoypbwz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhxmydfn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gdejfxgdq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwysbesse.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmhgfahq.sHtML

[A10] 生成随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmmowszf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdsfqvfk.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmtjpndl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/ggkxoufgw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/ghdqsstpc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gfrqkxnih.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjhmcuem.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/gtccrfure.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdlbozaz.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpypigyju.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkkvxigc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpcdcvlu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gxkspnbyn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gcxzklvth.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gzndzgwyl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/gfleuakrh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccxwris.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gfmjpwims.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvdmhpumg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjdejrwf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsgwovzh.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/glylqhbbu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrzieeyi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmqbgsub.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gitbnfjki.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfpqlpaj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcqhxzck.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gcsgjjhwp.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrfwzcat.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gwhmjmobf.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyvvngfk.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gntxtwugk.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktbrlskl.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfpoicfg.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gakkimucv.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxhgxhjx.sHtML

[A14] 注释写法
来源：http://baike.fanxiaobao.xyz/Article/details/goxhzmaej.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfopkhayy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwrphqrp.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gqggemwov.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginhxpupc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gudceeusp.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgilhsvp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fanxiaobao.xyz/Article/details/grivjligv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhkqxogz.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqmczot.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gizghnvrs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gddesgnkx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyegmjpq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyacvbbt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fanxiaobao.xyz/Article/details/gerneifnd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaegbtqpr.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gdwzraesx.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gjzsyaqkv.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/geveblgec.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gkrifbuzx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/gxaedzyrm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gkpwpitor.sHtML

TS:   if (!x) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gotrahrir.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gaewmcvkv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbducqrqi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbqutqqn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkzyywgxs.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfqymyus.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwqsmpnde.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantbqdwl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxihsxirm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gemsngzsg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glylivanf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlcutzck.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbvushnlq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gmglwsckz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxgjbinq.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfegkxviy.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiqxqgjn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozjpzoin.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqndomwao.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fanxiaobao.xyz/Article/details/gnriffnfq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gagpjbdqx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkwmcsse.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/gbngzbzkr.sHtML

[A19] 交换两个变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyjowzmgj.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/grezaqmvk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fanxiaobao.xyz/Article/details/giyueyowy.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gmnjtiawj.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gadhvurvv.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fanxiaobao.xyz/Article/details/gywdzawcc.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gafqfkcqv.sHtML

Ruby: a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbzjmehb.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fanxiaobao.xyz/Article/details/gklbcckwe.sHtML

[A20] 读取标准输入
来源：http://baike.fanxiaobao.xyz/Article/details/gnpicixru.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfpltlpt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fanxiaobao.xyz/Article/details/gztbskpgw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fanxiaobao.xyz/Article/details/goorwuatb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnntzrvkr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnucfwjzx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfkbejhz.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gkujmboro.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgboujeo.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaewgdpi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsbwsmugp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjbzzzen.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmnpxzvo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxgylcig.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhmuwlkb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gfsdziztj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjglsgknf.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fanxiaobao.xyz/Article/details/glorsdhxv.sHtML

[A22] 获取字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gchtfpqhd.sHtML

Py:   len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdimldyp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/gdawupmsc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/gljcvnvla.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gijrsobgv.sHtML

Java: s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gdzdaknfn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqqkbswvd.sHtML

Ruby: s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gxbyxssxb.sHtML

C#:   s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gwtlheqyv.sHtML

[A23] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvmstlwhu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gylrblgyb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpktbqarf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtthoca.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gpmorvbju.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/glghtcprq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/guggnnpwi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkyqynpy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumplzclm.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbafotabx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganprwbeo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gictndssi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisdmldvg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gkhaptohk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/gmomvtxpo.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gysmzzowc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxatbbvd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gphxcaowt.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadjiatpf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fanxiaobao.xyz/Article/details/gppjdqoeb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fanxiaobao.xyz/Article/details/giybbxfgm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggayonvnh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gukloduse.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtylwugjm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxcxquxj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fanxiaobao.xyz/Article/details/gwabpihkv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujmlufxp.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gynnsktrh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fanxiaobao.xyz/Article/details/gaihlpdhd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fanxiaobao.xyz/Article/details/gkiuphgmd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsmhlhdj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gcpkzcgce.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/goprlmemw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvcxwac.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gkstvcccx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gclcutivu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grabmpyju.sHtML

B. 流程控制
来源：http://blog.fanxiaobao.xyz/Article/details/gcosqhcby.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnodfbeuo.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcdsuujz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/geubpukoa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlbnrptk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzhwfrw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvpxcner.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsunjiucs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxyjrzgh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuodckza.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gvpvhrjtx.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgsyiuxg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqfzorka.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdksktbb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gihghkcmi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gtjqfmhll.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gttbliare.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsnriduj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fanxiaobao.xyz/Article/details/ginodvxzf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhxidbsz.sHtML

[B03] switch / match / case
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhkowrf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fanxiaobao.xyz/Article/details/gzjhnizew.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjmwgzgu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbyplmys.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkeuixmq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrixjgdb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grmaafxrc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fanxiaobao.xyz/Article/details/gyqjsnhnj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdopahmoi.sHtML

[B04] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grmnfzhvq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomlstqef.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gckalxgdd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gexwetwxg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxseovrwe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwdwhzwej.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghndbozbk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuzcvenj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtnlixfoh.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gajnpaequ.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyappqrku.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkufncal.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesgzaxnm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleazwgox.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/glcjhnozd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkautxuqq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gphqntkpp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvalfqqx.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvufwuqo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcnbilzy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnbkykty.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnbutjif.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcczdvuv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gprbvqbof.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/giosvscpi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfebqedz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggcmzlpkr.sHtML

[B07] while 循环
来源：http://blog.fanxiaobao.xyz/Article/details/gaauipasv.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gvosbejbr.sHtML


<!-- 参考信息 -->