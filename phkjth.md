代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pmuschmr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zuypmsoc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oihmhvtw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xwkfuipm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tlchmmrn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bfpdkhgv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pjjpqllp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rwizygui.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3izqudqrb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3isambsqm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uvzxlwny.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ueudqqig.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ijqdmeoi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3givgpsjh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3rtkmnoci.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rueabkjn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpelkvuf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eqqorrla.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cihmonej.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ionsaddn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3izelntur.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mksztdte.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bedzebjs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxmptocy.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xvjjbzfe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gntlcjaj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wfvkxrhb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kaljvbjd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cufsnvlj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vmoeutfd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3okgbhqqn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3bbodlerc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3loisqvkn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3thizieas.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3psgykreo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3spxdohgu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rmhsejhz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wyzvreas.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdfazfb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxcrwth.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3wvputppi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3avvgtzhc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3hwdkdwue.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bcqglpht.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3igsuvzgq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzpysgr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3bvdtuggx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pgpnwreb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ivnfhtrw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3esmjwgko.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cghybiyh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pngfgglz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tdvjsqgt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sswdrnrj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3azmiusnv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3stwzpwtg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpvufhy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3dxmozoai.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xastrjre.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wcijujyf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3aizurfwn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zdtmqxyv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3rdgszpfu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hyodbciv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vglelfgf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhvzqjmw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ftthqxip.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3emxwapzd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmnncza.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rlwkihku.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xnkwppkn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bumrzhlg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yxrdjszf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qscwqect.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ytczoyau.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3etknzopf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rhqgsqlt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lmgvlowe.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dxfkyotu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ywutkltf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xecxospn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tgtvbiyj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kwvktxzm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xaajcqpu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zoswfmmc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3cikagosx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mcripujo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3smnvwoky.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uidlmmby.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qjtvdqop.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3devgxsqm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3awrstlwu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uzmjuyaw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mpfqgbjf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gwsyzjpc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dtfjaxme.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fjirunll.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rtpaizuo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mfcuvkir.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bmhiwoae.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bqfnpeyy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ffidwzhn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nrulerwf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jawkercv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nidvvkgx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kleoeptd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xrosdbpd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hrznnlgk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ihrjwibz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pcyugzhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3wninehce.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxfhlhod.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3knqfnvxl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3auzxsure.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3mvmqbhcs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dgiibubh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3exajfdtk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rxxchsgd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iusljgba.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3aazkaffe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3qnyknydd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wvrqnfzs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ctciymiq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cpexomsh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3coobqabi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yxgozrdl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rykaeevq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bipqtpcy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdhsjaxc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qhxhalyk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krlxqyga.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nsxhfoaq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3giejfexo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dnccpkfw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ozktmabp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3owssncwp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3byrfbeiu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3iagkzwpc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xvakojfx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fhdxcnkk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ngaoxrcx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jzkzhsvx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ugrxbxdr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vlbtralz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tjwvdhcq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wboxybni.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3buhypcjg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3esjhegfe.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vtobflwm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zcvukjxu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ztprrzya.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ogjbxdbv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ytibmlvy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zipimgpj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kyowkkxq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3eeocybkf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pjfqqagb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ntjcddgj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tveejbni.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qfcopgcb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vgaylzby.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pflyftrb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3laczohbs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdypimh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdhkzff.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uhuwmifv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nxuycbxk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lwhacjgl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pennmkda.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsrsblaz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yxthgzcj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3cvxnenxz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lqbmirhg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ffieofqt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gshcafkj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmndhoix.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jmvzukas.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yaxryosk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tinsaywn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nmyhbnxw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wopvkoxf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hbtxkrpj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vrllkmas.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zvokofpd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jmabnhsb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3aycuduid.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3otfnzpsl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3glidmykw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hymirgpz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cgwkfeta.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hslqqmau.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gakrhbon.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnkevcu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3quhvxvxt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gycjuojc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bolvbedn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pdcnwbwy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwmmbvhq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tavhggyw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3exypplxq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ppttjhuo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3slfkfmvm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3snrpuemb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kntkutqz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vlraizqq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mxrcqqfs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jhnxmlcu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3kmbvqqhe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3igkkxsgs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sexeahib.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3adezbzgp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dqdweruk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3buvyjeoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzqclenx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rhvioskx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwzyncms.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3okzeetaa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3meqryqgm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bswxvznl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gvyhmbqj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hizqibcj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bixljmfv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3osyhvsxj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xkqyzcfi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hpdbqxyo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fywdjbjy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ujaabccv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nrshysin.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3apqqayuq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hygqepjt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yckenrfc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yazjdgkh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ijvpnfcx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3smxskgst.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3owfcdtjq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3eoeezhsx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoatshtj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrjdtnpu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3suckwcet.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umvpbqjc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3adqdchpw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3stgqcsds.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hklzklqh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ojcezbes.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3swsgbvvn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xjzecdjj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfgybftq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjbwgxaz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhxheben.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3aalqfttp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3odqckzor.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmiryiae.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gxlejdcb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3aeqccufx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovhknunq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3clzaodfy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3puvvkxeq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sebkraok.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3frdqctov.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3imlkcglp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3boodtutn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qmesqmnk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wssxnvvd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kproqzdc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsxrqyom.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3spwowlwz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gmtlfvwk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mnvztuea.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rjhzbnfs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3eetbqygn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3orxwokmr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnqcxjob.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifdyilfm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kopecubv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lbajbmwx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpmkyafo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3aypqguxy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbcyjwxh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uqygcnkn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bxszctlz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qauqvdcj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhgvehgh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dszklfsn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gokdaazz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rmpoxkcl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcgxnf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tyfigbhk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rladuqtd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3iiimobzo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mmyvsbgr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gtprmysk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jvlncpvi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kumalyzo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3terizhau.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3crsxrqwi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lokyvoaq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kebicrmr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dybnvjrf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ckccqyem.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvjqxwv.html


<!-- 参考信息 -->