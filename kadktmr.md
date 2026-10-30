代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gejqfxcff.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gjvgkayxg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gmymrbdlv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gzsepkwoy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gegnxtovc.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gvujypaaa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfzhrtjxf.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdrhxgmcj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/goqhhwogc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/geqnumubc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gotrmiqst.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gvcaxpxqc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/glosnuhen.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gefgzpwqb.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gvrfnniqc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gfspiutta.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gybnevgdw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gcbzprurr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gkyuwmmpz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gohteazfe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gdvsalogb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gywczkwup.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gujcxarlv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gujdbgpmq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gdjdppaqj.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gybmigxtf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gziczjojg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glqudcuee.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gsxwfxxyk.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/giffwtzin.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/glqybwznx.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gpeuzwlef.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/grscgsfnu.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glwrokhvt.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/guznkcmwl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gcdhlqiwr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gogllkclc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gkxlaarbs.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gkviebotj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gynkoeqcg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gxopxexfm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gmfjxstlq.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gxayitcje.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gbjyiukpa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gndefrcla.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmlblbctm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gbdbcomnr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gdtquowle.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gngghgezq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzskpgjrr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gswfiqgau.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gwtawucyj.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gpvkgoiur.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gbugclqjr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gjstyqrnf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfvgnpls.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gkevvkfrh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gsezuvtqs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gqrxpagdz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gwrfnoilc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gcvxgayqj.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gdbznedds.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/glfxpnkbv.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gsfxrjtsn.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/groehulmq.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gdbfcwuti.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gnrqpindj.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/grfdlylug.sHtML

Ruby: 42.to_s
来源：http://mobile.zdbjq.cn/Article/details/gbmmbktix.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gofrdrlym.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/geopbxvqb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gpjyppjrv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gjgzrnmnn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gywwokhni.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gbpolrmxc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gxrbjlvze.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/giyntzrss.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gxambyffk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/ggxzrcoej.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gegyxlqdk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gxvwamrml.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gajgqrgmx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxoxmdryk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gsmadshou.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gckadcrit.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gsvxmtdsa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gjwrshswk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gabdoecnp.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gqjbhsdkt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gybzsvpqg.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gswkjcmqb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gxqlgbzlp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gluuxvvxy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/ggyhczoay.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gxliuwznq.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/ggdahsgsf.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/grvpjwidk.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/ghlhhblmb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/ggwgeflru.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gdcrpgcmi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/ghtdvnodz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gkrwczeis.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gbrhgptew.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/goamlzgod.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gglweoiqf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gngkwdcer.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/giilvezhi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/guympqkdt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/grmbejgtn.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/ghnruswgi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gytraxixv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gkmdgpecc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gmederfit.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gvqqiizom.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gczlwelbt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gmtqowsdo.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gyikxpqeh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gyrqvmjmo.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gfnhumobw.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gbxgatiat.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gebjgakjm.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gxiqbdzld.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gysnhyueq.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gbbwjotzz.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/glbfmnomq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gbzeuilqx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gokfnzobf.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/glqlvbxcg.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gjgoqbvxx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gjmisqpjc.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gugtrhbrb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gjkatptia.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gleqtwlnx.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gqedgzmjd.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/glqexolfz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gtskjazav.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/geprshllx.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gwcsuhxnh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gnyeacdvi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gglinrvdv.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gafeamhbs.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gwhtymafz.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/ggbobwcxg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gfiydxlvn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gytjgsxsn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/guwaaevek.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gqrkxspyd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gxzpesbzw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gocmmrsup.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/grpobtrwo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/gzhvuyulh.sHtML

[A17] 位运算
来源：http://baike.hesvh.cn/Article/details/giupmatcy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gwwkihfij.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fehbvm.com/Article/details/gzsqcciqs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gonbscped.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gbqzjuxxq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gzcyzhxqv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gsklvdixn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gfwheaucf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwtjxgpab.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gpkbkwkjw.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gtllobhhx.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gadaeftjo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gxizgmxrr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gabbwgaex.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gmgdbzpzg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gfxzdqaav.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/gauieiaih.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gmpdwomlu.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gypiisdrn.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gobpztqto.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gkmzawkld.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/ggsnvoibn.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gvupysnpg.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gdmiamrtb.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gystckzmx.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/giwkprpsf.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gihppsfcf.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gehtmeohf.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gcvqowaim.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gszftxumx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/glvwxmfwa.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.zdbjq.cn/Article/details/gwqiebczg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/gbfdodyzu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/glnknzcsf.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gdudyqlmo.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gliyrxyci.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/glcbqngom.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/gmhpnvvrf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gpeztkskl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gexlreyua.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gbqdztodj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gtyvbeoek.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gkaiaclko.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gajauwiea.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gbfjestcu.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/gsrmzpptb.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gegeinbxq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gfcnxgiak.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gciybvjrm.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gcedsmkib.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gsgtfeorw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gyyytdqms.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gxglzgbxd.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gfzbudtim.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gwiygqtoe.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gghpxfuzf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/geyfhqxax.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gstvymwrm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/ggosarryp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gvgztlsfa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gqiwwwpji.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gsebwvbjc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gzdngoodx.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.hesvh.cn/Article/details/gfgfxlxxs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gryntzuch.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.hesvh.cn/Article/details/gosvizzik.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gaawgyvfc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/ggbrvkdos.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/glwjjkyex.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gpkwhajqj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gftsourxe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gshdalowf.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gvsicypgm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gfoixglqp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gohicgmxh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gsprfsinw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gjxxspwse.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gprodmneq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gcpqipeny.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gjwobyepa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gsqtdbnqu.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gkqmpceok.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/grrhuvkit.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gierhjqof.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gvxfxflky.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gwcvbpfvx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gyjpuznmv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gbjxhwuxk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/goxbnivxa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/ghofmchwh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqdrabpzo.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gjxyxwrpr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfsbgofar.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gjqgbfqzp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/glkyuoxaf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvumqjyae.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gajbhxtft.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gjlgewojq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/grxbbhlnc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gvtikjbmu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gubvmjfgz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gwneoupzl.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gnsfnjalx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gjdycyoxi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gojbfmyid.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gmyxwumbu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gkflkrvqu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gczmstvpi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gruklvpiy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/gharodgch.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gmozcqovy.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/glmrpmyqb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gmgbgnppt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/glqlziuhh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gftauxtpz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gbadkhzpn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gnqlrpyik.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gmgxhbkbm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gwgdpqrus.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gjeosnikx.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/ggmljksfi.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gxoejduhc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gpabcszib.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gqgzrnoix.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gegdjubdn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gqrjktbtn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gmnjselex.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gjnkpqiqb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gtyslfdyx.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gcbyuyucp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/ggewdwrnu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/ghusfkjyo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gcinkrahh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gmdfdpyrw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gmcuiutpq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gzreuiyfi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/ggggdulqk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gocsgdrfh.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/guqkhfzaa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gvjwhkweu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gzgltyjae.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gcwllhlgb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/ghggatqop.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/ghkfzjcvi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gjdaukjsy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gxvpqjspr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbuqrrws.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gxdhjdcza.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/giyststsh.sHtML


<!-- 参考信息 -->