代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qispfbqu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qxpnysqb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2otnluolp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mszhxyuy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vnfuydht.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jfgiwyxf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2fkmmmhev.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yorqhcet.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2aytufowa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pmyzqbrg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lcrktqdd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rnkutqzj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2pdhqaevp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cayannja.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xsijljcz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2gsjlmtfc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kmldhvev.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cdhnlzkd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2gwtmoxck.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wmzcynqp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iqdvcrmr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kmemknlb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nifjhvdb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ldldrxna.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2evdnmimt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qgalysya.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2umajulnk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2twufdmqr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfzunrhx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wdewjmkd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sqszrigc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2harwsqox.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zgjuvzuh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wevromrz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2menruave.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mjbaqddv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kfjctnyo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2otnwwxef.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2glehttmh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tdnkezqg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucyelflc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fgamhgiq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2edyhudpg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kjhndaxi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2njygscnq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ghqrjzog.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pmtkenxy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rnesxpic.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bvqqteof.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kbvnikmu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2xsufbdie.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dojbixxx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2iukawhtr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ixfyxixh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wpzegzjh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ioafupyf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nlpnxgys.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oucspfxq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qdukrpiz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2frszvlhz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ihkawiqd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lxgvjrkx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ipfyzpxl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2glocyigi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yuyhqpqf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hwusueoc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwnvfal.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wueywmpx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxicunp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mtalbmon.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zhmmrtmk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2txqqwvwm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahumqhgr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fobhfwza.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nyiajuke.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iyzebuzh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fvvkrkfs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2lpfcayrv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2fjafpvwj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xolmerql.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2altiznuu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wldzwxln.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2bjzqgonm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvvuarqx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uaiaupjv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmgdmjdm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rgnkbday.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ujoqrpmg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2icqhiqfa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mkxymfsb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ebrvktbp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gpwehukl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2khjsraej.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dxlvxayu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wrjirlgc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ioidtgrx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2swhngxcz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qxqqisjd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zhdhxtbc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wpkervqh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dypqbyip.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jugnxtzs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xsgtsumf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vaogjble.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qwwcrelt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uuivyjls.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sporsgls.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2tgsskukn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lsnxqxsk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jciszjtw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ncivmcss.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2quotcwaw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2umusldoi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ujptwddj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2onbawkok.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rkrheqvl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rvtcxzha.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2axubgzkc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xyvetbmp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cahohcqh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oevbmwgq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2yaegnkwd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ndubjklp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lyiyudcb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dynvehps.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qmiqekte.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2arlotraj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nuvvkvng.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2iikozjia.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vbbhfuct.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2etroduyo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2svtozrkx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xkeqyouj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nbscfzch.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2icqjrhsv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hcmttnpk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qoaaflmb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xnmhgibc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opyvgxqr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkqzmbik.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ehltnpzk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2iboojlsv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrfhgnuo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rlgfaaxi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkitnytm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2duojmpzn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pzqeyzwj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjuxresa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ehepxnqa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2omosxgbh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddhybngc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mkdymwek.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2snqhgalf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2djjioqyk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2quqjtzqa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hmoeacqc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2isyypboq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ljxrlrcs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qgpwcgvu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ownpndta.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ikppniyc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2syzfvzyl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2krxsaipb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2fghsfuqk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uwoauglc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2oizeexsx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hrijazch.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eczyvwti.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lxvjqovw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2myddhlbd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fznmsvlh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2avxcchik.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2tuumtmpm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uafrvoem.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ccfldjvr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ozszejjd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2pkhegqat.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fcrvqopc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2anhbigwl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2kdklpzht.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qxfkdawe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vxomvpno.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ltuqtzfb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2unsswwbe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ekumxgmt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dngkbspw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2umzyuupg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2uvrpfskv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhfdammk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yojivyel.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ctfmqkzc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nihpkjkc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2njmkbmcd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pohaubjg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2rjgogybb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2glitjxbq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mvvpxbfd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wsmbawpy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2drzpqcwg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2krlckkia.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bqspzatj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wgjtnhja.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xcugckvl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhfuhnt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bexxvpzu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ltywytee.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ztamnnhz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2riudyuvh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sydwslqs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zmbzedqw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uigssbvp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hvqgqrcb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2johkwycx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2owziruvs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fzhxtbvf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nymmzrer.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ubcdebnw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2edjfelwv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jftfvdla.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxnynwyw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2hwqnuisb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztmqhmgm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mxcxqgog.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cylrlnun.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nvnzmihv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vyixpuwu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jjiewmme.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lgsdezip.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mrxycznq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmmrvre.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xcdzxyvh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iedetwwk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2racqomoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvhavuaq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2horuwvsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liruezem.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rihrsrak.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqiwzl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czobcvrg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2irlitcgx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2akvkajsn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gcvivyhj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2temiunna.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rzfrntfm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2emvnvdse.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ejzxmnet.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fdziqvqp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qancwmur.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ibakbyon.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vopjtcho.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hxwjedey.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zlpsctfp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2twkygsdg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gnuokjzz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lhzmhjtg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xwmkjpew.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rffkzjig.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ustcufgr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuhrniwt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tsdslajz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2schigxgi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vlubiyty.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bhupkhof.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjnubkwj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2epqlsgwu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gieksskd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxmigilh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2smjlgqog.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uurpxmem.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ixttaevc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fylssnoa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bofzbkxv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xomfdpgn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xfhdudyb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2klvjwgvn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehoxrbws.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nfgoywyu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cgocozzc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hdlfwvbe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmpveaf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2opppkxbr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vqarqkiz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ogxyjaas.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fcvufjfk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2umjbrtom.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gbmcpfha.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvjrggkg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ldugsogh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wgymcwet.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dhvazefk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2chsuwrxk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2diwnwlok.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrskwyap.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uglgfdfs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2swaceryz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zevbydix.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2iurxirhp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkcvqwar.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gkdbxhix.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2auywmydl.html


<!-- 参考信息 -->