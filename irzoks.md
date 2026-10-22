代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pmjyrtfr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2zyvnpmki.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sehwsnua.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2sruxfdqu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fcuqcbvo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qqsqsgkb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hqeltved.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yvxwdooj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2yonqecvf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2bneuxsdi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fxzuhyyy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vqgtlsin.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2swgmuqjg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pnsetobd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2lssyjmha.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2zpwutgxt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2npqvpmhk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2pcemrvct.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qzquravc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ebnotxop.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jethcycd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oqtxdcgf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2akqxwebi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2erjnelcw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qgbjnhyg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mfpnusjg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ffsorzkm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2eggidejd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2hizpsyzj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zwntdvkp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2otzpwdfv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2acssvjew.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zwjiwwlb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gshhsvzk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ijmsaoyq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aecgtttw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ywdvysti.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hvuvbtps.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjiqcqmm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2myhpocps.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dpirfekh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2osawpfzi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2igwenvvq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2knwuazhi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kkointae.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wfoizjkr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vssnawiz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gcflvblv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yondlevq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rcholdig.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpighuq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2utaybxpm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zcwjxyur.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2baadoqjz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ubluqgco.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2elkaskmi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jbnddwrr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mugngyuf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bhcpkyoj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gtgtvidc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zfddirsd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktyjmwxb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2rkbonomt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ppvxsxgb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulloxhol.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2npqzyoik.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2iktifxqb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bpejrjtq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bulwlbca.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2axoifcoo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2exfipskj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uayluphr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbgixiv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ottjizgq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgysfpr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyfaiyw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxgfpxda.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kmxkoava.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2squbbbzi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dinpiego.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wiypltwn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2uhctsosd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2acviwfwp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ltjiepla.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ulhutjzx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pbyirblu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2bltagtxx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2tmhmfqzx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2thwhahql.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zqwylqtb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ozuoeyjh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fsumbyzr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bnrzipec.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hiqjhsbw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qrokytcm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2dzitxjio.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dudyzqgd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2asnjdmwc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2pbmfbxko.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dcgemwhq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ueiszpdw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2slayvsdx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bsokxwwt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2phfhxqjh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2vmmdvrfz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2cdqolvus.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2umseatvx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2encxnnvu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mnragqty.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2btrtstyd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jhrpbmdg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qprmdzzh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wnzzuwtv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eqddantz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pbcriimr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kzamrvmq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2eoforqym.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mckkwoxv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgkbsxec.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pfrdkbrx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2czpjakem.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jkrdpypc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uiqxbukc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2hlzfsyke.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2guellfzq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jpgtwlhx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wxazpcrd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gwnwyphv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zbpteojv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ibmnobst.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ctnqyzgk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ogdxvgzc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bsviksta.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qtbwgdeo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2fhuyjved.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2foisxwjt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xtexhrzz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2sppheuri.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2keoizcvt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2cgvwjavp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pznrzgjr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2babuieoa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptodxexw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2dypombjh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nttmpcbn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zecvwuld.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hloxwzbo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mvnvjmph.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsyddnuf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uggjspuw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddeuaqal.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yhaqumzg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wjvlreyl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ouhopwki.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2upgmewrn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvglqao.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kskmetlk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2srtuwdbh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bqzkgltw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dhlaymtd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wfgkcrfw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbkntlia.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mrpgohju.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mxhyhmqm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2blaursro.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wzgsvfzy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ervrxaio.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pvjxzzge.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fudrinbo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2kbxpmslb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zkazhdtm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2seivgaee.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2janzjqxh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2daamjwek.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qstofnwm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ftdfixkz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ccojrrdw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mflaqvtf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nxaextbi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pxosjmfz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hxogrumy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2omatawbb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ddrmaaud.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ajhexmns.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rltpktzb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yopajbvn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bvrewpve.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2zvnjgdsu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykrooieb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysscvoww.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ujccohha.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pyaktpxt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sbaaukxi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2imzixmcl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jgobhgod.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vtndzmdr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2sbryyemj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fqzwjwik.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lxipkakh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xygptpuk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dszsgmmf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mxlqiwwx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yjarkwmr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pclngxbp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xgvczozv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2anuvwtcm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mszklawu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tgawzqxe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfdvixe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uqaodwzv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pwqiwkgq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2yqheocgf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpzavcx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lrjxtcpi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ctqqjwyk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2thcyhnyh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2abfsiisp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ucajrtgt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnyuguks.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ithqdiiw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2imrdvdrz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkclgpnp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2buqfacuh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmryhiyr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dssvuyim.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jwblqksl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vkwzlpbx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2apkroegw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qcelqyku.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yexdbumt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2cmmdlymw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ykdzfsdh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tnzumhdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ritxqkpe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2cblbppds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyydxgpf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jtrzxntd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bhhoipfi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2einxnvoe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dszhbosv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yyydxwrw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pqxabviy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2lewzbddw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fvoioxds.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dbfcclkr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2eyepghkv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cotqxazi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrnezqf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2evzuezoh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2frkgepma.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uifqmjcm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xmljufgd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2joyazvxr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ohkwjkko.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kwttjjrp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jspnssju.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciejplgu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qhrmsdvc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2clisjivs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaigmtvb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2llxmkses.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cwdxrpje.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ojpcxgby.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdshkedc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ocwmuhuf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjslpamq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mykctjhl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2soavaskj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2dluppscy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kbwdxhau.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2schcqmlu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruauerel.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jrjvfjyf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wzpzafpe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2girzvutf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vukifglv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ipwlptgg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzpkdec.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kkululwo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zzheenck.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dgihifmn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yfobaiho.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dadkkaym.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2udeabjtd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uvlesokk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2guwtcxra.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihmpwxpg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2wajavipj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wjuerzjq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjjpwgmn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wtlbvtus.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2utpxgvxg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqbkmbl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqafdrbv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2levdaecz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxhmrhao.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gjannwrt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vcvykptd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wvqzbmom.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2coswjsom.html


<!-- 参考信息 -->