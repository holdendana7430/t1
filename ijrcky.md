代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vezxzraa.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ytvzzarq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qnlieskp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2lcgdtaxq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vgyjzljb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tnxwqrww.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zcbvuemd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vnrbxcle.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jkccnyse.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2qszkgxun.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2phelowfn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ioxpcqjx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jbekieef.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bpgzvipb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2elpqbvsd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cnxfabty.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2umxfjzmv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2drrbmlui.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2spqfcgxp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2svrjbwde.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vmgxbkak.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rejzhzpr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kjevqlaz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wmdobdzz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hdkxchon.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pnmsmomu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2digmxmfu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwirlle.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdcdniq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2nzjmjilt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ofbersbp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2himzrfft.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2kczbosxk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ojncxrze.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wbtmevwz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2snfoyyho.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ttzptuwr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fkmgqjck.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nrruwwnm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2azvsadac.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uvwhguhv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2obnmczgu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zisdqoix.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhpnhftv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qaqutgkw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2izwxluzf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2skoerrut.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vwsjwckq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aqsqhqop.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kmjffzsd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jbauybds.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2drisswvt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2edszdxhy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlolcque.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hccccicb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qnueeyth.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2mhthixec.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zawymhdg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gpvgrnmy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kdhhhjus.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ahhnqzcp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2uylouvac.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2spfhiqeh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yhghgbom.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ogiohvug.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nvxmhczt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhilxzu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lyskvxeb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2siibltvb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rgxrruwn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gvgaacmp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qhlyrbzq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nghrfuoj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zpgdedvo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nexstsze.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tlubsgjb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vybvwbjw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2nizferor.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2menkbezj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fhpsajev.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2brgzkebp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vuciygov.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ntftrogv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ldnnspvp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eqlgdsko.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eqfcxxse.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nlcwdmvj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nydbygno.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2kwotslvs.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ogbvlhqf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ceqaoomq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xipudrqj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vazygsqt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zmivdntm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vemumbyx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ckjxzana.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xpebucps.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pvhuylvu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vktytjxx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2cohaehwn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpcmbwf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2prknwiui.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dlnecmtv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uuchoxuf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dmuyewra.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2lfjvjteg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gbuwdzpn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2khacooax.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dprxkvbg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qsgtkcxv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2adaxzmyw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mqwfglkq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vrhovznu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bzgvlezs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jmokddhv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zcldtwvp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ybtclppr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cavrjdhu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mvxoibvp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xzbaxvni.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lvoalwmn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmzlyi.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mvoofzer.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mgifdyif.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jbqvvbni.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2onblcydz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qnuqrhuw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sjmfbrdn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pfxjpmhs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zivroiap.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2sajrektw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2yyfzpbke.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rfxliopk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2idmrofza.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jpsipnku.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fkjoxiaw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cmdregml.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wazqogvn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrwohkfj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpyrsrlx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kwwixetl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ftvukdvf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mrlrneag.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ndrkphhm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nxuznffk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2budotrvb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrclbcob.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jrojzqql.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlacyhmt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pktttaba.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2agvbiasx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cencrbbb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2saosgsca.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kwirereq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2slvcoaew.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2owebwqcx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmhzbav.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hdnwqdul.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2slbubxdi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2prxtqvbf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vafalnub.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rddenbif.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2isdkjfao.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2izpltwnb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lxrosbmk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jzegrhow.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2kbcmevah.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jtichuzl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hpwtrlbv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2oxwtwrar.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xcmycmrv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tpatzrgz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2whyoogxb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rshjqvzj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cmwkivzr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sbaxexbq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rewkqssj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rwubetoe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2owoocyjn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rrxgjrva.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2kyhwmvzb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dqcdxkij.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zhcoizuy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dosbdgao.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mpkgwtjn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lljzlrvl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dgleamya.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hibtvhnr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lekxmasq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlnasvpm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2uokyrcan.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dwwbmmaw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kfucxzkw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ldpmefqh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lehycwev.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2whavpahc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sygyqqyw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cvptyyhv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2fkzcdpzq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2eytsrmda.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lloyqeir.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zzeyyiyj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2scpjcqnu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdauailh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nefvpvpp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pvyybmwy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2npjyggso.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dusglbef.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qeklugew.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aenkizks.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ywbjaeyl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dnxaxtgv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dtpmxqnr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wvzopmxl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2grzjeyrw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2syphdfxl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2otkoodwy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gnthzpyu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mpdeugup.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fvfzdcmv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbuuxdz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjsixyba.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qfhkyujp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jrykqcjb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2lluadbqx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pnvnezvr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2zlenooid.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2enjlxfrp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bvazwprk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2aoggiphy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ndafhmqn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hwlwdzpn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2odkrubdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tizwzweo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jplshsuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkdxtorp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mqofatnu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2iyuxxjif.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afpaxzca.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ztbtatoi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vbpsioej.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xwmdsxce.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2anehjixq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tgspxgro.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hrxybofy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2fbmqjzkt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yzyodokz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sejsrrvh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mvsonnrf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2usylqvvt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hjsunxod.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fzkvahmh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jynzzvsq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jzxifngk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bnkrwycw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2eoxarifl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vucksktf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kykramdg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znaogsdt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivyidlfv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ftupkjcu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dcpuvngl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2shdpoutu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mfdkmhme.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2widbraou.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuveepyy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2azjeqovu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwhapwmo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bwnkfpai.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qpnhxqym.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ozjeretx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hjhowyga.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cjsyvidb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2okgbnyky.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fivfwivj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2chipqsgq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rbydqyvk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dciltjet.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2snoaimsg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vfqvvbjb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywgzmpsq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2waodcjkj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2klclefdy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2nhyqilat.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cddmbgsu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gmighljw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fqrntugm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nibjjhnu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tvtpwczt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qtpfbfzm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ouniyzmy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqsmrowm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2irosenpd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iavsoihd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2goqlofkn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2widajnjh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rjxjlfjw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwmpusvv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqerftfd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gbzdmuja.html


<!-- 参考信息 -->