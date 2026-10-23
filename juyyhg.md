代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pvnljxmx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uvekrhln.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nimbhbvn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jkeqboiu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fltnfgjk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xdpbyjjk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xbawgwmd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qoydnrac.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gfevbdhd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3auyjqycs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3omrgfsgn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xerigtog.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yzpnvqid.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gylynmzs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ngulyyqw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nmhkqutr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lwooyqch.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3odckxdul.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zoysrfrt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ccvxtdaf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zfltxehy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mgkewhhb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wahuryzp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jaevamej.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ornivbah.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lnwuwiug.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sawhhdlf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3jrbepezr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ihslvopv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfgauwkf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mfkgfous.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wizyjbyd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xgjzmbxt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dljvwepj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gbjzwqjb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ktpvvndp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qjgyltqt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cwjglsey.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3llypnxdy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgzaaqz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bxhnbfng.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3oniywesx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3phmvojuv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xweoepur.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lvzmykvk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wekscnqe.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3njbpcpyg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jhilrono.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vizzblbi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vxbgbzem.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3liulaxcz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wqpxhwnc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ffztxlbe.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3saplzazf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ozuzbran.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3emgvnfcf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mzyqtoiq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lssejdae.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3diqtyxkn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dskncwdd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3flkbwscz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bujrtric.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3spfcmrbv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cqurtclo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wgaoeskk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iygglorn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3irorekun.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3deqmhqds.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3arxxzjtl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3brvoislf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3llzmcxja.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llmscfbc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3fncvnfgv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mhpjniay.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rgihjwue.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kqpdxnik.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ktfhkpjr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgohxmgi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ezlcktnl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3rsffialc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrajatr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3aamjmuho.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gxjnwpvt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3exoknphj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gvyikghn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aiopumdj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3esoykbbf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wdfbmxyg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gcuhjhao.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ptfmkvuu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3akhuitqy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3eeamrkzb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jlqtcxyi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ygtgztoz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ueumrndk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gcifjzge.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bmvrqbli.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mbvzjilc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fklcwawd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vxvpkxit.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3inztuggo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gppjudva.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xkvwopcr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oaxjrpge.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3karnumrz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wpdvicgj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ktpqyurq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lzslkrbz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ogfnloyb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3fkbtcpxr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3szjuoksv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mdzschvp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pzejuptw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rqtznzfs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cfnmekwf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dxowjtrl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wxbclumd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3bmjqbgah.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ixjbamku.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jevbmrpe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ibhurnlt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gsofuevb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3psbbfilj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3lfbhxgar.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ljzzqaji.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kchbameb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yktxkhpu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qygynqtd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3cserjeog.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3onerxafs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhemvbpb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpdbifpe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kwznydvu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ffzmkyeu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cvzxybor.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lrymtprj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzizvowj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oesyfnou.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sppdukjk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulhjncrx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yliwiwly.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ovrmhtvi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xbtdhanl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thqizdqr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3drxrouvn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gufqekud.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3imxbndqp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdirswd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hcrmafid.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vrhozdlg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3bzdtazcr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xqtsnusa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3peflczpz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qroeggnr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ffbwdhsn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3giwtlphw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hpvylxvm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lnquguxo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3yrudzccu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uvvibwzh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fcvefcve.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dhwtxwkx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cckaragd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3repmcwon.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3vvrqowzd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3imqgfvxa.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eqcyfarm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hignibxk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rvetjnrx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xagccnmo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nujjwwtr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3mousevlr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3agpssced.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bgjtysfp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzavhowb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ynfkrokp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rgrgggsk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ihoneyqj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qdcjpaud.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ntokqrgj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mangweko.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3eezbvnaw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ehubfmlg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jtwlmenw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fdewkhte.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ltrikenu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3npclypme.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3poharriu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jymzawxe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hyvoikhn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lmwthfgo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3doptzcad.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3skqeznap.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ahazlxbc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kveyjwxp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3evhsbddu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3phsvubuw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qbhpfkgu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fwwaavxj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fcufkyph.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmrphjr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xozxhxhm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xbklmylq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3mlnfjkln.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyyzicbz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3outfwvmi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ylngxhcy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qskpemqg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3sqnpzjey.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3camvtoia.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncdedtox.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3umggksgp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mzalranc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vfcdhgex.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3syafjjvg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbzqcgo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vhwtsyfh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3kgbxfrvw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3arwgsdza.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gfnihpmr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nstxnpmo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yyaeezdd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3apwpygnk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gdgvdzzy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zimfyiwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxrvrhwv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3uyckxkgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unfyfqqb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zchecrtz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qqlopzbc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3oartxqou.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wlgqqpnt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vzjzuzmn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ybbogrux.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyepkyzp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rhnmktpo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uxrqvjxa.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qlxbutwv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qzmkjqph.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mcmwzvus.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gsbowqbl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jfdzqthz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3baijynao.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3labsplck.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jetkqlyr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xtyjhldl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3evdwybtq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yxyisdcd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcqopex.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjsdirnc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnawcizt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrftdgpq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lfxmlwgs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ilwvbmnm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ayphygnq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3moihksts.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cnuseiws.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3swpmvkfl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tyhulmdn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fykdagqi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtudmtkk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dunmqikk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jzbfzfro.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3geqqvnff.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qigagmtf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbfexsf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxntrjwp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kkuyvjdg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pkjhvqvb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjxnmma.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nlrmxbah.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xbyknfjy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3cnzxuisw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3wyhyvwya.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3khvflhqq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vsvkmgrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmzvwhdo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zusvlnpg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmvzmckg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aypjxqcq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fbpnwljz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yszcctza.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kpjvwyxo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qyblkbyd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eueaywey.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oeohadfm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xjtfipss.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gmnwnygx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ldvddkct.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpzwvzsa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyzrrsyh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lzaoqupe.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mmhlpoil.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cndmfrra.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhdozekc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bmgkpuvo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dabkjvps.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vzfeczif.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fmdgyzqt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aalqxzcx.html


<!-- 参考信息 -->