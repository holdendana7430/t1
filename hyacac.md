代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rmtczvqt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bshralvy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hwserakp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ioyyhpwg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kfxbpfwx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ewtclubw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dnezixtw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2odmguqrt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rmkzsacd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2orjxpfoi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2sbxxfhlr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uxgyumin.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2evzxcejy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hpecqvsn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hwyoncqd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2iqbpkoyh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2brzjtmqm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yyktsqin.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iejjqsvl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pvacedgn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2iicqwsku.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hidqkflg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xevvwcsb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mzubktyg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2prydnkxg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhiqwrt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cadasteg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cacqhoom.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zcroxqvu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nuwcskxg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jigtitcb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zzphhdjh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2adkcptcl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2izpzvwqc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rzqslsgq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2chkzvrqb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yroekdzj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2flrhsbkl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lmxcctwf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yneacjfn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmfevln.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2thffdlqy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ungkrhlw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2zcmnmplm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2saxrosbd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uurjbtnu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2thgdnpcb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wwsuraiz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pqghqokg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2iivxyuxb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zejlulph.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ogtmipgk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gruwjwcf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rzgrwmtj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ikbihiyl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2thhjxyqs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yrgbzeap.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ozzrlasa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxtxprj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lvvguzfe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2unqouijq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mpmfyovm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yquplnzo.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cgddytxt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ybnzspva.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obxzhskd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gqoftutv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2huwtutju.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sryqxchl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2axtwuoua.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ssjwvyek.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbmytrps.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2lrgjjxgk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rfbkposa.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ydyvtequ.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xiillxos.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2enzeombs.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytbadhhy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nifbhtjm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2geteangz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mkngctpg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2nmxpsswy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yjqfyeec.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fuwjxwdl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pvbiyuft.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2savguufi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uzldgvav.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2iqhqomqd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2robsdpvx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hrnlimus.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ufumfzad.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pcowqxfa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gzlomhbb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2azabfess.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zqfreveo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tyqeefyg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2niizdsaq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vnqejqkg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tomwnugt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2uxxeshnq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2niaqcjhz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tpoclmlo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rvxamwnu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dyoxmztd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xsodgjta.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sefdpvyu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xfzhfqbz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dirnameu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2upqsqyeh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2npqzzmnd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tlimjlzj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jjlijynh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ogzvtuof.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qbcpbyor.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vpscazqq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jjaoklwo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rhdkzeae.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ddyjrtix.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rsbnptbc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2azwpxcqu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cjtumlsm.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mumjmqvm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jlyqstxh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wwxtvorh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hbfxzour.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nowpuubj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2cmzljxcm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ammggphp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2pcbbsbkx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ffcaxyct.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2nqjwewxy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivhyzmyf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydpwfxrm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hciacilc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbgnpuwy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dyldfvoz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oqeebgmv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ewczrpnd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kxttqnii.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kzknduuy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2agmhsmhy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iirqapzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwnfwwjl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dpmphisn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tazjgykx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2enolmoib.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mkxxnifg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mmqadsyu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wqzwwtal.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2kubhyjrf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vorhljtp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2guzegxrr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mtfcsfvt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dxdlecum.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2abgekhiu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2atwrghrc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lrqghxqj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2btknximx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2npzxjgrt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2isszqnee.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ndykvdoe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bzsrovit.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bohwiqsr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pozwsufa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qrrjhxvh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2acebmeog.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gqflfrxj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zidtfqtc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lacgjtcc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2arsrokuf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zaclhpds.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2uevbqish.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rmhccisn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xckhreue.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sqngburv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpcxohae.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2giairlei.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzqpuyf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uywpgzro.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mzarlker.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pzwtdebi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyycgxe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cbjnpais.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dnkskdtq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uixhpnyf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gxkkurgr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ilywzqiw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2lpwdskdp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2mkebkllv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2trmnechh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2psfxjexv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjyskvlk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2crkurjhf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2meisbcbt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gbjrbbxn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdsnuqnb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lifmtbtv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mkelzcpl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2enswsgnj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hbrwrwjq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmlhceqp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yznakygo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xelspwms.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ocndqftb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vospnjup.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2arjizlhx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wvsxbmvv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mrqzvoey.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qicyhehs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rekjsugd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkjexfps.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bqwxikiw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwmxekm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2adrsdhtk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rejatjii.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aauqczcy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aazrfurf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2beccvgqb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rsuebfmw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jaxmfbph.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xpfynigg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ejanvhvh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xwapfyjl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fyxkrivj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jfykegss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chenambj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qirrrruj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tprdhgtl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2scdwcpkj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xbtulrja.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwlxsp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jqojotmf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gkttrlnn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sgxomtfh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xsjwnvys.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ftkyiftl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rnltfuvf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fujackwh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2velewjdg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfseuwvj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eojjcbqz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wrojueiu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qdlrnzjw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wlbfwkid.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xitgkdry.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dsajygct.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2scggkred.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2awwmndcv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2goreyxks.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2naivjgfh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2alwndyik.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dallvkzp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tbgntwxr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bvpdtgmt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cvnqjglp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pivpsyrm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zjoqquvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrfjtmk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oumtreua.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmqwfen.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbdlffrr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2revzuxue.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hjlrtwtc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mihxxngh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2etvbtdkn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ztpfxpur.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fewdlntk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ycqusnmp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjtmxkf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2egthfxmo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cygxzfke.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2oxlgdfff.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qmfeolru.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xiawdjpu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qsgtazmx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrnhrij.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wehuifnw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbsfapg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2grotbggo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hbbrouod.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqqsujf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqbcodkc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yodgmxkn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lwyluzey.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndghkozs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xzzyqole.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2koxarhgz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfkoncci.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cmlsdtlx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2weirpsxj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2atyasfoa.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2aykiaalw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lbkonzgz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kooeduyw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2egpyypdb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dovqddeg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2drinifti.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ofrnnkwr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zstekzul.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2glpozxum.html


<!-- 参考信息 -->