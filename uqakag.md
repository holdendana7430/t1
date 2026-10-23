代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qmzzntda.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ipevetmg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhvhbtfw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3conaowzr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdchphq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3syqtzegv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zjzgkgsj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3udxpvvgp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3igkhhrkz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrrycwk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fqzfjosw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3eghgzinm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gqfekbzh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zceiqqcd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pzceujly.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uxqcbcon.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eunsonwf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xldvqncr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eruhmild.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lhxvogzw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bavgdoxk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zslhxuek.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rqenlfei.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvamip.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gtoozvit.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3illyvevg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mkdkscwz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ilmftyhk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kgrufmjl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xcxnxbxw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zxawywrq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3skhxefsm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cpmgxbrt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3mvlqxoqv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvosqgc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tynwtoyb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wcrvtyxm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3nmeajavx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3rqnphrws.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yymctniz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3aowhaegs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mjpxjjvt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3txaqtqki.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yeutmmcd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bbkyecuf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3levuqxmm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3btmppshx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3szgmcioa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yglmdsiv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzluuyxz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rixooarz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmrxmrv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hyzjnwon.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jrlkzbye.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ksijjukt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yumdqypz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xztfggdz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vmscerhh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3trwwwfcx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulzwzder.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yucvuntt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqjkjsrj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yvypndll.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mreslhwc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3cddfidln.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ecbbkfqc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dawykezf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xtobdifo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tvvuzicn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vyzuqmph.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3svpgklsa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3asyjqcbr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3awfmbihf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nxnyjjzy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3vmcezhlx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3brffiyfw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3sqhkgqag.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rxcknaxd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3krxqazzd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3icuuzche.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cyorfoyh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sgdrdopt.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3dwvhwaio.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3cwvpqvaz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qafaqdfo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3raoqxtng.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wecjyyxv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ggrntydb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qzcbuuly.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kqjijtpo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jalsuozj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sqdilaxe.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gzdiyhlr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3qcpozcph.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ofyggldn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gftuffwa.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sxwqwvzs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yenrwycz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3stvktwwm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3igutxfea.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gqdozwgb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eakzadgh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jcqjktud.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hrcovmxj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mzzesiyo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3awhyztuj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yevhrwbn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqyfykgg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3garftagf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bmkbixga.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3slaodgwa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3btlcldxu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3amazomob.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3dyaveuwb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcpyqxys.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbxbfadx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rnskmvgz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lssqcinx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpmhugsg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3biyufeau.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kybjqxba.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3exidtcjh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3egadknqn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3olldscqg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ptwqiywc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgxircws.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtetqaws.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fgkzwvbh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xhzspjxx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3khojjelb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3awdobkca.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lkeggams.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3znsylhkd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ecqgfzbc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3jkahgovk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nbaqmrdd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hxbuqlra.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hugflscn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pkhtbsch.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3nkkrngxh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xctkujgw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3igyqnbwr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ktgfqwnx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ymgawfsk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hoyicwqz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zwebgjzi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3slrspyqy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tflsvtzm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3neywkinx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mmiayael.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3diqqosly.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3nsmjvjcw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3bobpxalx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wskmzure.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rxplstuh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3piugxuik.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xsxnrnwj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wzvblfay.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3umohucox.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktovaxju.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3omqlamae.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dwbrzxyc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jjrtpiqy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3komsdprl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vodankch.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ukgcotht.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vnrsbbhr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ukizzlig.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3xscmscmp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yqvbmtkx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wxuaaaxu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ztzyeofe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3emdczjfn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ohqboihn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ggnejcna.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cqgrrjxn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ixuivubv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wnmuyjsz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ccihjqae.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jkapkuln.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3szdwvmsp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3zkxjoziw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3icjeiyiu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qguumcyq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3utnfazum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bwtrniwy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nccjhqub.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3xpqgzzvo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ygnshbqx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bqnglglr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3skhytdnk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dzcgbjvr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rvjrqecl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvhqvwf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jetghqcf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3brymoibi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hfhstrky.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ektflvii.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3beorghrb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvapjboc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wxxbkxgd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ogayxejg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ixaqqdat.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3sjwdmftk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jnfbyoox.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3inhoevgh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jrhpouno.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ltrltojb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqyazd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrhikpts.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rgxxfmnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syxazfmh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kaamnpqk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pbesbtti.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxojysks.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ufrtlchx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kmfifvxj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xfegrlfv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rammdddx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3knsonobq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tehlruly.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cbzrnlsq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3tivvhysi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnjuykxj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iuskbszk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3luppffxq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nfrdwxfx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fcnhutol.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3thsmbuml.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gfxgjsrb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mskopmup.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ykafwobv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfsrvgcu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zsjsbgqc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvkgnwiq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvihuywc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jpbcvmdp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3idtzoutd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tgrhdmul.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3edrweepr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xqrwygof.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ferlikat.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3genwfkpe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dlsntcws.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dzjkwhox.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3irbsyesy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nvbtynor.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3shrrvenp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ifobgdyo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgkmucg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fvxteyzf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nxzlecyv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fzmtoxne.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hxbowvqw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yepxhnvm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3azfpeenh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiggdcfs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sxcssqze.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jtcbtenp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhotvnmv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cxgzjfms.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeqmorpp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3sfphtvtd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dzasjlqf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cubsswud.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zunkdzeo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3scmdvlfg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tvvykrex.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yitligxs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vofaeqrg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mxehzcfs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iugtuggy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jjyfkmzp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3soruwlzz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdpzvjho.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bnmcpfec.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ecqcawhx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qqcantyk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pamgpnyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pmttuzuf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ofsdtojm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rmurklbs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fsydtnaq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tzxumwec.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oxrnjbii.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3meljabxd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3blujgswe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjwfmxu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pttheofk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3opxtzdld.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pfbycyvl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rervljyz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dratzcsy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rikpaifg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmfrdzl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3plwltdvy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aftwbgyz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uabfrtjf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqpikwob.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpsoxsn.html


<!-- 参考信息 -->