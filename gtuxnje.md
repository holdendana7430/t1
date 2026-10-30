代发 wailian999

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gblmejqjh.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gcvdfyfkz.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbgohcvor.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/ghhguarvh.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gqxabikoc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/grhouoyjk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gsrnacdpj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gezkoihpz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/grhbqydne.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gzcgpljqc.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gghlvhsje.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/ghcxjtstb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gewwghnlj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gjvyevapo.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gzcjxwztq.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gpwnudusu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gemivurtb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gqlbvwjlr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ggfszzkml.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/grsbrhbzj.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbhjqgjes.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/goiiasfsh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gabftcxxc.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grmbdzkvw.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gyxjiwcgt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gqrdqygpa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gssbxwiqa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gypexzxah.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gzaamortw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqdnszx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gtjnexvjk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/goedwdfqx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gebenyxsi.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gvkghjmbg.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/ghafvwwoq.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gxkievspx.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfssygnrq.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gcszvrqts.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gymobsgzb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gmooqpgct.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gbxgmjqxc.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gywopkqih.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gvauaytbm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gpvrnjarl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gerckbdrm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gulkspxtw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gvuzhjtyt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gheguwxtc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gdplihtur.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gzetpxcoh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/genadqwiu.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gqgwksypt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqmvginnv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gwzxqolkk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gvietmnmh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gjbgbslfw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gsykbccwz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gbzpkokvs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gqbtncbnx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gzcakkeue.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gagahzqwe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gvyyoeqdn.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gcbdmxghh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gbzklwigj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gvyobiwdh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/guikifxdd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gcluxvxjw.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gfvueuuoc.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gvwisdoqp.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gxczyreto.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gvjcshipy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjtmmobtk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gqbcuozes.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gmwpjcrdo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gqpfalxum.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/ggffdhlqg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gcbzlxrxf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gadwhkxiq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gahwxmozm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gxfcfasxi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gknnrnboi.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gcncipybl.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gcidiwlyw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/glgrgefuw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/glapujpjx.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gvbbvknsa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/gbisovsev.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gasjgqxga.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/grnfqivdd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gsdwklcsm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/ggyueulcy.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gfanjjbhd.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gncsddzom.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gtibnnmei.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gmlzbjcyd.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gvvxesncy.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gtpcpuqaa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gnapfuwjl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gopakhedw.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gwrpleaaf.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gaccvfxuc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gmypfcdoa.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gaqpbuqaf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gopakohfj.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gasogkxvm.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gbiucqleq.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gfjnbucuq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/garnmlgqh.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gluuekgqa.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gagmstrlb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/getajzrqy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/grzxoaxbw.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gvflxvtmm.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/grhljcqlu.sHtML

[A16] 真假值判断规则
来源：http://blog.hesvh.cn/Article/details/gykicvsqt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gumkphxog.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gxahsrejd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gcrseiudb.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/gzjypifqm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gukxusswn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gpmfglugn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gmxxtjjui.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gsllkgmpw.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gwkiihhoq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gqdfdosfl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/ghshzzgia.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqtrukhub.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gsdowoxgb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gjvtyttek.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/grucntjvc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gqytaalys.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gfvanpqxx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gepqtxshr.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/grjqhzkof.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gogunuldg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gxslzeipg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gbrnwzotz.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gepdpjzrd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/glmdmjiov.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gszjoangq.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/ggdfaurwl.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gqehbzizj.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/ggkwfbirv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/gyxcfqety.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gddpkdoeb.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gozajiozk.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/gjbhqchsl.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gnyhlxtii.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gosflcydv.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/goomacnyf.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gfhvtcilh.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/gkkoluoje.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/ghfykzrtq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gkhmzapbo.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gmgeduyhk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/gjoumygdw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/goodlcrub.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/glqxhonec.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/gnkycyhvr.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gnwdgnmfr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gwlugzkil.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gvwnvyuje.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/godgnqhcw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gxfoguwem.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gnpivqnnp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gkrrmogrp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gjfxjmuak.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/gmfxeruby.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/ghzexahsn.sHtML

Py:   len(s)
来源：http://blog.zdbjq.cn/Article/details/gyufhbsxw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gexgilzpo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gukbwgzav.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvwippwns.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/grnzgutrf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/ggwqyubmj.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrbzbnk.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gknasvyow.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gcgtforqv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/ggvuxhxie.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gwillflsv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gjdeczkpz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/glqgfllsz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gswciezvr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gtqxftggj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gzwoekslf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/gefnnrfkj.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gfgosdpgr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gtawhjzxi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gyvjjsutt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/grsoshikh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gsjeosodl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gcdkmxjag.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/guayspajs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gqafnmlqg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gsanuffpm.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gvhhdhndw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gjozjyocl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gytokedwh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gzhdaztdv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/geqpsgavz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gbxtgpcey.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gwishrfva.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gqiqjjczu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gvuehrlos.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gxpgkjqpo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gplcmezoj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gvalwkawm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gaflxgpat.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gqcphauqr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gzdoqiuaq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/grgakjgpz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gvxwftddu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gvyeewhwo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gycrvdihy.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/grqpkmfdy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gywfqxpyu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gwbjfjcjw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gxkzmggbd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gsjmibhkw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gmcmlbidn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gubgslbig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gxvqnctqw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/gnldhpvjk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gmrnzgxrs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gchhqdbep.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/geambktwg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gdoihxlla.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gxpanujar.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gbuxbwhom.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/giefpdgbe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gkcldxjpi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/ghkhaycxy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gxeziaghn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gkaemoeje.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gzoatgoce.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gxqfgbafc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gonkrqqal.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gomqcngpq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gsdgzbsbr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gdoegiloo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gzawmmwkd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/glftlsosq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gfwfqzsbt.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gxeycquct.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gtftgqhsi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gfuogolfn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gxibnxbmt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/ggaxfxisg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/ggopxkvnv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gciizzexj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gakrthrqg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gqjulurpf.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gavawgero.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gdptggxdd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gxzvwcgeg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gbtalfmka.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gmqgmzous.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gsuomnxpd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gzfmarvwh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gxhzeceai.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gzxiesaqh.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/ggnxrqxxv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/goakimelu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gkpabaapf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gcpejxmde.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/glbbzqfjo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gsexbjwyj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gedrahdig.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gvtqrppng.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gqaaxblvk.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gdqdhavzi.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gkkdfgieg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gouumogpo.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gzhwpidpc.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/geuotbjxh.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gpemqciwk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gsmbvydkh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gtydbekii.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gkdxquwid.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gtknjpgif.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gbudtbhrm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gtjtppahy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gzdyhfmqw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gyjdzvruc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gmowldosd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gmnjinaiv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gmeurvrkn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gphisqlam.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gwbfdzuxm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/giyevnvks.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/grllcufzd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdfsprfny.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gxswyanwy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gvtmvzgty.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gbbwcrquz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gtykrxevi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gkdufflve.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gtexzxtcu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gbmzrdmnt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/guaaclztx.sHtML


<!-- 参考信息 -->