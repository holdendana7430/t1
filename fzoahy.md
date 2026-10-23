代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hnldygql.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3orvylmus.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3zdnaxrub.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3brthembj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3siwdqyem.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hjdyppqb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tmhokcxg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cbyrxwyc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lrilobmo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3demzccoq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3moieahqb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3chfgzkoo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qobpcshn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ntrovkcu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kvjmnooz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3fyeaniup.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dayqvhyv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3shldlmsz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ukzzgpmo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3sziftmmf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3subkxyft.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iaoemyif.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oipblfrp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dwfehpuy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nmrapvgg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dnfptmsl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnkbmtbm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3basffjwc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vkzaftvn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3puvixsww.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lnttdjyi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sidaawkz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pskhinvg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xqozjrnh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ujvzzuhm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dduoyfbn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nlwvhbil.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3jwvsokrh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ftphbljt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3udfxtdcv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3betkhnxp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ozmdzwgj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fybwlgbm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bczqwcxq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3nuzhneep.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fnlobsza.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3vyewrjki.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iymxpxxo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccwjeusy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlyttpi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3lbjgkycn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sjemwuuf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tsgtabwn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ixmxgxfz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hyvpldbm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ekjrcvfz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nvjdyiay.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kgajjlfn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zicousih.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yvectkli.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wyirpiau.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3abmlvvro.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xkbawgzs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dshxeafv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xmmmyisv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ywplbmed.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yqeqvrii.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nsdmkzxk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fyuqnnpf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3efovkmos.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qghvuibu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3rntgthaa.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3brascfcj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3sxgmmcro.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ltqvyybu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ootthyob.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3avlszofa.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qnxrqmgn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rkdpbglt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tlqcqkxr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gjznckxl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ipcpomsc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nsctdptc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3kwbagqro.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wliizqxh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3netymkkh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lblmihwg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ngavivrg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aonifrrf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3maoovxjp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lnkcrttp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3kxcjbawg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lhhjxrlv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zfopqfla.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eevglihg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bwojxbmp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zldjrawq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ipterrhd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qfoqgwqg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qdllvnzl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3obnmyafz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3khamwgbf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dttdaouj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mrojrmmh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3drxsugou.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hgudmmeu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cyarpdzs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3idkcikln.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gtqscntp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bsprtjrs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jmetjlrn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3irxdixtm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mthslbar.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lbzekbrg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3adqcexdp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rgbjssnf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fkyxwfcz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3neujcdii.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zvoqvrlk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3urkcpeyo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zpihwtuw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3grxjmhux.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfgbeiji.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byzvafbc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3bfmdwofw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3bswfkeuw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfmforcs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3iwgnbbwj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3husbjniz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqhguahe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rfdctkfz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pyaisbic.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hweypbnm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bemxrcnc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iayvkwas.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3enimxsst.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hjgqqmpm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bmqrhynl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sqnnqzws.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lvlaocbm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgbruxh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3rpihvbxg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fajrqjhd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vkgxijqe.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ntldfolw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmbgolio.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jaiynipz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3arzighir.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qazjlenx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jzppxiwd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bxxknwep.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lplvylfr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xdgpyjzc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ebvbnxqf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mqjrgchr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3kyauxrjl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mlzzprqq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hxyibstb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iwgpmzpv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kovvtdts.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mgncbqgj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qafgfaxc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uodhxouw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bcknbbgo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqoaslbi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyqilpj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlufcbyn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3udalseej.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yysuqqgn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wggzayfd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nzpmletp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3mrcnbrtl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3soahsxeq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3swdmzdjp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3sziztyok.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gpyzuikq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mpyjuoan.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3cnahjptf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3niuibier.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yfymzejw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dbyjehrh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hwhnuxaq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hmhywahl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtgrygk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eircoesr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nvvmhvsw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yjgbtewf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixmjrjnj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aqrfaxia.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3izxmkiwb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3dmjcmexs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3bujfmlzw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3btgazpfl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hrnuuogp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ocortkql.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3viiapuvm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3czuexaar.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jqfpywrq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nqmwkjpq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vbsujyid.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ciadceyx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vqtcjhfi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cdlvutwh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xerosptm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hizmymtb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkwmiurp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3sxzjvrsu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3issqwjvd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nclfmybw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3odsqdwtv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ykyashzf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gzrjfzaq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tgdpnrkd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pnkiudqr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cozrunrw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3akkgovce.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tmpuiyeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxxbpvoh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cfetfjro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjhenkvh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gutwfglp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tidmumih.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyohqgut.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ztrlxtoi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zvgypohg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pujmpzos.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mcogqrvw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jykhvnju.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eumqguxp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3juozuzcm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3onfqsenw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvmrdwnx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gdhrenlh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ijpkhvyh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nqtsmvco.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vettgzso.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tpiomkfx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qztlqipz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3whfexics.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3emeytxun.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3voqrbccu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kpyzhgps.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pqbqcdib.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3spolfsdo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lhcxbmeh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3prihhwtb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3blvpylni.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvmpyaqf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fzjpagij.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wadlymna.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfekhi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pypiyydb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qknfpvdx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jhcdqowc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3odcnnivl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzxwcaky.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jnrglofw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zceooiez.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsonjlzh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wnnpvvpf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tlaznhdl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdcyscap.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ptmxzada.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bpncewcn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dfgapvjh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ficenrqh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ghmnwcqc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqalblzb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnmyrmda.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fqhknggn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxhvcgol.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fahkeuhb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3shctippz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ucarbiqu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3huhbtara.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yzpyhqfm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaaxxjja.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsvkdhhp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rejpzrya.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcrysqww.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gclmfujo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3iihwfdia.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqkgsppd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cordywjg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yixdtmpi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mdezoigy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3syfdjtyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hlhoowoh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gysfjfks.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezjgjttl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qjrthzqe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ztwcfgyu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3tvvpvtim.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xmawcrqn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwngisgo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvewqgxl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkyzbgjs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlededof.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zzbyanmi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bwwexxja.html


<!-- 参考信息 -->