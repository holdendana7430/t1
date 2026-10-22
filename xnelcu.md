代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2dwncdusk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2emjkbwoe.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gjvepvpk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rvjohndc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vcgumfhq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2eedjufbt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2tfqfumfe.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nowksjrt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2istwisqf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sibnfnyq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ypwhzlfc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbjgyccu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pcyagtoh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kcxrfcax.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nnlqyhqa.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qljtfofr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2sggjpfqp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfrnjvn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2eijhnzfu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bvqtlqsm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lptzpzjo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mfczktoc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2neofeyad.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2twdwrhqb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qktqvixj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fscltjmp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iiyulhcm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nhzbmzsb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2angecnqg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2hsbmolax.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jbbfzgma.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2onlqpdut.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ogjzwqht.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cyndmzec.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dtnjkdaf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2squmygcu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2sozphqki.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mktbkbia.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjtktol.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mhqreryh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vruyruxi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2frjcekxk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zxneqxqo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ksyvwaxu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzedccms.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmrvzlj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ggpidzzb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wetglbky.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcketcqc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kfkoclyf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2pkxmbqzp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2saazxchi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lbehaxfy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hhfngata.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xabxbyop.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hknsewhw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyhyxgpx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2egdcwuyt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wrdsmkoe.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vzxqdmhv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2kwtoswek.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2tdfolizl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ovlmhigi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2caaxajhr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hahgkdyg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nzbtqmdv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mukbwwgo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jvwhpiit.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rrrjjefh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jpokxsge.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2uedpkvjb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2uxvcntvz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2bmxchcyk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kltuytex.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vxonlyoz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcljpumq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kzkjgiuz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fndxcqsy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lvjyrdty.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jxiczeyp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gqdercnv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hfjikwzk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wlozfilj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iaktyoas.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oiovftgq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2litrsnqr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qhqqsnuv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uxwmmtuh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2jiaqpolc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ijmlfpwt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eqphaddv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gklbdyfx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oapbvoux.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2beiesoke.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uxqmgysz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qqaargzc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ihmenjyb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2deuzgdoc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2iqaynkml.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hgwasnek.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2glzbehwj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2omzgztpb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2canrebqp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zauslzrf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2imtebuag.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bqykadeg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2sbbfqsbh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dhcqvtqm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fdsikuei.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fwyitgnk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2sephzynl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lmueyeeb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xiwpgtzd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rseboxmo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdrexsub.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ibfpdrfb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zvrxqooo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kiynagrt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sknlxqwy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qyqaamez.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uzmdzoak.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2prvbiypm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rccnclfq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ipiueiby.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ywqkaidt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tgtxyzmc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsarzyz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvdabmm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2puqiqjlc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dvlylhkg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jeoebsli.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2djuxnlig.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2trsjvqgb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2cygitimh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wrhlmmkr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2vhsmwdky.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dgkfsvjr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xmsdvaem.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pwtyszkc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xcuqexml.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gezdgihz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xdjinyoe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2uepnakjl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2peycsgqr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uyuxwkpn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tjoaiwxz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2kwuhtypc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ecppqkkk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2amtrcuny.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mnqqvhqt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dbwtitsi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ehzspksq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojgooncg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuqchia.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rwcgmslq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fslyluev.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bzypdmts.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2viyutqqe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oacddspr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qigwyrlq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nqevjcwt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2huonbbnm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2yaukysvp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rvrktfpi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2diugancf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ntopxokn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdaievmx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mmmkiaxy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nzvpgigd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dfmnpvee.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xpjodxsa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zpfapaee.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xpnmlivm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cqjqpljr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2brwnxado.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yninwxsx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2siadyvvq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rtszadiq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nohndaeq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mljhilrd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfurqjyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ktbgsnmh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tbdilimb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tyigkcfm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxueyter.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gmuwflus.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2exqfgwyf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xnvaxojp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mpavfiap.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uieveyyp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zljmbbjf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2idjossqz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntruydus.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qwsceeni.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tmzdnwkk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2znbuwxua.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gxicxdym.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rnewpfzw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxdqgfj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2thiniysb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bthmsgxa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ofhowopu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2echtxrsm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ptzlhazb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vhiyvnlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjvvzjlr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ucxazcse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kubwaugb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pzekisqs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2edqkwwon.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dmdnqooa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ydxyzdmg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jnxqjfif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pgdrjenz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2llclgucr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zzdcgybe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mutudmyg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tqmyumyk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2exyvyyzl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2lilokphy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ooohxzzc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lsogsagv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yeudtozz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zvlspgyk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mdtyketu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2edbbnnlb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kbgfhhmg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xlxgastr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwevrfpx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2foybromx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxyzlvo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jjyizcge.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hmzuosdj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lydfidua.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oweppclw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2foxxiwaq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pnaznyqi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xjlqzfhw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfrtrxl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xsoxrnxo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlojpsd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ebgrblda.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fhezcnhh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnnupkkz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wszahvym.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kknvhuzv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bkwmxvxd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cwnadmln.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mlryqexn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qyqlxjog.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pohhjysp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2koqwvzhp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qprhudww.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ugitjwdi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ztjiwtmh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkyqbjjg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dkdkriwg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqyzhlas.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtirqnf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2okkjkffo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qxpzktgr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzilmqoq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sqigsxsa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgszgqkj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjdpaho.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqqcbxg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtftnnqh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qknxudeg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tncizwqy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2anvxqzso.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mnuolfal.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2inuvlzbo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ibbwhvua.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2akcqwynk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nukesfjk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aghvazrg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yljhqvrs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2itttngux.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xodnvoyl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2neucyisr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2urxkondg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zwpaisrn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vzllqvtq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fstuwiqp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldfpmoxd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2arpnapye.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rtaguqda.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dlcowqpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2buwkozec.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cvyxrkhn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tgibruec.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njobwccu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mqietbyx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2whyiztaw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2puexxmjs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2plmcsrgu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2upyezxbz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzsnxkef.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2utdrfcyu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2coygydse.html


<!-- 参考信息 -->