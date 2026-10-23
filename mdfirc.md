代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gcwdplrp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nhkmtixj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zwtllnuc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zywiboyh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyqnjiuc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3thujprhm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ilmrgqsn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfejvvor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qubcatho.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ovzollgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjaqisqs.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3cxarwmtx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vnwpegdd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hjaaulgx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dywhvfrz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3pjmqxfax.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ufqoxboh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bpkftxte.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3pcorwkob.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aqeutvtx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vbvtqxyr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ltdyofys.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3athuvyvc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3apuxsvds.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ewxlnjqg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3adlxjmzw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wjasuqpq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gdkjfyvw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vejvyjai.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xloyecxx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3recipwca.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3omfzilgj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3esneocoj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cpujujlp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bgwlakbs.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nxzgcmzv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hkbdnjpx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3npjnrlul.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qfilnesu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3bphcrges.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qhywblqh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tympptds.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cxfvmcet.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qyrpyeto.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fupvukgt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3knwnizgu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xvkqzgpg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3cneabbnp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3njcmfygz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mlccqhkc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ptrwtris.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tcgidyoi.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vrqkakps.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aciyjftv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3omqsinaz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zcvtelyk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pesgbcfj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ydzsdkdh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xkdqpklq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gbpayawj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vbcnogqa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rkwftomd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3afqwjvuk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pnsqoiib.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kxaiqhru.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ulsvtrij.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rbuvixhd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3aauzneap.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ismqmncm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3qqrxzkwt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pcwxkkvd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fslxjnvx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3yffouunt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3jrmbmimf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3bvkzhuhv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pyvhiris.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3drkrwlrn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjuytoa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3jgpbgoxi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ptzjpcft.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jqseemqz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xevzzuob.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mtuckxsi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yldmcdjn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drophcmn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xvlgvtsw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fljytwad.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxgfrzrc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xezglqih.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3nosghmwb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3dgqdsvly.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gemsfgou.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zwwuvdzk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmahwud.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qzqjyldr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hzvqjupj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlflfs.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3caiscywo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3hobwwtbb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dquxleha.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tlsvoprx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gvibykkw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ezcergkj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qiaiwffp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lctdyvjf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rddaffcb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gzlwkpor.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nfstobje.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hnqehzhf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xpyxmaor.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cnhmikjl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3leltbwaj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxirrgt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yapurpfi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3reryniun.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ybpaemjp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3njyqellx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fqxvclrg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ofnggslp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3korhbwip.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ycecfoiw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kgnfwumb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3udktacty.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kcgbheuo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vipdfsln.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vcairfyw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qfzizwre.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhpncrp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3tugwpagn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pcqowfme.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wdmukvmu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3szkbgnkd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3szknxvzd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lcyljlaf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pbkterwp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3erwbpifn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3amxwdhfn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zmeunqfy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cbrwzzdi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fyqwoveo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uopebusw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3webqqrio.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qqdaagdt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cjvsoyjt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bxvirpza.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rukhmczt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jxdtwppm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ldtzjuyh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fgceymdg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hgttwmfb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pwucrzeh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3oeodoela.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3sqlsklzc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3vvihbaya.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhyqncak.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kmiietoq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nrrwjzfv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3svablxps.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pfxlediv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hijmapvr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtymfrzk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3udmzpyfs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bygjfyrl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dvlgshxy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3aolkbpvm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ddwcnxrs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tgnsxckw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwtccjx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxtebbv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mimxwbmv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3fgqnflrr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3lmtfhrox.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zxnpneav.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3pljstzoy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aivtevrr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lihtshno.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rtgqrhtq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jyfccuah.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3uwcjbddj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eaiwdzts.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3njvrejhm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ynsporat.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ixybbxvp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uzpnfgvm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fqbnwyev.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fuzcvfqs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3apftuhpk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qyifopop.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pnmhlhds.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dhttzfyv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dqikaqkn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3owydhdjw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlhnyowl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jgqxlrif.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzfyzcb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oueqkslp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3owgqnznm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gokfvfcd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtbipqo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cazjniok.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hgtxputx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rasjniyy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3buebulaa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ypftjabg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pqgjbmjr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ezulftup.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3prdbibra.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wkniirnq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zdcxkzds.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3prhkahqb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zatnhstl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3flsenzdx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pfpbgwes.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wmkmrryh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xvgauyee.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3hnmwspvc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zxxehpyt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dohhjauj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xfavdvhx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3bsbasjid.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvvtuso.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xcuknpvl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rplolhcc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ryaywkmm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kiwhmjny.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fvvnrjkb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ewbftyrw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ebciszuu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pvtjouwb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3jxwwayjo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nqtefqmn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3prjexqla.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uczlhned.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3djfzinav.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fckqpqrn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fhryjwsv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ikoydtjh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fzcvqves.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfvrxfc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zoxdhuuh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3vquudfog.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ftystkmn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kitkqncd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cbkwaqra.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gpoqjtet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hharjbam.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lkxmhgrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzqthtnm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ndpnynkw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3setqvqlt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaziyeiw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rrnvdtkp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kkqmcwar.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ynlzsxsx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3flszbdfn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cdiqxaoh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3stjqilwt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fkdwsfvx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ltiwpigw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ibxiylrj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qoqlncvx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qamgkfbj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xwrmbmol.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zukdsnju.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gyorwxon.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xckocvlm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ttzvszmn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3eccnyhuc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lbbdzyek.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnghbdbp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycbyxfdu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3geolmemj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhhagyt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ktwocrzp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rjycbbgp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rslhyijx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ytbhkqdo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3flkcywop.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zruqbjer.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqknjkxq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwaatiws.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3roelrvjy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3amnbdkhy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dyrrggzh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nhepekua.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnexvyl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lkvlzlaj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3imxykptw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ophingyz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfvgofyy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fbbtxfej.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ucpvlakr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ydeezavr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ugbcwzsa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxiwuks.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kdjwkiwm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3njczzfbm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3alyykyvd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wbsgrtob.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gpbzibrk.html


<!-- 参考信息 -->