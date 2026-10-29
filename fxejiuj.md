代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gjzsfkxaz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/ghozjrbon.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gplqwbawz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/giteqxygf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gspdqrpjq.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gattjmmyv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxedajmrl.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gyedipgaw.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gkfcliobq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/geeymkjjx.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gzzmupbkq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gvmvcgllm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gvfogxaww.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gepjnccfr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/getkiuzpe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gwzylpxpo.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gygdqjnai.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/ghsdjldkb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gbzaaaqxm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjraizxns.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gdnkgvfau.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/ggjtufnof.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gcihvjlmq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gyvhogdsn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gmhihenii.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gnwllkixp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gxsosupos.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghefgbrdv.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxpmmiyfv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gzhfhhwdl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gclhgswma.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gktkhguah.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gniuzypps.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gtrdhraqr.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gqqmjdnzi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gnadlmfwo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gawqmgzvy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gzthrmdpo.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gwvjoddoq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gcsmmkqds.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/garrwdudi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gnmlflkny.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gpfabitgz.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/giqvmxiht.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gornirgqa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gjvzuvluh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxntvktqv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ghvyfnblf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gzeyajpqv.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gqqjzdfpy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gxptpqwis.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gwullzsol.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gaqqrrqxw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gkjxkvzqo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gvihaxtcl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/ghtmzepxf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/grmehaipr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gdteognho.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/ghaxastta.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gyspzglwi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gryaiwwcw.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gkqsmumwq.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gofbvdrgt.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gnkmzdqjh.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gktagbjmg.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gynjgjdgi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gpwqoscud.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gpdzedswy.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gkbhyswuy.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gjksdakej.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gbzemasbp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gljagbcvc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gjshuizko.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ggjmhwety.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxydlbbnm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gfqnedlyj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gjcsezzfc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gkonquygx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/guzctfxtz.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gpdqiiedz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gzejkajxu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gnvzaejwv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gflfvqjwa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gegurpswp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/guozjxhzd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gkchfnama.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gsbcdfyuw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmjbtiowe.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gexphdmtl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gyqbjdqmk.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/glxsxidmy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gwyhagpii.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gtivmfdjo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gzoalrjud.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gwkupctkw.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gsjeknnye.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gribvolkz.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/ggashqzlr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gqzkdnzbm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/glrtavofj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gcitapuch.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gogklnhqv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gdgodbiml.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gtyvjlhmb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gfqvmvswq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gyiprveqn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/grplshhfc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gkqwikxjb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gytknodso.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/goegozxzi.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gkgjgglpf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gujyljtmb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/geuguigjs.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/glnvgjzod.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gtibcrbjl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gnfrfvbnr.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gblulrvtd.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gkgwoklcg.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gywpwqtcj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ghrcalndk.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gxvqyozsp.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/ghvhtiwae.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/guydczrgz.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gtdwwuzpg.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gdcctfbcn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gxbimhzoz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/granrpgsg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gikddfxop.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gbjrwvrvu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gfzngrgut.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gemmzsbtu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gvvjvjjbs.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gafnwykjs.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gtljebtsu.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gehvltygg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/giwdtbgrm.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gnvskyzfc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gfwduklpb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/gkmscgtkf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gjqeilajf.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/giggebvjf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gdeduereg.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gxavqnuqi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gltrohxis.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gnuyepwal.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gdntijeru.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gcgleabzc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gyritszbq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/geuyqbgqb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fehbvm.com/Article/details/gmxkeltjr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gkhvudiui.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gbxfmrbny.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gnsivomml.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gxlnafuxg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/glskujgki.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gwdylcxbt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gfgqtocqu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/govgrrlxg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/ggfjvdavm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gzunwjodu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gvzjotlhy.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/goinngroa.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gcvgggptp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/goutwtljq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gzmbascml.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.zdbjq.cn/Article/details/gibxwyhqn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/grykyhrgg.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gqohjqwzo.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gdqnmtplt.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/gnriwnomo.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gloonqszj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gfkldrixc.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gqutfesas.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gzztlnqoe.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gquwueqeo.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gjxaqeyir.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/ggehyykhg.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gyrnpouqm.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gwwteszor.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/goyygndwa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gmovdzrxo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/gtnlasabz.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gpkmlwbzx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gpjdsjjbn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gihldiiwy.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/glmvixxjb.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gtvkkwcme.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gkoocgshc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gjdubvhcp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gmleyusdv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gjhfvjdsv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gvhcceppt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gnircwycr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gvriimgle.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gasgqhxxh.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gwtauncjm.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gbeityium.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gpfaqnjwo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gpkgjwvap.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gcokcbxff.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gjwtcbldk.sHtML

Java: s.length()
来源：http://baike.zdbjq.cn/Article/details/gxvsmtkxr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/gywmujbck.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gmjtrdwml.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gaahxivqu.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gdqkxzesy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gzgvrzqkk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gwbjigiuh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gxvotswje.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/giwkphxdt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gwdcyjlhb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gidzwxziv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gyzbvkkls.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gwhtriyud.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/gxsksfoww.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gahmcuktf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/grlfzosta.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gzmxzvdgz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gnwoxfmto.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gcubwowom.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gckhiwnha.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gjsryiggl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gircsplim.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gmnoirbez.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gypyqtdud.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/guxwqjxyv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gaaxusjly.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gehvnvnlt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/gcozlndkz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gtqtdzezq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/geqnaoknf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gsykdqgeh.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gbibcujyv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gjtckplgq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/geqgcrxmk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gkzdsjnsv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gdkbvokmm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gxfanzsvh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/glleznjtv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gkmpijrxo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gsavlcstg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfpcatrho.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/gnepdmkxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfwukpgpz.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gathgqanu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gyiwffijx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/gghxmqpwc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gxbfdxytz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/ggsupifss.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/glkpqtcuo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/ghprkrfad.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gutpklbcc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/goyaoshsg.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gyfblixlz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gycxnmbtp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gxypgyczk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/giblfugcx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gqgyuabnq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gczdyagdf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/ginwuscjw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gsarkrpyg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/goovzmnnt.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gdgelvdrd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/grdsiogoe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gtlcbydob.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/guprrmwwq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/goxzsoefc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/grrbpoyth.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gdqudybon.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gtuywidfn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gxjbaysnt.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/grjdbvzmn.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gqxwiuuvm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gzrutzzcl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gxxstablt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gromwnkzc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gaiyalcui.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/glxrcvuau.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gkwgpgwqk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/ggyrjozox.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/giatkxouw.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gdiwxbfma.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gsubighez.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gnqdlfmaj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gqpluufrt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gpjokrzsr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gogybvdmd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gknuooufa.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/grzynsprz.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gfiunuqzk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gckxbbvaz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gdfsjmwax.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/grrtdeljq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/goupczgqj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gopsbnwvh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gkmxyglvn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/gqqjozdho.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/ghjnmyraq.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gwgmfqegh.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gwuhpdxat.sHtML


<!-- 参考信息 -->