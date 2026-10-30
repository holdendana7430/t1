代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gppnjbcxc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gsxfnfnxi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtgrcbgtb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gwujalvgx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqnammxjy.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gwkmiosqh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gccaueejh.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/grqnopxno.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/ghaxegprr.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/gkuvdoqaf.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gapvvqgva.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gogbzmvji.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gxzymkafs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/grerzrnxt.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gygbbdoky.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gqqauwsvc.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gimndjgtc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gsamulyjc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gfdotuqxu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpvbdees.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwypsvopt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghbsvhpdx.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gsivtiglr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/grfapolea.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gymxxqzti.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gtlvkayss.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gezvezlpd.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gectxgght.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnwlhdznm.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggvuhfisq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ghpvuvdxf.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gyapyaeku.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gvuzddorg.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gmkpdkvyh.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gxuhlmhdp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gpuhtlbad.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gqanegkio.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gdfxurjcz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gcodyumjw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/genmuqzwe.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gsvdglmbw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gqmaheqoj.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gzxcztaoh.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gpsicyrdm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gkspqronu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gspzzezjl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gbtctvmov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gfcrtwyvh.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guyxlvypx.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gfbmwolua.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gqdwqvbbz.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjmvljmgc.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/grlmkyemw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gckbasbfb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gaglbazvt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gamzkndzc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gvchdvevs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gdljuyqew.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gjnfgbujw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gxbusnuzb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/glgdzmvfb.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwexzdbsg.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gesdgggrx.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/garkgfiev.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gqmgcpspm.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gnpvlwowl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/ghakiirsa.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gezvoopwd.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gbwtfegym.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gkfaiprsk.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gsnxztdxz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gtqnwurzk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gbixouqmy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gzhhawwhm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/grlwjkjpn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gfrvfulye.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gpkhyhlgt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gzqdvwxiy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gfmvujyzv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gnjanloza.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gkatpbwas.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gopswylqq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/golymdbwj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gznzxjpsf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gemwmikdh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gifzeahsv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/guprkubvs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gvtiwmnqk.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gjkvntkdb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gghpdwkgl.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gycvnjnti.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gvhsunptn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gefoyrqtc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/ghymadimm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/geamsnsau.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gczosvwmq.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gsoyimuly.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gguyikfjy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gspvrvwau.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gsexwvemv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gfbbkjkft.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gfogdymmr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/ggltmmygo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gxsnwkkmf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gjuglkgmn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gkautlaxz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/gekkzxtfa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gvhpirfuv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/ggafvdcpz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gswufehln.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gmceodmvm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/guqokmsgk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gkxehwsbt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gdbweqmuh.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gomdqonna.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gqwuvlsvh.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjfuknmyk.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gzhuilhen.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjsngcxjq.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gqlqmawsz.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gedzhnfaz.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gqxlfblsg.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gorqfiafa.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gafvcpewj.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gevlkoiiq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gzxmonxvn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gpwvoxlxw.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gytpjvmtb.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gyfpvtipd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gvevlyjam.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gfoiihazi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gmrdkbyto.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/geckklrym.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gaqpxahkv.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gstspwsja.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gcgfuxpym.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/glbzgddwr.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/govqfgscq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gekgomqdt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/gsqtryqsa.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gxxchjjii.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gwrnqxbqe.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gjzagdmaw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/geacsgmvf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gkaghzvfa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gyzqqxohu.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/giivhzjvo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gjpprwluz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gfymkrwmf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gcrmrwqqd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gshulypuy.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gpkzjovmh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gshnndojc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gmonnlast.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gmsfvevkr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/glvlpyrzw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gvhutqwyx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/guatafpli.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gojnugiys.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/grwycgyim.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/gnbrpwhjk.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gqnwqqabo.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/ghvyvqewj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gwkeofgru.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gjymjbjyg.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/govnklgtj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gnnquuapt.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/grshyxqra.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gugfvxtwe.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gxgnqtxsu.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gnrooinsp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/gncuaikos.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gnrwrolxl.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gwnddtfzl.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gmljsqvho.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gqscilqhi.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gejflahpj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/gxajohpuk.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gmteklovr.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.zdbjq.cn/Article/details/glbjsphgv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/ghuczdgrz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gveufxdjt.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/grhrzzyng.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/glkkevajn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gtgemoujf.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gmjcqxupf.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gntpgtlcp.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gvvqagcgk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/glzauknga.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gfxorzlko.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gznfhdvfg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghwmxvaxk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gysvqucym.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gmuenfpfd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gnornybmm.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.hesvh.cn/Article/details/gtobahgai.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gddaqqupp.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gkazuiycp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/guxfjlwsh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/ggbxlqxyh.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/gvzlwbxpx.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gjrnclrcz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/gqvdlvoxe.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/grpcwghji.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/grdycmhwx.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/goicdjjeg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gphawrath.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/gkwlbsjxu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gcctsuhcw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gbvrirclh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gnpkfisxp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fehbvm.com/Article/details/grocycdci.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gbkpuzyvp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gmmzhzhga.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gfhdnabkf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/grdmxxexd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gwzftqewz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/grutymyqn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gzszdwoem.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gsowzowmm.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gymmvnssd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/grkufkghv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gqimuawkt.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gezleqiue.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gwipbxbhj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/gbylltwuu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gylvdaiqs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gggplgpfz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gjsytbzsz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gzbtvlhdn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gspzwwxji.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gpzshuzqi.sHtML

[A26] 类型转换总览
来源：http://read.share.zdbjq.cn/Article/details/gqbygwknf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gkvrcafgc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gfmutuqab.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gexfqdznp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gagafjdfw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gtaogbmpy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gezsyvkku.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gzcbsudor.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gdfqdtwke.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gudyqfjab.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gvnbfsfcc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gojdcxqar.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gzxyjuzik.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gucpxzpux.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gtyukyskn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gixdiwcqy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/grctstfon.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gxkxrmdwx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/ggwzphlxt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gdriycrmf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gpbphiaqf.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/giavamgjf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gyztxiqfs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gtatgmykb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gutodwlsu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gcxxbbdkk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/glrwiktfb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gpszdnkdy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/grfhfaskj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/ghyilxicd.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gmewljudj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gzkprflwf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gtrvmxwzk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gyfecessp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gjlngufxi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/ghvtjvsai.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gyikjzzdw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gwdqtrxwk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gxxlrnxww.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gjuacfukr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/ghhpfokdt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gdzfvdxcu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gxdlxgavt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gmumyfrxz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gladwpglj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gcomgafab.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gpwxhjuiv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gfucfazcm.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gsourugbu.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gfpxgajdt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/giacdfdnm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gnyeqpmck.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gtldywzvo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gjbcvxoay.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gqxmwnzdi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gvpyojfgx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gtlmvityv.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gnxgoxcnx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gnputmahz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkuzoiyyp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gydxjryjt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gsdndfoor.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gyeorxlsk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/ghmhragqn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gpnrljfti.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gcaidqrxj.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gmxobwcao.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gibuagtxv.sHtML


<!-- 参考信息 -->