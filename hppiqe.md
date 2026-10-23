代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ilbgkyld.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vpobuswu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsvphvui.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdsqbjtf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ydriccdc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rirbzqee.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3icvbtafu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3finesuoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kluljafm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ypnmebaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cndjylch.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mscltxay.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3walnkgaw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tmnpfzxb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xbxmacxt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3udkzrcfm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3osmehozr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kxqzfbxt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fcfcoazf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gjudlkja.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3votuqzba.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hrdhqzzp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jhkcztjl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uwhrkjbr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3widzhuxa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bcqpwbqc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ratnflrl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3djhlzysp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tckhnvom.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3oxuifsnz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3kkwfvpjl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hmehksnx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3leipvkqz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rnqcxifi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bqlkwgbp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3namcmivs.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ccuhafxv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yjdnvtio.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3imxrjogb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhhnein.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bplqcgkd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3iurapjeo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yjyyzuud.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3zxgqefrg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gchldnxf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qfsrouec.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3sztrxmyd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3plionspj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzubezhs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3viqjvwuf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhezokgs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vmwlcaii.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjsqqbtd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ckzfdxkz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dzylwype.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fhvwssld.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rfslarof.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hoonhtpv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uhipcbfq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qdclyscc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3loqyqkkc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3noonerne.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rmmwxzpp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3uwrvpovn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3errvyydl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxqcxvik.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hlfzcche.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kjjomejt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3zvvnkkeh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gnbkspet.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qpplvcjv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ooechpzh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3uartgrce.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3eujzptbe.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nbqgsxxo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qpiwdkzo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hldayyxh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kjtqhfkd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3awnowvlu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aqysuvnm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hlmnsbbp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bdrqthwr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kyqxtbpa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ubeuvwca.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svczvrjt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqhrsmky.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dupojrvo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbrwkma.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lariagru.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vzgpvxty.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ozvmlopk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3slgehzbk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vsybudtl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ekamtrtj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cnnnimlp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wueoayti.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xrayhfxe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwfwemzv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wckoqtyj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3gitbmbel.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzmwjpd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnhgxp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fsxobvln.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rzdgzidg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ggfmblen.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sqhvfiea.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oztcwqvz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fhatqetg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ukgcncwq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dubefmup.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lxbjuixj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3wbvroohx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3srbkiawc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mrblquvf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hjxiqhwx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vylideyr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrclgfbi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3odxjsthg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3idfcxlgm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mbrlnkzt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3htxtieno.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qyjagwdr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hdptokga.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lvmacugf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qyucdkzr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3khccnjia.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ungrduiz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wlpevdpr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vbcgfula.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xsputjri.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zzewpvsg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zjihnixy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jipoerrp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qiocmncp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zpkdflvj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jtaptyrk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lfjkraom.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ajtwbwkk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3owhjmpmy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hctkpxqc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zrlpnjby.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rkeyqmmh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hnhlrdlx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3sfnczuak.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wwyotgvd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3prxhuwgl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ffdartdi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yfqsgios.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bmkhkksl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3yzwdixrz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfhgkfqy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsfckdbu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dgxyhnvg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3plxqpwuv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3whqsjvim.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3gjrydxji.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sblagbtc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfjqgeep.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lbpiohmj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uoflryii.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kydvbder.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjjuovho.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3onjswism.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mixvpurk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vprezhsl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ggtwsrpf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bymbrwxa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyiffsr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rdksvitu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3bgkbqbtv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ynilapou.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yxruvuty.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3tiqpprwh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fuorrxrr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bavecjsn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3snbvfayx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fywfpraj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tixjlbho.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mfuiajja.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3soldwomw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ujlywdjt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tywqeeug.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3syritthh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zkkhyyha.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ikoxrfbb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qdrnigke.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3osswdinv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3katqetnd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ntarkank.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ibhcroff.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mqzwxmxx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ydwdevob.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3aryfjenm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gthqutsb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnntkrvt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnuchrrb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mypmafuc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xduvolkk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjelgiy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3emepdtri.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sdeunzyw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wabjzqev.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3wpeczztv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3axjprxyp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jrxctpst.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gpxliasl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3pcnlximy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bgotzron.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3osampmbc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vbwfwplu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3qegkojjw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgpnatlv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eaqkskyx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sugrpgrh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zhdpevyg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnomtirq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ezyeisrh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3bcwyyocf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3dqwizqcc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ocknaaln.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3omkmlsyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dvzljhqb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xehcswdm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3vqospnuf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cxiismud.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mndvsofn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ubkwwtbk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cnzhgjdc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3njawvkpj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3uhybtrun.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwikmv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lehgsvwq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dodreehu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ycxsczme.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gtbrwdwe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vydmedyp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lvwwcyta.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3woyxeovd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ewinudps.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xroscnjt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cvmnwxhc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hswomzhd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cykoaxfk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nyvvgngn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3whjqlzqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3echhewaa.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pmoudrwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztejeyvh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3lhkjhffz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3aaakcwtp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmigsqu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bmaotztx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3grdghpkp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bcwibatj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnveqel.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pglmhtuv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3unegpecf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3scvvwscy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wfnmzoag.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myoikuae.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fddapjqu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ikrdaeop.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3whtksswu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ddahhxbu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3adsmnwyh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ugdmotbh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ygazdgzj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3gvsdazsv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qzqxreyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rhwjkeyy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmgcrpvi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcdxbmmg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3asarpwwv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3efyipjrb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zfhkmrxu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3txmbkwvd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vofjqltd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zafdtapw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkvlwgiq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvgmmwfo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dxzeibtf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3quayggcl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vpcjqhrs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfiztdkl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hhmznyre.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xotthugi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3sjpxqcjn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3umvgwmjb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhhryayx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sddyeakp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3plehtvfl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wmiklalb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymhddmav.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3coivctfj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3unyaxuug.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iesprosg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3okqxaqqp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sehawhtt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3owbuxlyx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgwooan.html


<!-- 参考信息 -->