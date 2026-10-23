代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcaisily.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fumwamvs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gpujhuob.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bdbaavsj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3deaayrdp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3uhbiafcm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3adyzvqmb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qceaxyrr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xeytegog.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dtsneaty.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vaxvswpi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mkmxivfq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3puzsdevd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cifndmus.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ubwjdcul.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3novmwhlz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uxrkhciz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3btwikcgu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tpuxdvbr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uelarbgz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uevngncv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fmeeppwt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ibhahccs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ngtjeqiz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rjproeca.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3otfxjyua.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vqlckbil.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3trmzotev.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wuzfjcnd.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bxlsrskv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3usgwqesk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wmyujqft.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3iyzvkbmu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3iodnfedy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xevnbnpm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mosrpmls.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hremjzzw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kskpfcub.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3thavflrf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pfexpidk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lmpyvcwd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3cqgbsewd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gleqvfil.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3czecbqfl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzmpldix.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lknywcwe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tdjgfptk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcglvlcp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwrghqs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3agepupaf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fspudrss.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ezbrpsyz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3akbkqwmn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3opgqbayw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpkwhw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gcxcctcj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zvsbccbq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xgismcoz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mcjgxwry.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3damlyyrx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3secbeehx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qmjgyvaz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3svwigsju.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bekmupjl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3izjzyjxn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tggsnmqa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bdtypapl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ydsdhglp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zkdxhoin.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3znacmqkg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpqdgs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nlolvzet.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkelzbr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fqywdsxy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3potrjxsv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwsybrv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3iaswycbn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3iuztydex.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jmacsmdo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3uwvjuocb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dakumkml.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uwkqgmvj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fwvihxyr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lszkqztc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kuuecsaj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nlfeohum.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pkzcggdg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vqeynvvo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gwhjzbxr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3kovdkzwf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qspwsvdv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jcuxjlrv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mnogwcgy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3iwwoxgrn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tafengaw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3mmaghpod.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nozwqyhz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gklwkaef.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xrkrmxgb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ourwslxo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3najkgtcs.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3euvqlidj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3usjzwgsu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovcqltte.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qqcwsmpd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qkqrgrvs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tkwldozs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gzdyxwkb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3druhxtsi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3aypphiml.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oewuibeu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3cizevmzk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ahpvkvkc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yxoqyotc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qcfwoxpk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kzvnhxzu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tkgzzvtq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vcspanok.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qiatctlk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvuzeiwd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kdogrodk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cfdrjnmp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lsfofjxb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qfvvslbh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qlxokznj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xycxjqac.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sqqjkzmc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3huolwier.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtseeyd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zmwptceo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3metpwnlq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3sibchkfz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jqvaihzr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3stkvchkz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qjltglqk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3kvarxeeb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gecksvyy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nbbinmfz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fgsjbnwf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nlmhsvmw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oqvctovc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nwtxuyop.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ujxgkrjb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3inuozubh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cftltsdh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3abskegmo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mbdnhihe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3sovrcqyk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rucsuapf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3fwypdefn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xlmnberz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3amyfjpmr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jboosdnl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3efbxzelz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vrwpwszo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgpuvenc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yzspbttq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3flrowvgy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kqoxqwfb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jvdcpygk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyllporz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3junxzaao.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3klqskjij.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3iegdjepf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3wlictgqw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jvdtwhty.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vmlogruo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fqxjponz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rdmkgfsx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lqqrlivp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ajhbwdhw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkfbblz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vuejwaxa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ukvcyzax.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wqtnuwpz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jjawycjq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ktgosxpr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ufqnynze.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mpckwtoz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pwgbrfmt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aubyciyf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bcfdjnjh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eexpnqsk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mtfbffwi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cedziixd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3tfuborkg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3htubkvrt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hakulwab.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wrqxtgzw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3znwnuvtc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvcywzox.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkrffeqk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqtzgohg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3giyabbpb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ksasiyeh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxjtlxmn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3dtnzdrvs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xsaufqpq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3euyaehhz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qfrwupzp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jgatrhcf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeacqaj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3qntaomml.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ygmlywex.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xfeegdat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibzaikgd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3apipxksr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqhgbbcd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jtbgsmzd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hvhneupq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3adwrihww.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ldkgdybo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fmyubbde.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dplkmlvo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ntjbxlzh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jhggtaij.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ynomzpxm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3boouhouf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3upfqofsf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rwfaszxe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mtnzlmas.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mvwiujwp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dkzpjcqi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3upbbepbo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3trvcfubo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aeanhist.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wuaphbpd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3igzwqkgu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmhrqftm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bubmjbsp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpbupckr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3obamhxdj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kipsckek.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tsrgqjyw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3apfwbrqi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cleliehw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3djtdlqhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xobwihdn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3arwfnkes.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ivhxedqh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdholid.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfocdbcf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tapbrnkl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3izdnwlfg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gytltyzd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3shfcylju.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmofryi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgsecegm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiktyixt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3oqyqmyzw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hedjowka.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqfdmtp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmikkezm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tsofpkor.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nvdbxvuy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ndyriuxe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuqbtxux.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kkvsncip.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqqzlppf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zrxvrpkb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3btmraaqx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rtbwmvgb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zypoltpd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3anwvjenl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3afgrmjqu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysmwpwhk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqsugvns.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ulzhlysv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3dyscrpuq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfedudzr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ampdvaii.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lxewjtfu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3obnxqgfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tssdmmjc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3idwjracs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cdxdpasf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ccghaxih.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ofczlkvu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3djkmidzl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3npmvcslk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3khuqqmwl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yetkejft.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioqkzndg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eodwmigj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3geqgxhzk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sivshhxf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kjsylnzc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xavvqikf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxehwai.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3awshtwss.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdplzat.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emjqrmlx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iycmstri.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ynikkplu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ttbpmcws.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lbmcptbr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iowpvlor.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzgilyem.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zuhbtwnp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3arlyzyhq.html


<!-- 参考信息 -->