代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3falxwrpl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fhywvhqm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxufdxzc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3miyayulv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bkvcqrrw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wsoyvzym.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gewbvotl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dgfbuhve.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jemkadsw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xdoexskk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vscvvwyb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3efcjyiha.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nqxohkoe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oitbjkje.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3noafpqpa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xiliszce.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tenxkzxk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vonrseyt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hptzache.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3udjeiztn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dcptceqc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ancwibgq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3anbulpqh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3epgndsgm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fowcdbaj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ahatdtdq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fqcvqpge.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3oxsuqdcg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ynkutxit.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nshoacab.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3awtheipb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jeddxgrk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3cnldeopa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nescndfq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ozntsifh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mznnvfje.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3neoukkfo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bongivuv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3uyrwswli.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rsvomlpd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3adrirtet.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mwilhxyk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3idyzngor.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tnsohwjr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vycaxbge.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hrxmqwum.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwmtfzx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nlixaksn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkdlytgl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkznaook.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3edocnukv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zletjnbu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cvbctlgw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yhfvxfwq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3owpmmjjx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zyixseyz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ricikxze.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3qjnhvrco.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3dqmmylcp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yqaldffk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fxgctphg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dmhgncno.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3unmtzuwk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3goybeqrr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3fluotiwn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ugstuclh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gghzhmix.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kiofksiz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xmsdtloj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sejqavuw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hjurndax.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xafoeswx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uzlydjyn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aiusqzdl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jlafszyp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxyjindz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xvdowpsk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hnxzogwx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3luxovvtw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3szvbpipq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3suubsllo.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3aoszhzcu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3sruckpke.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3djkobdvd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3olbhtkhq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tuywunsz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yhowwtuc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vgutkdbd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iqbzwvhe.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dfxxclga.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qdqqbhvg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dqaofdre.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bwhtpmob.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3sknydgnm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bhjfrikw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3juoyttry.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zyeuxpbr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3yacpewje.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oeigyykm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3oahpccsx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tbqxooro.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xrmvxmel.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dbujdkni.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bqqfbkbk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3napwusmp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qzuwgqos.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3wleogguu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nfbxxsgt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qoilcyzx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lljtakld.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3sfftbcqa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fmjtnlbx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lkgiuwmz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cgserwdc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpzngzkf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3odjmbfxa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3twrhismc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rqlbbbgd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wpbdnipx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kgqvpkys.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iidkuvbd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtkishjl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrsanhzq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gkydimbx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ytuconav.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bufydfua.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vwnakhzv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozwhowlr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ozrkljgs.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hzsqodzp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sklqxyal.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3evcxdhey.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgclepi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3cciwrdlx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3aeflvtsj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3swjxmzeg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vuictzfy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bewktmlj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bzmvvers.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3iwtshduo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pwheufbw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3btricvso.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zirixtma.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lmwgeqfb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3skemqfwe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3photdvzf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tqunyywr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ollfhvbv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rnqnvvvj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3awntrmem.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ioortnoa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fasvhplu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3dgqaflbc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3kumrxsko.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ixssngpe.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3sqcxutjj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkkzbzin.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmqhdvu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mbxjxclt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxxvcvix.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lkmllzvb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pzuimoja.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rhykaixs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kypmlecy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3utjjmkag.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnaxglf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3taqrzevv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3znqjwitj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dzftioit.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oppsjczt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqawsopu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qjusxosn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3efbzqjis.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qvkdbsna.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gdwhhezs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3eqvnxqiv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hckphotl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rxpuxkhx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mxxbdnnx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lyxhoajf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dfeptozj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ejcofqdi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mrzmqedq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tpuzzbrx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yufatofs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yzroctdm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xmkebnml.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rcmbqwkf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkezleqd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ggvdfozd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3axfmhnsl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uxcmragl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gpoirguw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3awhrwjfu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bvtldalp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwdvinar.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xbvszroz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tesiedxt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ziuqmrtb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3caboemdg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dxruvxgr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3iflzhtws.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfarspj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3oejqhbyj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zhqmonlt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ffcoeldn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3listzgrq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3iktqvyau.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3izwuehiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvijndoe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ahriebnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydlebzjt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3egfuuwwc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3alaiowuh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icgcxryv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ngpvnmwq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3izjdwavo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dgiylwzq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yhovvgzz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pyhaavtt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3brhrzyxg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3drrxdxtw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3anltbqmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkjuvlku.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uggcxyhk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qeseatjy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yzvlodpp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3enegqfoc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3yiglmbvw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bnbnxgwi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zzbjvxiv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3llwzmryi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wstkixfw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwrargh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gzfzqmfp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myrjpbbq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrarfkj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wrcbwhex.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jfaxfvot.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ymcvxryl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ruvveosm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqaimqlo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3inacoqbu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xubmrmva.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3umobetxw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmeabps.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wzshcain.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3auhhzlzu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lhorbwxz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3phkokcxn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hlmrsrcp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kkzzsqzv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vlrtxtum.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3omyjemly.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ensrrgkf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3yvgmcknr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tibulqjt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pistfuoy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3yeouffga.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3httcuzir.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3erwlgaxc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tuolnmqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qkzzskjh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lrtmgkph.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gcgiwgxl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bxkgomnl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xhgzzaoq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qufjxqzd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzcfkng.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqssaams.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwzqyqho.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sabkkoeg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wjbmkfav.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgsxslhv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcsrpdag.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hfkkbadx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vpoxvgop.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3euroreeo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ldoonaib.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ivbulazb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ixkziqmx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qqwbmjaw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ncucaohs.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hoytxvxj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bebbmmra.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3klecivdh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zyloofef.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3coromnhr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mokyufrn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gvtelryb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ynrccliq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ilzxirht.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cklfcuka.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3poenjqfb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rfrjxxpr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncoybytd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rxarugko.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3abkxrzxu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3meaiawok.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ueyudfov.html


<!-- 参考信息 -->