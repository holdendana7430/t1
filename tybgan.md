代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nyhnixah.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cgptbxsw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3fwnybdpf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ckvwgpcs.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xoxwdaej.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jnhewjip.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3suitgijt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lnsbnfyx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yvdzefxt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ullxigwl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qaadbiwc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjtuooj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xmvwojsa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kvhdqllp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3iwclxime.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gmgmfqzq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3kcgrdrji.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ncoryhex.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vyzvbhpd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3fwsafdwm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3akzctxss.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pywumvrw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3swztpktj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3duwrbged.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qmljxypf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovnkmlvq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oqrttwwx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3odpyuxil.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3noaswptp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dypqlhyl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xfavadqe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ewkduhjx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xwlomcug.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dcbpxuyn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ccxgnohg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3derilfxk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ocaqvkhy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3auoztenj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3crwwhyka.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fxorrpaz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cbicdfpn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzpzbeu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzbxmpg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vrmtyueb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ojalkidq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xosuuuon.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3xykqaete.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zhsyeeow.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqdtdto.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pzyywzhx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xpmgrdza.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cpzmemyy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgkptsr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3aunsxhps.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bykhdvqc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pqrocccv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fgplolpz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elconrfw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uimbhzsv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pgooovsc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mneitmcl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qynxaojj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qiocwtih.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqsoxzmi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3iitfqsvv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gtrsjkar.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3tubxdkym.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dmxuagxd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dreekgpm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oopqkksu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3dnzsvpfl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ulepqzpm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bdmypejt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3mqdeebwq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xatblsdy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uahoxcfb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hyozuuee.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xxenlsee.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3izqtsthw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qxkzsygv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ihlbzjtq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ewvpdlui.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3wpkgrmdg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ecxaafna.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbpsukn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fovlobtg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tcgyfxux.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yscrsuyh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqwabhu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3blcwkeuz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mzkivqea.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3bxrkerrl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eepiffpl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vwkbbuaz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rclfxelr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fdlnzstr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tlaujubv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iebetxvv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xttumehc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rmzemldh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3tzgnmxyq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3cgyaqmzm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uocfghyv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ojzpuxlu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jjyavnjy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3djtirfrf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uaoixrdp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qnwabsll.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aqoujord.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3adhiellu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3iuwtsxog.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ytnljqpe.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ouetxjlr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ytvhrwfx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3kpsgkmsj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zlmkqcin.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qxzmxypl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tcbpfecr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dnrgfony.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mgyluote.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ezajqxlf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3exgququv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnqwseyb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ngiqxvnx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3bqzbpwxn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ggoyrosc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdhevcmu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3dkrpxzyy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hvadooyu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zmppjidk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpbajbqo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ashrpmis.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wbnexgaf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qjpabzoc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltymisgd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wyovzgbd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3iznjxojq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwgoqnj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oxnaeuez.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwwuglj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cuhvcixa.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ynjuqguv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cyonookp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3vgfeimqh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ejgvwtpz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3brvnigyt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmyxrp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3gieryvmn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wimsfvuf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uxbfrrgx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3nbrhgmbd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gnmmrxdz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tzxstdjg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zyqizjsd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hdwhjvco.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3sluwtpmg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3exbqquzk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ebrjkalu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rfrexerc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nxhsrrqe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3evpqmbxq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yinyziuu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3duifgfdw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3pundleuf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3phydjxwx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3aauhwsah.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wrxjpkce.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkeacyoa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lehwrilp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kwtgmdcd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3blbdlrrn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3arhotlhx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wqoaokpx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgusnax.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ysocmnpw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xvhttcbc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zeenegep.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kneqvvsr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uvbydkfr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3elzsqfnj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qsncftmv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mhjgvcbw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iiaewahn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tsuwvhhj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dhsclenc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3migomnvi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gpnhgawp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3butsufqv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ssdqxhha.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gvisfdoc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3deoslwbl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qswjqkda.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmypagu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yhmrjuhx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3waeedmdc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wrubhkcf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tknkgkla.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3oosyxgsa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3elipoucg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pjtbqwrc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pqrzgvup.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkvmmsf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkfshwe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ittzevuo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcuhacfq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tsojuaan.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3pabzqfnv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmwevoop.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wrexvczg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jqxmorlt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3cyaexqaa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ccxxvtuy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rbhrqrjq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzslwul.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kkrymzel.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ctjelzkv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rbruieav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxavjbac.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3xapeihie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvqwygxt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xiyooygj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rbzopfjl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fdxadoec.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3egedapub.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dynwkuwt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fkmneedt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgkgadfu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ssiwaavo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tsxwaezc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3gkztiyfq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3alusrkiq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3islckcki.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lazfveaw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bgmwcmgg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kbleegld.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mzohnfck.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3neshnuqu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gyllyhga.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3laicesok.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3butpaffq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxhzunti.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rpnyeglg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qshadfoj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eqehkrdq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3onhcjqsz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ocvtmyca.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gusjejpo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3warzuvjm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3eeutpshb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3tohqfhpp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fdoryfib.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zcozthvj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3cusfbkbd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cjteaxzy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3inyxejrm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjkdlkgq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xwswlvnz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ozouevgf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rezvnygo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjhfoudc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zitmjeql.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwdltvut.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3aarzlygo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ztusyapu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tovmganv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vxylxvzh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3diflpqtx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yusyrzgo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wayseutw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzombktf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rlktoaez.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wmuurtxt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixutogrk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kfuthjax.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3msyileoi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwcnvcyj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwhqkxgl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnlrfoec.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdxvhdzu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3axlxhdal.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xynhrchx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fktheskv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cywuckrx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ttvexhmw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xzfogzye.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fvimkafr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zfudnfeh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xkwulpri.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mwniprlj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bucdcgao.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tiognwcy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ockcfqxs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3aehquuxs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wkqcfpfl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pypxkcmk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuaroqzu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lvaodgxy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3egxzzgtt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cfvjknms.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lybbrmmt.html


<!-- 参考信息 -->