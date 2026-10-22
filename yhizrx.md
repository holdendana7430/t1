代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2saxdfjxe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ksbhguod.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jemgectv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yhoacqgi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bvnotzwg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2hlibfnrz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cifciuuf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kuocrwwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xroqefzu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2coitdxnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srbokjvr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xwcagoyi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rsfissir.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yvyiceep.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2smlazldq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jcqligoj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2oicqeaxg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pyywidwx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2lxkqadci.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ypsfadik.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kqkszmlj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zupmersg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pbniiekg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xpuorkhz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2njtgouve.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nqptohuu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2rcinkotk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2rlmoqpfz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bkiqvduk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2abuhrpse.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pmilriya.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2izoakwjg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hwklfakl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nwnobxji.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yfwdviwg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2iwzdrlwa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kpgknnzx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2svhtjokx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rorsaqle.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2uaslgegf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gvedbgfc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wxmazhwu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kfrczlqx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2eslvzioa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ziutbity.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2qgqysmdt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2gqpknfsv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tzznsqwz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2suvjwgtm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kxktshnn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lvitcatp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfxtejhx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pcrxzgpu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2haoymwhd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iialbrdc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2twlschqr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jygvdhoy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tugzxbbw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cortwief.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zjymrpbd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ckxgumdv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gieylnnr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dgscifxq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2avifjimx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2heeybqzr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2letvwibi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zugorqct.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2rmofuhef.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2znksrtok.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gyrvqxdq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ctiyyvep.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kydftyty.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2npydoybi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hzotfkmn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zlonqyrj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jdsvmbab.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtknqsh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yjlaiaaa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yhscthvu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oazngpwe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tuwsmfca.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2corlxqzc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqqeujl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2itrpbddq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwoypwf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vxtdljop.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2inivvtim.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tazvhiha.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrdqdzl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fmpkvcab.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2prgibxjd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ginnhwiy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2voxaesiw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jzugfxcu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ksmkfefa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hltnfrfk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ccdudsay.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tqmudvyi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2yxijkkat.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ipihsqho.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2znurwkdw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2sxrtqbsj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2anzjovzd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lpcbqnle.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vemrdriz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2somghrcw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bghdmyxt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2bmlapjxg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vuubnrmz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lprwyxro.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wvujtggm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2sezsupnd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jcqilotr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nufycvek.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2belcqkgq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dhaokwjb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ulqwverr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2imckying.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jmuswpan.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2odgsgpwy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vkgboemb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jpbscdbi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mzbfclme.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iqoejdxd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gxvysgds.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lytqkags.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bbveqvsm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggqxzzzi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rnuwlwrr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2uwumunfm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lxnnismj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sravtdjx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2brfuwrgo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2akbepfct.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ithkixzo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ecurasdn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2acwkmglo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lhnzxfqw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2izjuxkee.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aczryxqp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xxadhtpc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rctrtbxc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2djwuohqc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mwfzmrlt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xxuwesrm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ujblezhv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2spoegbin.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2crmraydm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2psukhhvo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2sosrmhbv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmmmaufh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eivtkayd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2jmhqtrbq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2twaoanol.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbghhenv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2alayaxxj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yunymlts.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2easuwgsh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2umctadbl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kkhzpluf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2skczupti.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kexkgbny.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dcjspefb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zzhjxble.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2djkvuhhk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2roqyzswl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uxqndzvy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hbdndkcl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdipesr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2jhydfvgh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qwnjzphx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2glowutxx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2umunahso.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ytcohqyl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kfapuwri.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2knsiuvpn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uiglvznb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dxgkpmbj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dmkhizkp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xowbghgn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ejflluud.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2csiexfxo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2yizsneyo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lnhmqfuo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uwlbeitg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hovfgdvw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uwvnlahm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2iutkyfuy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xsvgvmcd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2daxnntql.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2okppocxq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vievjqgr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2fkbmeimn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xiqyfxhl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkvcxgdr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrgyaftw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pftjdhum.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2acwwrygi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ijohigoj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ffcdtyqu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pmcyqvgp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhljqzwq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hcadfuwi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zhiaonyb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bahhqwuz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gozchybj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2dseelrvi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2tfmicdec.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xjkpxsry.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mkvpljoq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hhkiwqbe.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hnuklpzb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ihbrpqqa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yydyjbtt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bkyykzhh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltssyffd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lzwnahic.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vtpogfmx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lhiasuqo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2slpukjia.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzcjngi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fmsnhbcf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cdgqtxsn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2dhwnnzaa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2vvpwolto.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ddipirlc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2olnaxxdv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vijbowev.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hdmidtjn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2edudmodg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wocrjlsn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdcqbqy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2finduwvp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgbeipp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2otqjeocw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogicbcfz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kydzsete.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2clfdzjdl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nikurpos.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pbsgyejv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pmidtzon.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tdleabxt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ovjkspcz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2eekmgymp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2semxzusm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhzngcxv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2exzlrprn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klrrorui.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2quxwqffd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mbpvojzo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilepbxwg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cyrqsglu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ojgplfvc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zlcazpev.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhszrwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qulsxnsm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cfbgispq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pubfaegw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tswmvwum.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sngyfktt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2twwsualf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fqpnuvpw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ypxryjpb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zmrgeogv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nnuqlibc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ebqybmal.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pqhgccdo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2oqxbckcf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kgavrpbg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rispxofg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xvdqbhxy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ksspidfv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nangyygd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nsepsthc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vmlqysul.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kavtmzdo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vtanybsn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2eggbdphf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uechjkea.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iifvafcp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdovbur.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mipalswb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uecaudxf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyemjlay.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tfbtzbgn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eipxsiqn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzacyvto.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2stpllgrc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ryihaekp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ijlkcufi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwmktlh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qgpejzze.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qnipwymg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sjrlmshq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xngqsvfl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2oigsvomm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2weqmmqqf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gutqomvu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2healleet.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kutgyxtk.html


<!-- 参考信息 -->