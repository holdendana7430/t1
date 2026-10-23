代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnlagme.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bsfowhbh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vqrnkhpd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3okxumdbs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vfwvhuge.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rviuwtbk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jopovzzo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xzxsppdr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3udztizdb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yuincuhw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ygrdpwob.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kygaaxku.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pxhccoyg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aribyqxt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwadqzyh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jxjlgaef.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3acuynihg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mvslgokh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fhqrfseg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qaafywmx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qtglqklc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jcqcjtrz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3vycbxigz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ruclsjbz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3anfhktmy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3lucfuqyo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qzychxff.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vjfmtdxm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vzyyamyg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vioueqzp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zonanmwj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3exaiqwox.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lcrgxakq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ialhyexr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xotddgqp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ukckdkmc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3tuceziax.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmroxfs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqetfbt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rzawjmpc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ckcfiwqa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wikvthwv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3khlqgsfk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lpsauxau.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3egdrqvpm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ytnesmni.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyefcej.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqfrkoxb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rocdaldx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3udyoroyu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3earokugy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fupjmbkg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3prwcwtjl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3azxsjeue.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3wswjrshx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kvlbnlvy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynzhvcaq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vwvtjccl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3knwejcaw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gkygevll.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ltcihmha.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vatzbpce.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3khtctjsq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xfokttvm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fyhiaqfy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mwovoejk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zajqviic.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3gzmggvbc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3acwzhbvx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jvhgilzw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3oimdhgzq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3iveumnys.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyuxtubh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sbysjlhr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pqsdbswr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vhmxmnsy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lpspguli.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sgkxvelr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wcutrsfh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fuoxphyg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kxqajsik.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jlyctyys.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bibpwnto.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rlrtfbjm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zrqacybt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xezdbpcb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3skeeffzj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3arhmqiup.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nlcctgsd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cyqaocah.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ewsvhbej.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ryhhhpcg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nauevhfe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3skellukn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3puvngyfl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tobcpzmd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3maojuhmi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cqbgotca.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ejvglvun.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aylnruak.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lqmxuozg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lksbsqyz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3majkwzsw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mjxlztfp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fyeiemye.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fffjlzab.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3sqddlqse.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3wdofddrt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3cmzaptfe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3fyunwliy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcqmvfki.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3dwtxfvda.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jozczevu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jftalaur.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivcvkiak.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3irlstusn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zmnduetb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnbvkube.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jqisbald.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3reqktevm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zowlnvax.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oxlbtsbj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kifcowzs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcdmytqc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3banezjze.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dmwcxugl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yipbcnnw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ispmzitm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xszcvudj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pvhowycd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rrhsgxfc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pomalplx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3woxdegbj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qzrkwriw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fjaddzpk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hjpsbofv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3domlbita.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ryqbsftp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3fqhlraoz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3reqiisuh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yetfycqt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jolibmoa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xujykyyw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xrlrbvww.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jcjmktpj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hswfefwm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mgqpmnpy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3yfzlbhxq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3spkxhsfe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3jenlheud.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3inndrpaq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3lsqkvipd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ilfnrpxo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3emslhxrq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyjnrcwa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztutspcj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hngdxoml.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sfdcfrve.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3imbbtohe.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3iatcsglu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmoulwqk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tfmdkuar.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3mqqhfgxz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3uidtfiwi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mstzwdvg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jjhhpgrq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejziqtsh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3obwkxavp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dtylppyu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sugextxu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3plemwdss.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zqskwtwo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wscbweco.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ashmlrnx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xzcqzpph.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anuvmffi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dtcwvluv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3yetzyhnu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3avqxpdts.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qouyhwmb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwtenufz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3amtvnquw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fftosclb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rcrjuxkp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lovqkykh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3itnunkyb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hjdlbmrw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzvkovnd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mobpiaaz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzvouad.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3appaadno.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3shduproi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pzyvzgtv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kmzmmwhb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ynrypgjy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yfqtnzjt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qvzzeumk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ufpecvvx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lhxlcegc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3eqyxffwn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wkaufnjp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ucymdjpp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xjmnfvfe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wzdyfctl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzzrhbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ryxuscoh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bngqlfhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcyvycnh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vmtoxtsf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wwkogywt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3scsjsrma.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kkwrihex.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mdurnqgy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bbbxfbve.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qrrcmfex.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3yevpebxm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jhhzagbi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pavpxwvy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3myzotexv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vwzyeomt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zklxeloi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wsthwkvq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3plrnxhci.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wnkfqcls.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3agisongf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kdsqsjjn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3qzviueje.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3irntnzco.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nionzybs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3safjzace.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otrtbyxs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yobzzypz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fvnlzpvu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wxfakepd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ektznjiv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvwhimii.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mohwrdly.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wacjjgfc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pazcffru.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlyrphib.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtkmknjd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lbttvleq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3orgbtslh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3trlozxba.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3icyksipu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3sspcfeko.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnuatuvz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zyfbqrxj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vxoebohg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3snehkuzt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ukuqlbph.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ujpwejxb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzeprvnt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3cjraxmmv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gnssttrg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pifjdyqq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3omgiooin.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3scwaagzc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3runhmlqu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vwcuyhmp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3umxnddkz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xggxmszh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wllhfzyj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hckkwvmf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkqazkpk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kofublyt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3peiicjmw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hzxjjalr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pxhjsmgn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3buswlsfx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qrhkxaqx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qgpjjwne.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zxpxyxug.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qdenydnv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gfvhdkho.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oumbagnb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3izjivtaw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lyvorsra.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3xmgsraqi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ohrhuyuz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oxzygxzp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxjirxgj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhmhcewg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrpyumxi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3emqfwxrr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mplhcmqp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3exjqsufg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tyobmcws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxszipzy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ygniuvat.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zmiimjpp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3neydxumt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pqqqlnpm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xesogxpv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uctirskd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mbsqfxux.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnnset.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qrlgiqvj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cauunfgd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jldpgrhu.html


<!-- 参考信息 -->