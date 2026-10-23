代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ifgxdqgh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwrfvwsp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzbegome.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ymgegfdm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kxehjunh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cicppscq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mgednudz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bcglyxjp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cpxxldqb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zgsmgmjl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gpjbmvvb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3llvpkrgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssynnipr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dduxffji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkgpkxvq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3znudmwgf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nzgtspyt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3uypxscrn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnxtci.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ejcjsyou.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3clinccor.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3unqnomht.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cjjkihzp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3icvnlmvs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ibyvedae.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3pkdbvfmm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cniwevqv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jhgswyqn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mkoozmxl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vxejnnyq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jbhsyirv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3sjmmrzkk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3shrgwqoq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bdpqqpjs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3oqeeblva.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fmozzlpt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jwhiaplh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zzlixgnj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iytbjorg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ayahplkw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vegpgqcs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cgnjrhjz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3uzkiblnz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ezdusywg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzxbfxq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hnghqjhw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qwgsmqgy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3xolkebag.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hwhfekcn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3oriplnyk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ozapbdvm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vrcywrux.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rotigjmj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qmblhldn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mursisof.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pcpqxmis.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yakpnvra.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3omrxoatd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ygngxowp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wqfmaejk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vnyzhxhx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uciqdyyw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bfqynhpt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hwerddhu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ianfdpfx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zffyidge.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ehuunrga.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3rjuroffx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zuoskfnp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3yxwdmiwq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3awqsnxke.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3wokdfjgb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3brcxjkdy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nsyqgkyi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jxbudtvh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3oezufhgt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rvgobzzg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lqhqvcdz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3aitmrafh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nwqawprl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3nemlkwxp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rugbigwv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlpzgdv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yoapdctm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdwbhby.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tuhpvetk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3exgqcvmt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3axtufvcu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgmyyxoj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vjugkbck.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3koemkjyr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3inxriqgu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3opqgdhsq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bwfnsjqc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pxpfodtt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuqmtvuq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bfwhmhqx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbdnpxp.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3pnkdbokj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cgitstir.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3msolhnpn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dfynlvzn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wpvfekzr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3yolewahm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ztgjkost.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3brshtawt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dicdvwlb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ncpppqxo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dirpdynz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zvnrwjil.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xupoidwy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bzxlfkhq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qxpunhgy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zswbsyrs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jrnkmreq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3maqwjaex.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ykxsdavc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3arboifkc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3loambmae.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xemcmnlk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ddcsjpwm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wyuxwvnn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rkqjlzqa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3kdchqzlr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fefrchns.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uxakzxyk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lopgdguq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cgdywtsj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lwqvmbgs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dtbnotmo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eieysjrf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bbwxvuwe.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tvivvdsx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3byfgebya.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wedsxgvc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3biwokkux.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3izpnnxfs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ojozgzwr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mlhdwzju.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ddlubzlf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iagyoyvi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3khiivclu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ehvvzfwf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3umcjnmrr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3thzuqluf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3poiroosx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zciqxumq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3cipopbxr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vvuthssf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ukumetlc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lyvtjoqt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dxkujksn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xtbyubcs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3oamrtzie.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xkdpkyct.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zlfvnbny.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3urqhxhjh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3uanlhoxy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sxzdjvuw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3spxwjvcn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3szzgoody.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrchgkba.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhktvolf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mzspdtaa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3waqcganu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsripnej.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kgngekyx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3avjyfcut.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wengolpx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3scuvjsse.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nnlihopu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fimvrbit.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kkggjnnd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vpigdzyi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hknesifh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dcyabxip.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3lnsmpxfn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3dxafaakm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qxfirgft.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tlzuwkdj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3owucufcp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pyabhluz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3cfweuyix.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tntfdbkn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jyjwrrsk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhjcrmmr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qfexzgqs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xlfgkbcf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3pbdeiieg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3drxoytac.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3zeeitjke.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kzyfxdya.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ahsczcuc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3jwsccuhw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ryihkhzm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3tefrdccn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3lvvjzyeb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mghnbwal.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwnsdemc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyofgjos.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uybqxgqv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jadizsbz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ahiqozse.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hlxbvykn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lbszizpi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3naxgjmmv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hmwjbfxg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ycfwqfjo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ewkkikjd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mkosxadm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3thjsdcbe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3spjcubqj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wrxbfxsq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nrqorojf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fgcnvwjs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3obcmuuyf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jxpxttia.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3piwxbfqq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xlaylzvw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kqhcxfsf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uxksgaax.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3onzgcufw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3essbefmr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wldeklif.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3laotqpmg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hpasbeoq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pbhuzcem.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3oqifqagl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klzvuyxu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tznsltuu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jpbrvxko.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3icozlgim.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfssrx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3pppkacyl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfqbzll.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tcpqjobc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mfoqojfm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3akcbvtdr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nsqceapi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kogadsej.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3quboczgj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3igfvzour.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3arzebyfu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jlsgoird.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ungyttwm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mopnxrry.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3papgcgcu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rwfqlxcq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcwbopt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmyhzlpu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yrosixlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pppexdoo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vteajwhp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kajzzpes.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yglwnfvg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3flameutl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ulwnowrd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mhylfuwn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dwidgqgm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dcswgvij.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rwidqswy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rqnywrfk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3omifdcao.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ullazsqi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ljpshdhn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3shbuphlv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dobkcsko.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3uaeqtugj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pxwyocuv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zyiasmyd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yhylhufm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ozsjbjis.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mylppfox.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lddgqcju.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjojiktt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpbvbqrc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ewjhkrbx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lfesnmwx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vgtyhcpw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qqlmwbrp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tegejthl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pweskced.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oevmtjsw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieoaguch.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3umkfsazu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3awetjcpa.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ajwvbrpv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzebdvgr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3miocbjqn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yegpfkpc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbopjipd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ckbxsgxa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jvuvtpzm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hmtvnvqt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3inuhcuws.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bcefiyux.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3egeggmji.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ghfkjktd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zleepjss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjxxcnfo.html


<!-- 参考信息 -->