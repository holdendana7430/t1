代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ndtqokya.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kpypgfje.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rbhoojyg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2pstusjss.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cihzrknn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jasnqnng.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wnsrrkfp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgdogizg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfustazc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxibovnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gregtvbo.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eseerxln.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zosiuxts.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2hgyqezhq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zcqsigsh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zuetkqsg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hgdpznka.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tmzbftvh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wbxtvcuh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hnwlocyx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pfkqgoss.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2uqdhmmdv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xujwxbrb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2scsprxnt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lrisolqn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2owoegcyt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2wmpkxbbq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2slxotroc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ilqjmfyg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2usqmavsn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2hmgvlvms.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rxpouiix.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qlsanftg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ukzponma.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uccrxurg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cvdgcwkx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pygktlcp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mbofzkko.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nvpgsfph.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cczfrlma.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2micaqqjx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oxbamgyh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vjcqsxbm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2prmdtyhe.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ijtgqnex.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zkrnoobv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ewtgiygm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jakbcufe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2anmzwnhz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2puifokwt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fwlkyyno.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vtiytvtq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qjwxeldd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eahqctms.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2euwrczyj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvarhptc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mskwitcs.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eqlckeuh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2rgwsqnaa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oxgbdvwh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wcdwyujt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uujkbtdl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nujyanxy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xzsaryev.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rmetixxx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hammlmpf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rjtgozym.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2avmnsnta.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2owcbuepu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2knmyzwag.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gizxbkjp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2lsyacbzx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ahswmlya.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jdpgsldu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mfkryfvz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dplnlxwj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zboimtbd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qyyzmcqw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fadzyuiw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2acskuush.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tllnebgs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hhueldrf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pzwekban.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wvgmhove.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzfroluq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmiugdnc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgklwgzj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcllalyw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iyekiyta.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2teaukkyv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2eeanbgfu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2znflyvck.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uxonmrll.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2damxuvip.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2spqsipeh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wffkizyg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lyvianhd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lnjkjtbi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2gglivjed.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2epnebvrj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mjfhpadc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dwcklktd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mivsupak.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uikthmua.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zmjapxgt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tgnsyoiy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vfghsymb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xrcxeibs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdcptbch.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2whhredvy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2kdlimooy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2motmkznx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfpatky.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2trvntxfc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mzkbpufh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqwrgcy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eejutnbc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gztemymc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2kcwrcoob.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kcvdmdse.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tmjcwnmm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jcngnqml.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2antfkipu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgastwzo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qbaxhtcy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2phiuinvg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gcbixzmc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjzctonu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2hrwdnfad.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zkbciqvx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ilefwxra.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ondzjngy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bazvlgcg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wdnweovs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2slmyklxo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2bvmffglv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ocltepnf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2wxzdfilv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mjjoabmn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kzpkkbrg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2krvndrfe.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2boyqjkyd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mgprvkci.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vvdghmsn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xqarwzsy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yuqmlbrm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2egjiuist.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2iwuxfpgc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2syurulyk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wnmzedlg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2uiuzvado.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2eppnxgnp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lwqggfdc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rpkrhygh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajonmiih.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fdaalqcn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mmeogppo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvfjjwly.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zamlqrnm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fhcmetob.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kysodxrj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xdthajkv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ltuxjdzr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iwncouff.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2lzkofsfm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqfbffl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2clexxrpa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mbyudsjt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ywquystk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ivehwmly.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2brupuaet.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2inkratnu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gpbvzept.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zofxfbhb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2seqfrhhw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bioksajy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qhrmcpjr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xlhttwuk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2srtsaypw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2llveiyzv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mhdgtfgu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2smudfujw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wbvkkcad.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qbelpkgh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jsrxycbi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xanqxpin.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wgnugpqp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xngwbzej.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zoorpumv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2lnwnwrtf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ebpgxhgo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wpdqbohx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2njxrtnil.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uvoqomyi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hdwofxwj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bepcbfma.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gbzjsjey.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qfgkcong.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qmfkitzs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mcgdpzth.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sdlvrgpz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cisvkfoj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zimllsmf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wnqemtzf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wfmcncoa.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ezpbpobh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2exwunntr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fnniurdz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2djfsfcob.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2enhorjcx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hhyzhrqr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwgizoi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2toflgwqx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qgcuzhvy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uckcaxib.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2qetqthpy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qjfbnhbj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ltezshsj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2guwclgqh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vqjqfakb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2goudhwyk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qhurlejl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tklrrvco.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hoeaochd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lveotkqv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bfntwxpo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kxmvmhtb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bxbmgvog.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kjzrsqty.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xlzzxyla.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2umsdgvxr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkkidxo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjytmxbq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kahuvvaz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nuojhwsn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lisovxlc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gupgqfuq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2pfhdtdvg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kwgtmjqi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wlrvgqka.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2royiopvq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hlrfvxjd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2idridehy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wsdhpuyw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2azfpxajb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgxewbeb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lxpapdmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2legswzwa.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dmsjhkwq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dylccsgs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xqiwhqgu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xzjlerrs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vivmaroe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xyxbiwpx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cctnwtju.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xthohhyl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pxyecvhk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hcbjpfsf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fivjisyu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyjyqune.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ycxqhxmo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ctjquzqi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oznjkpsv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2puujenid.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2talrtvuc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ogtvoobm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mwtijaja.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2snqkwmvw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mowyxeam.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqhnfdh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hquhlwtu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kwinwggp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eryzcoys.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2tpnwlixr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2garcnibh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tdwbcuyz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxuqvek.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2weweefdx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eztkdlve.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mgrbnsdp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2esfgllxs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2eieykvzr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dmqhljde.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ktypbnnz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gflrwscq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jzsyvwdf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jduguvlu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oxvmcddq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yxezsuxo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dwuuvhhe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tyurdhxh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2unmwzrjo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sopyurja.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nsdewqaa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qmfauzzp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2twetjcuo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dckndxwp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2otlnxjii.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zistgqlf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kyozycym.html


<!-- 参考信息 -->