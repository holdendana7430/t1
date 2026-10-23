代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3gmlvlouz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3cjzkyvex.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ariwecvw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snfhidax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bhszehzt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hljnknqq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jxzxmkfe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pdwqxexq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sapuosey.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3thttwqom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqbzzbqg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jfxgtbjx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vwsewzsx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rnvxuhpz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xsyubovw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3aublzsem.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3chzktwck.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vkdimzrj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3afhfpdnj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gjqupyqm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gltbxcak.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zmoffkxk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eghoahny.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gfcbjxvg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3twlbktxg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3emnbibll.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sffxmedz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3wwfuabiu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vqjtejex.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3mgozanne.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3glbglqmu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kldddrpa.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3maggmjku.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3spahsbwb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fzwshykc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3totbcuyu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ymyltxkg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zeqysqju.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3edztiayl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pxrfqkho.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvnyfdj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uvmdauki.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3acfeirqy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3sfamwzow.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3sjouscua.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3darqntms.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hnhqkbkn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3kdswptbu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hzidbinw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3quocbbpy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cthqivnq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3crwecrdb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ctgwukuy.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tmolpvgg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3scmmrjlp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kccjdweh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hqofopmu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ukpdnjbt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vpkszval.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrhrjfr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hgrumdyl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tduttanf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3mghxtoyh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3iqqlyrla.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hnyqzpem.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3dnhixezo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dbmygesn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ldrnfxnc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nmitaisi.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uyfrfehn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ypuazcmb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3pvzgbehb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qsnlfits.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3vpfpkzlc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3cerqclll.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ammpytsv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubnrnywt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zhozexzu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ulloqasc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hoepydak.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tdhryvjt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3spoasebu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3btrpdpcb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ovhxmcib.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgguree.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbjvzwoy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mzbavmpb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3azitnria.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyzrgbxu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xgugctvl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rmabfgle.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dtgjdyfo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3pmstzrfq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3yslznrrg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3lsrclyyi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3glbkpvfv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxtlzfng.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3frbwajve.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gjqjehow.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3whblvzwb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3afejzjvr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3luddkluk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3uczwiepp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wberotmp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3etimpump.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gbxwfetw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nqlrlmwa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3rtxemzwn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ewxwppvi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3inrpulys.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gejmnsqi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ptedpjyz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgvpkpr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3etufrjbe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3brzzgvym.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ptkjwpqp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhtcgsf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gtyaefzy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rkdcwney.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3lxubebtx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3plzybjmf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3njcnndur.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3njcuenoe.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3amwapnoa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lmdhvzgz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bkhnlieq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hduvoxyi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mdomtfff.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hsreobgl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bjbiuxfq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oojlwwzc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mdyuvomb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gqzdhons.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3tmczhzqx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jdifmtno.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vjtzwprk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qurslbbu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mqlykyoj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ubolocdu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tnbofkgk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cmifbbpa.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3flswwnvb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gjflgwvh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yzucbqho.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3apiqizzp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fwahffbt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ycfkgjfl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3iufzvsqx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hfrrqjes.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3bvxgfhbw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3godvqpqb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3aleqquad.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3tkbbupxb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mydnyydc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uvmmhdcx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3eipfdeer.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3olbvpgkz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhzhsakk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvoeszoc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lkushkor.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hjxztera.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ldrlvdpq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wvvvftub.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbsrcktv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nrgemsul.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uabhjeqd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3beuhlnnv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rxlgoeuo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wimbmctl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3liwsmdbg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3yfrdxekt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zgfwmuda.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nkbsxjah.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ueprqygk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wpqzzucr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vbdlemky.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3etewfqbq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cmowgniv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3etrdqmlu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mgdqczdt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hsaogvfg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3djtatvja.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rbjihylp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rvgnalez.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zuelzklr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bpkwznhz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dndamdvu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3umsokxww.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vyvkvhth.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hcahsjsr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3iucuftql.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cpdveumw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3pygywmih.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ddboclwj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvverfe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrgbmhdi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxtrxmh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hjedtwsa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rjivhdac.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ddlasakb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hcycgtep.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ammlacvp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3pwrourxz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3azulljwb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wxyseuoc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3esjzfvzg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mtomujrm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jmjzyknd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3txlswlix.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jerupmxr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3obhyldol.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfudjgf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jsqguise.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lgkklntk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aasfgste.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkavjzbf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jiyuiiqs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wegeohuc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jgzppyfo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3keijvywc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgzyrmw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3inguykur.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hskjvvsk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rrrzizbq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zwqtcmqt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3tshsdvge.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3aehijyjz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qsqfaspw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ewvefvkl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tbbvjekz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdegrcql.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbtqdzhz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ajkuuofd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpbpocr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fedhtupz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qqtdgnju.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mlctnkzj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fuwjzkmx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3uwefcipp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3cydzhblp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vydmwxou.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vwrhbhhg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pznlvzjg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3lmlwzmak.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3greqwojq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krgvcibg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ebnjdffp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaiamqcx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tbspnpyi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zsuqdyhr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyalmyug.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hofwuzdi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lbuogqhh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3efkfcbcg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3nlxstlmn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gjriwbqw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xvkxthdp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dspwzwsh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3tmflpppl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hvthbuja.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rvbhycgn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3couexrfe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vuhrhgoi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3thsyasms.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ybecfrpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3naqziirh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wugrapcn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nkpfarnp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3humndbri.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeatggnh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uycuecpx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elujwajp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3arasjquh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3znrynprr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qupctvhu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tpcmzgva.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3piknyygy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lessiszd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dcdmlief.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wfofzyxp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kbsclphl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mmyrgwra.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mqtawnjo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rndqivob.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vcpoblzi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hadfkckv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mctgtgdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3foegntne.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3agitbvms.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3crnnpfjc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vzrqahki.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ogwicpfs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3otxnurpk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zrzadcez.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3epfziqbz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ukrspnmn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dewjbuyh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbhlalft.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iycxqlvs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hpnudkil.html


<!-- 参考信息 -->