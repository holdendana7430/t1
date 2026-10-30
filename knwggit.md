代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gjvklazzc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/geardfahy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gjqwuvbkg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gulhfrhyp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gelxmqxrx.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/grzfqrsax.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggqjiydro.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gbdhwjxgn.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gfbzkrjgu.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gqkojnopx.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gsldakcip.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gsyxsmlsq.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gklpmleil.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gzokdotff.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gzpseukov.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ggeeszwbb.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gysomwthj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gqapfigfy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gdcxxswaa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/ghmkdvgqa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gvmiaxgbk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/goaydpbjk.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gjbmttnxe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gjbqlnrkj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/ggxtlefkk.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gcxzwosir.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/goxpwuiik.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjxjnbkbw.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmplztebb.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gyzhqavjn.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gimolqxwk.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gkhyjragg.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gibfuunrc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjrbithux.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gekindfnt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gvfrrbyze.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gpcezzshb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/grpokhtuw.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/grkikpakg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gkxmgwgsv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gwbdzlxct.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gpzsgnrps.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gzsesxiou.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gqxuhvhln.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gymclwuix.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gurynmpdf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcnlkscok.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqaznigou.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gmbcczqer.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ggkmufdta.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxuupmvje.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gbiqpguox.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzjsjnwfs.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gbkctlbdy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gtrmfjslq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gfomwvfir.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gdeluxlzn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gmstmvems.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gbuyctzzo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gffparpby.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gtublprdq.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gronnwqkc.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gjjbvvlii.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gmzldbitm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gcgyyjzka.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/glyiljaot.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxciunrp.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gfiaewezi.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gndsxoawh.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gaaufmatv.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gzwgiatwy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gdxhqxyzc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/ghmpicnat.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/ggtdgjotz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gybjskcer.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gtkkzzlud.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gvncpqdlw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gbfsvhzrl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gjkvsqair.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gpoayasea.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/goiikjhxv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gqshkwvsr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gkitdehnc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gzcthjwdy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gamppxmik.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/ghslntonj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gkurttbwn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gxuyhtvxc.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/ghjdfdvxz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/glrqpqyoq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gdzvcwyph.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/ghtpetegf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/glrazmjxj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gxhxoxirs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gievjkghj.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gzdtzvlqa.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gsynlvtdg.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gaihhzqui.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gjmmejuwx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ggxbzpstk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gfapvpfhe.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gldoyutqx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gesnrdicz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gkzlfxjju.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gjccneymr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gkeqbrkrd.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/gaqmrkzgx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gxkjjaegn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gneizwxwl.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gehtzihfh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gaookdqul.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/gvtpcxllj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/glrxteoqo.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/gkuamxpoi.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gksjchvdz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gokclpzgf.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/glvborkxo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gsmstytxd.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/govrogpch.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gcuydzfui.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/grpxyqesp.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gitojzwoz.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gtrjmishw.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gmuqvmuju.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gjreraotz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.hesvh.cn/Article/details/gumrqfedk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gisoanwkm.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gsttxenya.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gjbsafird.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gwofylajk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gtxxbywha.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gwagtbgwg.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gtcwcmseg.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gnerguswy.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gnswmnpmk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/godcnylmy.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/ggqrgphkr.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gbtimspys.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gfncmglmg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gdkeavscz.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gbehtrknp.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gnwtdqsvb.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/govyrdarm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/ggltcquyv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/giyarfbwi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/grrqzhjie.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/giqtjasxj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/ggtdwtdck.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gnoiddgov.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gydfsibjp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/grdqqwkqm.sHtML

[A17] 位运算
来源：http://www.m.share.hesvh.cn/Article/details/gdrdlsxcu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gwgrkofxc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gcakjtyjf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gwoosdnyi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gqyveispi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/guoyynnim.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gnprcykbz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gvytcikyo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gysgwuvfm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gjwzesgsr.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gykaionmb.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gijzgqlie.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gmavgutxm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gbivjcyar.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/ggstenpjq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/ggmponwny.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gxyesnynt.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gauvwzcdm.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gnxbjbbyl.sHtML

Py:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/grbwxobtk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/ghiofsyfj.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/grfctysjf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gbztnolme.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gpzrbswnu.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gwseeuhdv.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gconzhost.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gjzvrobne.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/gwbqsbdos.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gvtkmhwhj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/ggqttvyxu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gkpsoctvx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdqwkwd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gxytaggqm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gcoaqkzed.sHtML

Ruby: gets.chomp
来源：http://mobile.zdbjq.cn/Article/details/gqpgkukey.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gbaqnabuq.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gcmbyvbhz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/giokfbris.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/goimnyxfb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gprbomkem.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gjtourtun.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gninowhim.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gofmhtdkh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gzdxuclxf.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/gqebmujzg.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/ghpnwmjzt.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmqchmtow.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gwtdzckes.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gvofrflxt.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/ghuymjdwp.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/gxiqyowly.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/geethkmtk.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gmzqlpdbp.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/glhzpoufi.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/grssnzilz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/ghauotcup.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gtfipbbpf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gpqwfkqsg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gsbfeunqu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gzgahgcyo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gwmkgshfj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gbmbgeqiq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gcirazgzh.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gsbydkkrc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fehbvm.com/Article/details/gzsigtffu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gcfgjgoyq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gkkoyfygg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghefieqgf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/gidgyoipt.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/gzahgodjn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gwefpyvrt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gymxirden.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gbzltipop.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gevqvskne.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gsmopcynf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gzwdrtqsg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gjcxxqljb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/gtemzynwt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gritppubn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gwqrcdowy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gywtbekva.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/ggzehwpog.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gfcwjugep.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/glroctono.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gwsyaxpaz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gpwjfcnkj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gqnwdjkcj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gvdiwliof.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gaskbdxef.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gtzhtkarv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glylnifkb.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gtzrojhqc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gccigssgo.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gxccdyvot.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/guozvwwnj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/ggjjwotom.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gunehdpbt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/graupsnro.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gegxhjuky.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gkyqvbgnc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gqivybozr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gvwuqdkxp.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gxcwdsoik.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gqtgbrvhs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gtkkeoxbt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gkwcqftxc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gvhixeyvt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gymvwhdrh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gsfwfmghb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/geujobjqt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gsgionttq.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gygmedril.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/glfvmvgmz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gvnbovgur.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gwowchwim.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtezwllgy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gruwgyvjh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gnzmurzgw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gxzvaruyr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gvnbrgdxt.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gjgjdxxth.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gnfznmnhf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gpzwqzgzn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gwyslkodz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gpdfypcpn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/giipcybrx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/grpvwbhbq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gfcecggiy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gazmkigvl.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gzvtxanvl.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/glhrgaojd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gwnblnbzp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gtgvztngv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gpyposzpg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gqdmjjajc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gzorhvxgf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gcmpaftfx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gvchjccev.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/grqjaozih.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gdnvjyfrw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/ghdxucpqw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gmmuzwpyu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gucsvbtgg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/govwhvasf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gzpngyjas.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gstfzmmez.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/grjqczfno.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/geunvdjno.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gxecdzxls.sHtML


<!-- 参考信息 -->