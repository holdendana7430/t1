代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guvbfqmzg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gljoscwuo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvspqpou.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxrblnzr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkadnpxm.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyuvxdax.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbobqhar.sHtML

[A01] Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsezaagi.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcehbrsj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gnturhypr.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gixsiszhs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcndixdsn.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gopepctvy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gcixvgfhz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxsjtrue.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/galyumeff.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxebscmr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqllsqtpf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdkqcztm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gktsauevp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gmjqoclpw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gnasaftop.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjapjwqrn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gosvmwjur.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gzfjfnzbh.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhjzylfu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fanxiaobao.xyz/Article/details/gburkzphr.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gznrisntt.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/geqleglqu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwcrsreg.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gloilnrrv.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gxitiqepu.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmfychek.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gojsduust.sHtML

[A04] 判断变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobjvaghc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyewgcdjb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkbqvtngc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvqrlbds.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlxuvez.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gbazmgico.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gepcqlvye.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjhqdpjs.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasacjdkd.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gxlerdyyd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxenzus.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gffxmbeqx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpqycsbr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggehysqzi.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjpgzokvf.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxosczxeu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzptrost.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqsoabed.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkojwfhec.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwvsdgox.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/guatnawzh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gusfoesbm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwazurjgy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gdhqliipy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazlcmpay.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fanxiaobao.xyz/Article/details/gjgihnjti.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gqtuahuil.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grvbqrhfg.sHtML

Py:   str(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpdmqskz.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmgeqxjt.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/grjlczhxx.sHtML

TS:   String(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsbtnihs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gsubldshm.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkqfixsp.sHtML

Ruby: 42.to_s
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtxfovbj.sHtML

C#:   42.ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/giqptouzr.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpfolbbm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gryfvzzom.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbrvdxbr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjjmwlfz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqfvecln.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwvrapvl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrizdzla.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fanxiaobao.xyz/Article/details/gprenousp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gockzuvls.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlbbqcbs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcfsqsev.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwaztrzc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggrciiyi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvfhmphr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkprtxtw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fanxiaobao.xyz/Article/details/guemloeru.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fanxiaobao.xyz/Article/details/geucvtnyp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmjzgpkw.sHtML

[A10] 生成随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnnfdglj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fanxiaobao.xyz/Article/details/gfotmzbtb.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gzeteecfd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gabfwdvha.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokuezvpi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudzcigxa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fanxiaobao.xyz/Article/details/gciuamrlv.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbsfqlvl.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fanxiaobao.xyz/Article/details/gigyifidl.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gerdeoyno.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdcirizk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcnjyrfo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gherklmcg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/goserlhay.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/goekjqbbv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjczxssjf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gszjsceeb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gupcnzcjz.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmysrpbio.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpycxmqdj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gluhfjrkk.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/glqmnqhfn.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzqtwpru.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrrtfdsw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gikidtbqm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gncbcshld.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqwhzxrp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxssilmp.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkcghtuo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghejuylkt.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfdypckj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gunvqikvc.sHtML

Java: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gsnhlidvl.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocfgubwu.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwmyclnx.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/giqkcfwmp.sHtML

[A14] 注释写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhhskbsa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gvdcdpypl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmxnakh.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmvoklmw.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gnepgdbuo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqnqbazz.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbijzdidg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gtpgwuxda.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gufvtwzgj.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/geldtgihy.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfvdiqfu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gsdakdmrr.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnywqherv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvygmluqe.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiambndk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyiyuiuj.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjflaat.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqodfzhzz.sHtML

[A16] 真假值判断规则
来源：http://wap.fanxiaobao.xyz/Article/details/gskudzttk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/grztfkgnj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwuvvvf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhkjjfzc.sHtML

TS:   if (!x) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgcsaffi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/guydymkaw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxucxpxsg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gqimxsrxc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzogdslls.sHtML

[A17] 位运算
来源：http://blog.fanxiaobao.xyz/Article/details/gshxcwxkd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzpjgvce.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcslwwwnw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqjmpmjq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/godnitjsw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjbxlvpg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqhhyosa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gnawhehpy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxypmgxhc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfmwpimy.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gfhmzxsci.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gjfaicibm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxzncncs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/geomafuhp.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoczfdyh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxekkwcs.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fanxiaobao.xyz/Article/details/gttpkwlfp.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvcjkmro.sHtML

[A19] 交换两个变量
来源：http://wap.fanxiaobao.xyz/Article/details/glyecbltg.sHtML

Py:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gesginwhz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fanxiaobao.xyz/Article/details/gwycukhqm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffbadavr.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gukzvsvhr.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcufbowl.sHtML

Go:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gctdqyuno.sHtML

Ruby: a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmsnlhda.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fanxiaobao.xyz/Article/details/gcqghucwu.sHtML

[A20] 读取标准输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gukophjyf.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/gwfyweacb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fanxiaobao.xyz/Article/details/gznbqosqc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvuliepg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/grspupzyh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxacdogcr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fanxiaobao.xyz/Article/details/gjyiiesey.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gsogfgmjq.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwwcocbv.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjoskzaw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glaoxkmsl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoeinkgj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmmyaaxv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfsfxbez.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqptvxkm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/geengdkcj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gscgqezto.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfesjis.sHtML

[A22] 获取字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gslhidpst.sHtML

Py:   len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwikmuq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fanxiaobao.xyz/Article/details/gksmvzjct.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fanxiaobao.xyz/Article/details/guaodptuf.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjhaioqn.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnueljfrj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgfvznyg.sHtML

Ruby: s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gaankxzki.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvhwuzdm.sHtML

[A23] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbbzasvy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmyljlzx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcslzgup.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/guoyhukbc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyripwzu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwibwmfhe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfwhrncel.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycmbcquf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwkhhdiv.sHtML

[A24] 去除首尾空白
来源：http://wap.fanxiaobao.xyz/Article/details/gctrotwly.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpemejoj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtwrolpm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrjdpcpe.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gytnruffc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpuwrhxj.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoqxjwct.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkwistoq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gduhzpdon.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecffvaaf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fanxiaobao.xyz/Article/details/gzdglhfoc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fanxiaobao.xyz/Article/details/getdgxmqb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxwpyqbxs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgbobyhl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflnorska.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gseabslaz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqttghkdd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdpqggijo.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpegecpi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fanxiaobao.xyz/Article/details/gcbfkjhgc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gsneijaol.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fanxiaobao.xyz/Article/details/gohavdcet.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/gumpgbzmo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcnccych.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqwzsifry.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsruaznv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gnaegsfiz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwrdxmwbf.sHtML

B. 流程控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gomhevdhb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyqneytkj.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gqeapmtpr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/giubifxhf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxxfoylax.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/ghqmsyaup.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjvvnyk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/glaqhmmxj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjstadvr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyvjdwcg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmtkvvqd.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchqwlsic.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjwmwszj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjdlotxu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxptmwed.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/grgwmgxzs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmplusjgj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/gwvinxzmq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhsqsxti.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcnlkats.sHtML

[B03] switch / match / case
来源：http://blog.fanxiaobao.xyz/Article/details/gbviyxbua.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fanxiaobao.xyz/Article/details/gpmmsauxy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxqjcxhf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggopqqcsb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabuutznj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjwppkg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/grinsfljk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fanxiaobao.xyz/Article/details/gwsfhlfax.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/ggsocztbx.sHtML

[B04] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcaaeigv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrrmzzci.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gesfhwdpi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwzwozhi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggfvoscd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvwotzuuo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhplrbzd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqktudnb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyarhmee.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhdeqcmo.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsklhrsc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzyrcqkr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfovxmqfv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtusawfic.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxegwmwq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fanxiaobao.xyz/Article/details/godvniqxr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocsqjzou.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqumqozm.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/gzausjjok.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoqjwmjv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gggsegbkn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/grpdczeft.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvavcekk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzluuwhpt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwlwxad.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmbxaktd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrdhaxom.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwvcfosbs.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkioighd.sHtML


<!-- 参考信息 -->