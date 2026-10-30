代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gwluccbgo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gspgejnsa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfapaimr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmysshikb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grrcuwvve.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjrgmymt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkdsdjzzq.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkmmpnbo.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gzevvemie.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjfalecjs.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/gpyrxmwiz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gmpgcpamd.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gkzmdipym.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gldbbdvgk.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffozbxmp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gqqjhmaxb.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexrdwprg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/gsmjxvkcw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxdfqain.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfatwppe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtziyaqlt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefvtxcta.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitjjnrvc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fanxiaobao.xyz/Article/details/gnnlhdlsi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/glpbmxbji.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geutjmxbd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gruwoijzt.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/glfawxdra.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gygorrbjh.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrdllmhp.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gefesmpug.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gmerprrdq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjkhjsku.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwufrfbhg.sHtML

[A04] 判断变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqlrjbgfl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqjtchnq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndsxqar.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwywqsd.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gysybvrir.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvcqsqen.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqpsdqfh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gpohwuwrr.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gpstylxyw.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaccjvety.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gkdvuibns.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkgcjkiin.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpfajugnq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmsssee.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxakrpasn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlfrdnft.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/giyiyitht.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gngvcpsln.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gqpeafmea.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gzcplbuub.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gixfuqdgt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpdziylg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoegkedk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gwiotrwnu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/goqhoiity.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzkuezjz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkltpxach.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gngwjetci.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieqruxcv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgasyqdf.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gqaywceun.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkozdcw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtegbbdts.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtulnkdej.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gzlhqmwgm.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpsreuso.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/glndgecgb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gektneiva.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fanxiaobao.xyz/Article/details/giacberzz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwiirnlb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpoafvla.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbodgpnfw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcequtrrb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbhqcazy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gmhcqjqnz.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gvgvopbdc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gngxtkzvb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitwgjefm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytzzpbxn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrwdzfnr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjreefsj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fanxiaobao.xyz/Article/details/gflklnkai.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhfstda.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxncvqum.sHtML

[A10] 生成随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxcpuepl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnysuvzyw.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fanxiaobao.xyz/Article/details/gopwkyuon.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyckzrhw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/geuiknvkt.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcbrvbnn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fanxiaobao.xyz/Article/details/guekopbxd.sHtML

Ruby: rand(1..100)
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzfaqui.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbinfpya.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvtmmwre.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfimvddkn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqcyyey.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqipxmfz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkliqbghm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gpdnasggy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/gjkutmmvq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtdqtexi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpuinvia.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkwimstj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjjbqkdx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuvnryde.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/geqypywqa.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbzwgzmq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fanxiaobao.xyz/Article/details/gjypzhpyg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvwkyeve.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzefrsaxl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipgmcwk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbrqwad.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guemyrezx.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjfuwysp.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gdaviapoa.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gygfjpezx.sHtML

Java: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gacwmmfht.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzevrdvj.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gdfbsqobu.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiofttwz.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnclfsoc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghefzhfbv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwedmdy.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcasnmgu.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gryssnfax.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gqchnslyd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjcbyzrb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfublwxg.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gusxmgrbp.sHtML

[A15] 空值判断与默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gwuarjdgb.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/guvnrjjgv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/geuiyzkkt.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjwyztar.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gebelxsnf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxibcvrwc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjqsejga.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpajwxibu.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gvwohjinu.sHtML

[A16] 真假值判断规则
来源：http://wap.fanxiaobao.xyz/Article/details/gzdfxvbvd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgarrlwh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrzuhku.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gqceptzfb.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grmtvprex.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfgeznlf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqwmubtng.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gkuguyswm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmgbjudu.sHtML

[A17] 位运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gnitwdgpv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqimqtpc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvevgrg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/goiogywst.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gebfdddgb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvbjxpz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gkauhvgjc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwafcrrz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gabrpodhw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesswtifw.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gllvssawp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqgbjius.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtannzkhj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gbaqxiftp.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/gzbqlazzl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmeelyu.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gfzkvbeeo.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/gdtxjproi.sHtML

[A19] 交换两个变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcuvblgm.sHtML

Py:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gpzfdihhg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fanxiaobao.xyz/Article/details/gxcvmeiij.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyidzdld.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gppgqtddw.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gyswetyyl.sHtML

Go:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoojryvq.sHtML

Ruby: a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gktoflthd.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/guowkidab.sHtML

[A20] 读取标准输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbbjmzvv.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakbapalt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fanxiaobao.xyz/Article/details/gtwgddiym.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fanxiaobao.xyz/Article/details/ggxnskzbc.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gtydyutqd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fanxiaobao.xyz/Article/details/gogygmepz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrflctsm.sHtML

Ruby: gets.chomp
来源：http://3g.fanxiaobao.xyz/Article/details/gfzhkngpn.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gauhwnaxa.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcelxefyg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlwftvvz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvayrnv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycuqkapn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gripdpzin.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdgiqzp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxdysnvt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztassrqs.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkgxfgs.sHtML

[A22] 获取字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glwglbwfv.sHtML

Py:   len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gljoskgyi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfobfsqxv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fanxiaobao.xyz/Article/details/gcvxyxldd.sHtML

TS:   s.length
来源：http://blog.fanxiaobao.xyz/Article/details/giipmcrfg.sHtML

Java: s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gnkrhwojz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvrcizwmc.sHtML

Ruby: s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxalwwzeg.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gripakwsc.sHtML

[A23] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzmlufefu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsoprytv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqiuduta.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqsivqdj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gooalfsfl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmltgobul.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqznwrku.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpbjlmae.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauykjocp.sHtML

[A24] 去除首尾空白
来源：http://baike.fanxiaobao.xyz/Article/details/gkdmjeanm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnbrblly.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtahkefdp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/ghhuupgof.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbitfwjbz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgjygyrz.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqeftegc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/gumkjwusy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/ghoojbirz.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtidvcafx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcjywhrw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdganizgh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrcoukgz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxgusvelj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsvvouan.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvompblra.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fanxiaobao.xyz/Article/details/gurfaopjj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwdfujae.sHtML

[A26] 类型转换总览
来源：http://blog.fanxiaobao.xyz/Article/details/gzcurxlfu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gewnxgslu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghninayyt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvijoybqk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fanxiaobao.xyz/Article/details/gpkrywmtt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwcuheww.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glbchlvql.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkauryei.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gjoabluge.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtndjqkjo.sHtML

B. 流程控制
来源：http://wap.fanxiaobao.xyz/Article/details/gggdkpidd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gonnmppba.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqqygpos.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdobgjqhf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guaxtunak.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmnmkobw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/goodzkgct.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gfqempfjw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/goxtlyulf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggurwipkf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/ghusvslke.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/gofhopsfq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gystjkzge.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhzqcoau.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplvbvmmk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gyskbdgef.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/grenhawbq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoolyvrm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgcsbztc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gnldvuzdz.sHtML

[B03] switch / match / case
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjiclher.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/ghfzpbtoq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgpugfls.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhryplm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjsxwcwg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grpfxxvyy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggusluvss.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxmqjste.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklsbwvfe.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gdaauuxdy.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqurpua.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnfliqwy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyasimtpe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbiklykt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggpmebizr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmrkbtuu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqainamsv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtejurnvg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goefysjur.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmwxxumb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/gilvnprdj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvelyioje.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqudfckzk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/govafkanu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgkhocox.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fanxiaobao.xyz/Article/details/gqrmdvjvc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfudiahcx.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fanxiaobao.xyz/Article/details/gnqghufrv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbotfgur.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbtwftap.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtgotdpb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbklurzql.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjnpyrzp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/geatkrseg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtukloxl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfltfgloe.sHtML

[B07] while 循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwauagjrl.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzamioscj.sHtML


<!-- 参考信息 -->