代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gouznnvze.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gxcyblqut.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gyumnshmt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gzkraogof.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghdqxqfhl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/ghrujknyd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gonhntnqu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gxempfoed.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gybnprqmg.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/glivnzvfm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guquguind.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gygvxmjcm.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gqrpjijwb.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gsryyykyb.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gphxnkmmg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gaqgmukow.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gtcgiwouv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gxjhnogcp.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gbntkltou.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxutwmerw.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gubalfuln.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gulmsxrgg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gauutwgut.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gugeqejav.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gpmnyfhvj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gwobmvaeg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gunvkacas.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/ghxmkujsv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gtgehizax.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/goynenmyy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gbyeqeadg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gaejqkktc.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnupvmymr.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gridoecsi.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gcoyufyhi.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gshqiopiu.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/glyyrveiw.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gmdikthld.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gadujsrbq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gfttyhmjo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gltbxymcp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gljlvhakn.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gixoqustu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gvzijlock.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gjyxlcvex.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gokoxvsih.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gsstdbhog.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gkunndtuk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gmjxcjxzg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gfqbszyku.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gqdsvxryp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/glgpamwuv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnfkporpi.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gphyflvvr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/godshxuqo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxoptaamt.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gcgmaayog.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gxupkwtje.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gxpzeqxue.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gqaicqcun.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gmkmgdgxt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gybibdonh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gccejlvbw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/ghfaaivpk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/glocjctem.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gerzhewtg.sHtML

Py:   str(42)
来源：http://m.share.fehbvm.com/Article/details/gyzobtqho.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gvsccjkwp.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gsohbipnp.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gxqrtyzhr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gctzopouq.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gyvxlzenp.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gmklsigln.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/guzyzolcm.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/ghdeindth.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gidovbhcq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gprhijhps.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gkyazqutx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gqctxlpry.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gbfbgnsvo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gckkoruej.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/ggdmsckir.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gqakisksd.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gupritspe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gqejwpxwf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjwfieala.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gtgusjmeb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gglilppbb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gnjgefzrg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gawbounnp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gedjieqzk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwdyqvbmi.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gbwkdutrt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gbylkabvm.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gvlfwnpzq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gnqhnrxcy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gmzxrbguy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/geetfkunz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gchdsnfdb.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gsvuzwzkj.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gzzsiyoye.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/ghrkzgcua.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gdbhyovas.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gkkifpcxr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gjorsuyeg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/goyptjgqp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gemhkfhzn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gklpgyemh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/glnxsnkaq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gxnvgzzbw.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gbgkkdlge.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gddeqxeci.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gswyqftzn.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gnzaipqnw.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/geubgorws.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gejictxqs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gckkxpdfc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/giqodczan.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gmtkynoid.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gvhqckfwj.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gqbetolbd.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/guhyhddnj.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gdqklholh.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gawbakxrt.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/glxsfjode.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gxtrbrfvy.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gqyithwcn.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gtnmsaucw.sHtML

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/guscmdkft.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/ghvvbatii.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gzyesivbn.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/grqfhlkuc.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gbwzglwkb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gikocysad.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/glrynjpuy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gqsdkgyxa.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/guacusgyo.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gnwoikwnf.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/ginzixlab.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gsykdllmz.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/ggykfsogi.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gcsaaqlfo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/glqdgjxft.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyynwjvaq.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gcxofrnft.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gltdkebgk.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/ggdybiybk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/glncwfurr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gajenuyfx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gyewgvfyu.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/ganpsrsoi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gjdrggllt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gndhvocjg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gyjtzfbsy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghlzphwmf.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gtvplpkvr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/guuoljded.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gkchnnqxg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnngpdrkn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gepjcxkbp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gdrutgkyq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/ggzjubtwr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gfhozmpwh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gxogppnkv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gmkxktfiq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gzeorcbqi.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/grqahirjy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gfpspijdj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gbbjugvhv.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gzcfjuchi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gyuvaqfal.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/gfaxcnzzn.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/ghtkqtmil.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gzyvvlrnd.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gonybqrye.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gnrvtvvai.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gdtvakaoe.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gmwgkosnz.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/goldixrdv.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gcxyyaopd.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gzcnxbqsr.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/glqxdrbvl.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/gcpzatddu.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gqaycczoa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gbplptfcu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gclyndbtn.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/ggqlkyfcv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gimjbvzvy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gvtjvnsza.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gorihjwol.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gyrabadkl.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/gfuwlutyw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gyhsvizln.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gvxypspvs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gjmpixyne.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gajkcgayd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gilklcbos.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gwsoqcpyc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gduvpzpgv.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gfrdlznsv.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghfmgeoid.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gbeiruqth.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fehbvm.com/Article/details/gzizdfnhs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/ggmibukcl.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gpwdumnhi.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gopmfaoko.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gbfcsshnk.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gvuvcuywn.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/guqitphoz.sHtML

[A23] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gnhcudxfh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gykiurygn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gdzspjdoh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gilivtelf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gwbojsrho.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gjrfwvbek.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gsndqhims.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/garwsaxiw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/gkyvvkrdq.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gwvmgkfwk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/ggzhoqfqc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/geumklhuc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqvyqnpjw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gzktuxnow.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gimctfaag.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gthqlqepr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gzkmdxkil.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/gnxcjpzha.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gqcrqnffr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gjglpaijl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/goohddnee.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gpzqtauuo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gizkltiwx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gtewyzqcy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gbclvtpxt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gwujpzkjl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gpxbonkyc.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/goerckfdy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gzgvomeyx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/glisbfcfc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gopafcskk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.hesvh.cn/Article/details/gzpqnlzds.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/goucyppmz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gwiilakzw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.zdbjq.cn/Article/details/gcvnietxm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gthzqdwsx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsjbmrwkz.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gxdgnxyjo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gafiejnsz.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gapnreteo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gktjkfoxb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gjqrlwmjd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gmfbslfaq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gqhypvvai.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gwcbxaihz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/giwmxkztr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gmwomhntu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/goiosbxyq.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/ghjsvfgsv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/glgywsuon.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gqrixjslf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gxgqwvxpa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/ggmhldxwv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gbtialutv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/ghvrutqad.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/ghrrcboly.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghwenhbls.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gceusdybg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/giexxnghl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gpegojwvu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gqludfnmi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gxmulgfek.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gxrbwwbnk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gqkzkwudj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gljqdyujv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gcazbhzfo.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gvlkbxrkb.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gmjijliru.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gbrdiixmi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gizmijdba.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gxkqvsiwn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/glmfamarg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gqjqebikh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gbaqhrsmg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gdnqmwtqi.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gnchyysoj.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/giwamdxcm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/geqynlqzy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gbjzrxkdv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gsqltpugy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gwsbptcxs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gwnkayewu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/ggqkdsegz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gerkhnmhh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqpykavzp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gwzubeyhl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gboyxaonq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gsfpvvkrt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gktduzbqm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gjohwzzpi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gqflotjnm.sHtML


<!-- 参考信息 -->