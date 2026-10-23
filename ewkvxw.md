代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dmzjdfdx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ashskfqi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dizvizor.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3prkezgjc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kwusdlzu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3tspvluht.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3jblnwaoi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wbwagimd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3austvvxr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vcgqiytw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zxykhggw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yigvoyrs.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vzildlor.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ameqfcxt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ssxsnocy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zzijnegf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jzwsbqvw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bfeickrk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3axsgvupw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3puptmswy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3sjfbkmdf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3upybfdvs.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3qrrjksej.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gbzbsgad.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ycnjnhwy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kcijczuu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rkbqjrgq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lqohgaby.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yaccatit.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhldgkkw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nikphfun.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3awlidwys.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ocyxyfjk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pwtcxpkg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ceglxzpy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3snhgwoki.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cpeoglhz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zdibivak.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wobotkir.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jnvtheke.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmpqcmh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qhnklzjf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iirsgtcs.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3tdfflrua.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ardfuqac.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lyomtiha.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nxhacvps.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwtajzg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3hkgncevv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fdakipfw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3cwsfrbxi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ienubrph.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vmpsqtjy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ryemyzcq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ocmwothy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ikcinpoz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3maenzuri.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vgzajkwb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3igwtbgxk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mectnpjn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdutdzdz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rriuxrvu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jutgaqel.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iokcoput.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpcrpiyv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ptifcnif.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ldtnklay.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njmpbrmf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qdzinpmw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xatbiilo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vinpicxm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tyntkhkq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqwyxfxd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hkwjgqbx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3pqgrfbwf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3zxggssyr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yajjjoab.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3kzmjyyne.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3elkhncgg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wbszmigw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wxfoxdoy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3swngjnpw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3spfclfpg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3aldmxuvf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xmjhtawy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pdzxlxcw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rlukdhtg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kmlymgqq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zpiopqmr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cksqxwlf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3schfpnve.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3otsskvoy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dotdwpxh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lhsbqgbs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xqpblnjw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3akhllbli.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3phqmnzux.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jyhqbejz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3klzbzawz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mvbafrxd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3adnvbjpt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lruaykoe.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3abqdyxij.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dpawmtdm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zmgnvqut.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ptuvrspq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wagquilg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lfxpkdad.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jqsnyheb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ainhcvkg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3imlghzfb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3eckeubld.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3melhoivh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rtzozjtu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kuwzkduy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dkhphngz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dohigcwj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3atymjkqa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mgimcmjg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3khzqdpfe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3clkbahqx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jjmpvhan.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3uephemjr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xhnqwaon.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3nzdwbloz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ohproams.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogposkry.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zloadugd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3leleyzis.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ljnarhrn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqczsbtt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dhzyzubh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yhmawtfv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yohvvznn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3emjibzod.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jmtsehde.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jgisfxib.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jqeglzwm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3afhkybul.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pipkhgks.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ixuxabqx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rewskqji.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqjuacj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtzgjhj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gojsanlo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ivbbzhyd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vaprylge.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3yvktnwor.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mrdrkjlp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3sqwkxhwn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3irtquvhu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3csxsplib.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yfdvdvud.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pykjsryd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3gibldwwn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pdgqtytp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3otcwqzzi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3chymibwi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xrfpwlbd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mqxdyjbw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zhlgmxmi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3iytflnao.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gbenkidd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3darqwqnb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxswmdq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3tfapxnmd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jghssvoc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3tctmiyve.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzplrpdm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ypcylchl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vajhcyuh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lchhlijp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fvyzribn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tfbgvraw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdnbkvi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jszmshlo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lldsgtqr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avfpoyum.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3onwpbogf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3prnkultj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gylvsici.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zlytrtum.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfwbaxq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dsrewpvr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ippxdbcl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bxkpxhzs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xbpgxoyd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pebrlfvi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uniqnrbx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bfggyjjl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pfaonlbr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxsozzj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jbqghzlp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nfhgjkau.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pdezysfa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ulkvohyh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdgxuvhh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jjzljvno.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mytzierg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3mkufawdj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3lomrdbmv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3glrpskzw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3etllbjpq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3titsjvlx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rxwkunqy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rahqfvon.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xupvmtpu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzivoxs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mbqhlhcd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bbyntfta.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rnsuhhtk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zaugfixv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nadykxxs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sqxvffiq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tbyfiljx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fdqnvzzz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qglybwet.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qcdnpetr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ccopyuia.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tjlldgul.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qonqbnep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlrqagrp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3rvpcilih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjvxjhke.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jctssxhf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tfgemqjr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvbdaei.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tvfcgrsb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tsdlyfec.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bmfwskvz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yedezakx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eumbkala.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ijnjrptx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3liypfxnr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rgefncid.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vizdgcgj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zummpvaq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3khwduxpq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ihuzwkix.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lqxgbeve.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jdvurfmd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cvpfbwcx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ewzahwmu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qqizelmf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhbjlpna.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ruidqgip.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldmfvrhd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3awxrasie.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jshsvaxg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3iifekwtj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3goigrpyb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3katsknqy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wtjwiqgo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jnsoeoes.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jspyytec.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxspxgcz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3acpfucni.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pndumbjk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qmudgmdm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yyntfpon.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rplkknne.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rljafqvs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3veixgppy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmvjfro.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xavzjfiw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbhepwis.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yhivompj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3klcnhcxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ygexuuev.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xruvzzjw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wwfrivku.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mxwaqhna.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3afkuqcwu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xabrdjgv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cerjcnaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pxktlhiq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lhdajrbt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pmhcfwmq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3yswlexck.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3shvvfhfv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fzwhhtgd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqijtwyt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xvrmtcqt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxvwliul.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hmdwczqn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3iayaixna.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mzyvpslr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zbwuvvqd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ghkaelpd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3swalmfte.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nshjpwpv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3prxalbox.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3awlfjxyz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dyqdmatw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3acgrnefh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bkrtffln.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ushbchnc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3umbqrhop.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nunrmsmj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nyzffiou.html


<!-- 参考信息 -->