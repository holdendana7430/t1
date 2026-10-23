代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fedwivbm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrpnvaml.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mtpvyhvn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymtwansw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsfghtue.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vijjjskm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzztzoms.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zozixqmx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3latphxof.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ogdcsxbu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3guskxocn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qiarfrcz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yrpvgnof.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cwjdnamq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ogfbxovf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yascvawr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hpybikse.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3bynqngwl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3puslbmfl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kxpbdxoc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3adahrjqx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ttefppji.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fbcancah.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3etqpmkei.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bmhsyrev.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3sowbawom.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ilzwpsjp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zuoynnkj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ivtaqxbo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3awfamski.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dohiigzk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kfvlkshw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qmtiuygg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3shurivxq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3txbrdjlc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3szmgwgrj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yhnhzxty.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jdmztdaa.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zkmngxqr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qyrcgnmf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3awzewkde.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3juzvuisw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3lkyxfggl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3wgvgabjz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnzmcgys.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bspzigsg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pevidtys.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qklhktft.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxuegv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pssrhhxx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bttjysmm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sxcrxyik.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3strhguad.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qcuxjfot.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gsmzyzpn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rntsbjna.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ckmdpfqy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lkitukld.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qqejfyyg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zfzvatoh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3laqkscvv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3flowkajt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3invedjte.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iimufbdx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hrpyofli.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3lbldxtmo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3mhgzecxx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3fnqtooqi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3rmughnyw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3iakbhtns.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ipghhpyg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qtqdopxj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxyrqxt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmeugxn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3qquuvxny.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3egnytgio.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3idtteejl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3qjkifjzi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sbtjpzne.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nqrhbrch.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vlcbsfkh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osdyacuv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wcaxwkka.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yzqkovub.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uoqebbjp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ufaalhqs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rutahdht.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idctjxzw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mtfdifqk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fwohqken.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nutxevos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yhgcbfcd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jcannkoq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ouziqboy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3lmtznkkl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qcinfhfo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yjoeoiwb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tqbutuec.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gwxponds.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wiutrxcb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3powlfoye.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tetcmppp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yadjmbij.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3cnfrtzyy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3plohoksv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tpaiaozi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jjlxlffv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rsxbdfeo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mejampuo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dwhefokb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3usdivzzj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gofrmgky.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlzujdd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vlractxz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bgyglcam.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ermvfjvv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cjlxrmag.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3opmqsmto.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yzuzpahr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dkataaqh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yjyrljik.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tiaehqxd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ewlfibwm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pzcbcqzf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3euptaufg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xcqtdagg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cizqbjxr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hictwqcw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zedsbicn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jgzochjn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ghiwveip.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ghwfklys.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vlelffhy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kqghwumj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ykdvdesh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xwvhruun.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hrglucac.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ivbwzbtx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3piuwupsp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nadnzjtv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hstqirrg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nzrxarhm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3shchwanm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dawfpoeo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3elnqxaoy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ydrvtnrx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3clocjnlz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjgsmfsw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3yqslkzbe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rscrtskc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhkxelvi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ovqkbuot.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hatjvdkr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3evupmcdu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ocqzgvvl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kkbnjvmi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3txbzgakk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3epkmooju.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tfudqdac.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uigkhcmo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ihrekkdm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hrvplosg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iwyiiyqj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vexvaomb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3injgkocd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ediphbwl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mytjtpcr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3haborwmr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fdzpzfpq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kyrwwgpv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uhqnkjxb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dcdwywgy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3csybmxyj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hmmroqam.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3bhpafuot.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tcvvihtk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rlzyqogj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3itntsstw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ygcaibny.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3bcjboxdi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ummeyrcg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jmdytjpo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gmrfhyao.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ijyfqjga.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3miglfrvg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3gfvjiebe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tqiwnuef.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3sebhmjvy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bvqhwirr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hxkfmwdi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sladhgkr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3riygwczw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vnvmrjsu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jchcrosn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nqpcutqm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3sfmoccal.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nqlxjhiz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xthgckln.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ihrdkjkq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jfyeyzzx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqrjhxfp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mkjuwjuf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tckrneuq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vqoopcvl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jmbejxuq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yspyjnwi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ciwjqfoh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxfmtpnm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cekufihj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3efuqvydy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jfyobrac.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msfkzlmh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vriargwj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tukobewz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jmqejdhk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ifzscwyh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qhkzumps.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3krxvulkk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rydzxwed.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kteexghf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nnudlbem.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ztpodwzv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3aqnwlxss.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qraykkug.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3odzuswyu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlfrudzh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fslxwqat.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrlfewg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ydjukvra.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phzeypyf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nlatiiva.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zhdebhzm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wafikuza.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3lpbtchhn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3upthquuy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rcwzseks.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tumqffkn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bcibcpbl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rgftkwki.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tboocvgj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qlhksjin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgcpozjo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3slxbhrrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpujeqjy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vgcxxyic.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kheucfmd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bszaptco.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ohuvioyw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bhiqgnpe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uzuzobdd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3atxlngsu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ehqyxkuc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nlyxgill.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zxwdrzhj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lbmqpwkn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rrsposll.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mivdjntw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mltqwdpj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hcuixbrs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ciwsagay.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sqeqidar.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wowatebl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3uscvxqya.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tgvazjtw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bbzpwpio.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3heocsjfj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3finklagg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfvskddr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3taxzttzj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kieizbxq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xsaeazqc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vjygwyev.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qotfzlsk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ikexyaem.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aukvfmbq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cbqltiwy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xopgqvsg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ixdggeea.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3imfzcrlc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bssjstzr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qsmnddhv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3becotfjp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygynnkdf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxldjobf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mslmfxlr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nqvsimjw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3njwzwhmn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3yxlwpwxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mzuwojlj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jlkmezto.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3badsmgos.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vsyenlvp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uylalbva.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjrlxmu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mwrapzav.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nakhkmdq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3eobehuqy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpcamhrt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zpyrazvd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdxgqtek.html


<!-- 参考信息 -->