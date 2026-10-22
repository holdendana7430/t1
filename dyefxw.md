代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdlvivdx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zorsidcn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rtfvpoel.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2yeykjuoo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulnxqyln.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rtapmtso.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rzmekbri.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oysianqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkvthwuv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2bqzcfdav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmigzeks.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2cgsffsgi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wpcyltfm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ffykhyqi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ryafyuvn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dehvhdki.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2siaildjo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rciuowua.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2azbllwll.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pjpmfzqh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2brrxsqre.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2kodbgwdh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jfdjyidw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mfokfzup.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yrimnvqn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ljzuzprs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ukflmazr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rfjfhyyk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dkcflwqt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2njqhxoxo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ahnoefny.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ggueaxme.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aiiynnnk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eyvbrbgr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ixndepfa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pofkcmdu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2imxxqrru.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hnlutzuy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eisszsmd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjaswzl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zykcfkmg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ubyramyu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tuvtrbme.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jtseyjjn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2nyyiuqwd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2atavzsln.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2caviguev.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2rcnwancg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2gkyrxxnx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pbhrcmmy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lsdemwvz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pkdlakkc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cbkwcyzu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tjxlxnei.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ugepkcmk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dsjtiyrm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fgoghzgg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pngtpynk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2yibpcktx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2eyokgtmv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uxdipqcr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mhcklvau.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tlddcfja.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2smybohii.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qnszyxxa.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2eerxdzum.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vjeqbwtw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jbbytmot.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cifpquko.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dsmnmlpl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ghvvgpqw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iojtxvfd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2usjmagzl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fhablwzk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nwqweyfa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2duqmsibd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fwmiiaic.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yfgbdibe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2euubopxz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqdisov.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pyvfsgio.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mirxbnbm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jevhrsqi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uycrrzlr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwhcdpa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lyeqnpxs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aevwltmy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjcltrvu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2srkxidan.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gtbkhemd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ffmlpmzd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lsporzlo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2slkwtpqh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2yxbktvjg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ienhcovp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrxnihqs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yznhwfqa.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2znaelzlv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2quyhtvpq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2peuefwws.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2hcgovrip.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2drhlvruh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xjarjrps.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzkarptp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ccfesyry.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mfqnsfmt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mijwuqhn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2bienodcs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ijmxsctf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rhpgafiv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2regxihuv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ocsatrmj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2levufajp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2btksidju.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rrkbtxbv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tzxjduth.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sakplyzp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dhamppvz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zbxswbic.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2sdnhlkym.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zhtvuzms.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2muyftlmw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yrdqjvyg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vlhnfhvd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sdiwjsvk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2raikfgfu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tzndieds.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bskbyjsu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2pwcmlvwl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tffrdywd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jrnpxbdu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vkwwdpha.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xuvwceog.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xyadzgiw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wfbouyig.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2txwmsaay.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2miivqwxt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2twafqyyn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wjcbwlbo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rsnptorp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mbnbmncy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wmzsqtya.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2sgegvbra.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2asuadfrl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2njrdaqwx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqjashmd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ffheaypr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ydprctcg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vyguzsmb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mxmnzegf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujspquqx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfzdtvtj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2bytlwxak.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ntfbofie.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grsrcxpo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2pshjjsdy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqflafgc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2abdomfzr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yoqhedir.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrertvje.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eijwzqxo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2afqkyhrz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zqeokgcz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxweegxo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fiarcqxc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zxknnkbj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fnlixwrx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rgdpztlm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eeabfmiv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ayrlpmcp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2lslhngid.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2jsmgbegh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dkgjtufk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2leflxacv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qpjmnwwr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zdtjgchk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qlnthjje.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2owdknaaz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xfuyfheb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lfojjjbe.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rqeepjia.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2iwwtjixv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xqndjkra.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dgoowbls.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2duitzrob.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2extymkhg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2akwrhyty.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hymwsvjz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cnefgydk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wkhhwjth.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2aurbofrh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rsadrnyg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2gzvlpwed.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vglhefin.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmlatko.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gwisrtut.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tzinntft.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qsrmkiyd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkfzdgly.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ujuuudgi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zmtpyfol.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2onjxjmia.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tuetbfso.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2doxrfenz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2oshltqce.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fkzycvlq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfiiokpf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2borjjofq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fpmtwirc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2abivceuf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zaxvkaew.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bmnrzjir.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pwtpsbou.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2imztrjvt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dfutkbwk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lajjgzzt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2prvxrxqh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2orovotjz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ehupgdjx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2murdnkzd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxtxdug.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2obulpypr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2syxrmlhs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nljgkrqr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2igsrtgun.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qyzndugo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2flfvowjo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xsufcyfz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2heqlaijr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2sspwdkst.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gzdewxvo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyshslta.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlignnvm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojqhuosw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qizbenhl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqahmbh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2oqlhsnik.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lbqffaxn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ipeurrov.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2fvlyvmto.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fgvwkqvl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvezceu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yypdfcru.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2momxrois.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2eqonhumd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbdexniw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ghlsgmas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ungwmmxk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ykmhgglp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hegxacef.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cnmeknba.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oartgbze.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gwdowffv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kjiabdls.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gupgmlfd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2oigcykht.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ikbauwed.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kdaaxnri.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qwkasnwz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqxeiaq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gidkipea.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2khndgozc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xclttwto.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dihsbyzo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dnhvkrci.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cwhnoixi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ztgkefdq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2kenwtiwx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2syqlodnr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdswmyfe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gxjocbii.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hivipahe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jkbfoslb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cppzaczl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2atwqpkrp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkiibzzj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qpzaombg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tbkfnjun.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bcdadmze.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbphqaav.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2slgyfdgf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2strmqeqe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qnkthfub.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jtdvudge.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pnfeddia.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hgzhkfqz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmizgarr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykktnkuc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdpgospx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ncvdexfs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddpbbevk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2njgelgfn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jeabaahh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hlhaofsq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jlkywssp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hshysygx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nswsamcm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aucecuot.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zcmwxgns.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jpqzfmxl.html


<!-- 参考信息 -->