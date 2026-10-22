代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hhzqlext.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ifdzzvim.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ashvqsks.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwwjhpd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2valugddk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nhusnncw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ciuuqhps.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ueunsljw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jcbgyikp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2eevsddvf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xsikdgwl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqnspt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ymjeqeyj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nnihbfjt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2coyuackz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vkkcidsa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2azxdspoy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2enpdmjsk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2asgssrtg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2tawmdhyu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2scaykscj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yooobejh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pygswlbp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2iaewsasw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2uxezdzng.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hrqddvlo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kbsoqgvj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jdzxacum.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2clkmxrij.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jiwpvper.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kwywkqpx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vythuiym.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2usjvyxhw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iuhfzivn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bdhxaorf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mkjzfgik.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hkytpwrv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zypynzmt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ebgjxdeu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oznhsoul.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ojnnyvec.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eomteuoe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2amrlfwvp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2owrfpodk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hoiopgie.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2sofohecd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2vuzfotic.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fppoboxv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mxjjroos.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wwwiybtp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dnhodtzu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kljmnrzf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zktwpnxz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hhombzjh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dmdbmqca.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zdqbnrnz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjykwgwr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2srzymspa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xugfmenx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fufpuqqh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jfsinuky.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qejvbofe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sfdzwlnl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tmddsemu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eowpoauo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdrxsvp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bbjjlffv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqcjlefn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfsyyadm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2boslrcib.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zwkjiypi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bucwmvjh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2emmvynoa.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2sspgxjcm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xppmcskx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjtezbnz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2slibnfsr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lszyofay.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kdvazmtg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2mdxmcznd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2dpghfeqi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bykrwwkx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2geqmwhlp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2unhhrsky.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ctiolokv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lcgravoq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wfriivkm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2shpxmcap.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eriutdio.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2amtqcghn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ewvdihnk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vssoydwm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2qvculzix.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2czunxbeb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zjadnmxs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdoeopk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwgiqut.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2etqfwfvx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ahaiggna.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2isiruydu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vhxpisrd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ngashuqp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gtsbqgkl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gbvbsnft.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xgkeffwq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nkyaqayw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kpscavao.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2znyaxabf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rsgdflje.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vzjxxhvz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fwgcjomd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgphklld.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2culdehvb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nbcfrrkh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ozjonddv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2gufdizkq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rxxuglvi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rekmrxdb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wacpvfmq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gjvnnhtw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vmuyztzu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2geeuunjq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2hirhxbuw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wtttxpke.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zgcxiwer.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ebmhvnqs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2flaocbhb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pogrkzgf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2bkkmjblp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qbbcmgpo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnxdewif.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2smtjkdjv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwwxqzci.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2bwgmirfz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ecrrnvep.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hxgwblht.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dhieejwf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2brzxvlct.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qtmfxbxq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fkynsfhd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2giuvzlwa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwvvomxv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqmfllec.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdtmfpqd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2bebjxjzl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvqkkou.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vryfsmdz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tnvdqyih.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhoysqu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2cctfxllb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mgzhyrrj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2irguttem.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2exjhucrd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qobhugev.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ggkioadc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2atwgrnit.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tpvrnvvd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dbqpywsb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2txqbruai.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2aqqjiemi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2toorsjez.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2arazdlhx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rujsppli.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rumghigy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gwucmrgy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wsztnnfk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jolzzfqv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2humjzeld.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nplcoxbv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2uddcamcu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tpqfqnie.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2iatcerop.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bagdejsm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yhaivgyz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmzofkqm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlapwzvx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2codxlkcv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2htylbmte.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lzdowgez.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kreamspy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ojdqisuu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tuyrbboe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ppszgrwo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2angscxpe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hzwbcyxw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lhidoivg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czjnpxcq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2tzsujzkf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vyjsbpkt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rudhcyag.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dmmibcst.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ovcxgzzm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uaildbmr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2txjsetrt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rwgmqbfe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2yapvmxjx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bgclnayi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bufvcyva.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lsylybca.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jlhljseo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2slbngfju.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xktohqpv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehddqhox.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fsxaflmh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2eppaszbl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jhsrjgcc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rmpxmsjf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbyalgiw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2koiulqat.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ntxrqwec.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wazyxfii.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wrqxfecr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcsefuki.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2udvvuylx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tjsiejde.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugmxrqhv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qvviqmwy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2abpjftmu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqtfnlf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bfncemmx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ifiksesw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yeswbxyy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2gptfkrug.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zwxxcugv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vkoojdgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwrdybvl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ulebpuoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwccirew.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2etqkyowy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vbzjqdfm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dxtmrgtu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pyhqwcoj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mpuffsgo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fajxxexi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qjqmbfph.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zrpjnifd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vqdwwiku.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vtrbbjsu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fvfxsagh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlhjdrmp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nlassywz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dulmhqng.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2drdbzxol.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwsfihe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nvbzlqdq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nhqrzudg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gywjlckv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lobmqtsp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2awfwkzqd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaupktso.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rnqjtjmx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2thbrrpjl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kzcqtbmh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vlyxrolx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ckiewfnu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzeqtcif.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xfffkvfl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ugzcadmq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pklnirdb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyvzbbnz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2oaffcyrg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dnucghun.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2yidehcvi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2quqqowtp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2reaqypfb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbzwziu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiuegygp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tqznacsd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2isqhfeva.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dclcixog.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnpvkrx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2drhpmtqr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2grsizrjb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vkkykfjc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ozowbxyz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrfmlmez.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pqaffytx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xffqhiln.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cibjqbvq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cviqgytf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wasywjhz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2baitdgif.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywbqtoup.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uknblmbs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wsdfbfnl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xusokmls.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vbuukkck.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vplvjsdx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2pedbtdlr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mbkcngig.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pwixwmak.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nfrcshxf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kdhtqpux.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tqeiduoh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bimesxvg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pkbhrcqe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gbuymnta.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cjkbdwtr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2iztsoixm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2npevwamm.html


<!-- 参考信息 -->