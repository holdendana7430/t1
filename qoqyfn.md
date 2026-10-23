代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvykfjqz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mmkqrqbv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cttjnvxg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xvwjcwmp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3sushnnrm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wnjgkgqy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jkxwixow.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3cifurnnb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ogjvxyhi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vctjxxvq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmwrtetp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cgworwfq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eucsntcs.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yqvpbiwb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhekzvbd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ieqwbjad.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mneliwrc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xftcgflk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lbadnvvx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sobouefi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dnnranhh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fhkscvqd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3fvbxdggp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mtbrazyb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fksptswx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fafiabuz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oosdtxpj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cljpyztc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3lctcmwgv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rygfyhut.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oqmlxpre.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dzsyhknc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gmidsiaz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pdvwjdam.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kwkfpcqj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdgzply.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3souyxyua.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3prwpubyf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3uvkaxaxy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jphomjjr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xouwkosa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hadqeuap.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fqytsigb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cnovampk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nlpzmqvo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ibvglzgg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eofrfyru.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wnvopehd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3akbrwyxn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ngzktccf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3kjmwaqvb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jbyumkwb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3njojuugt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gppplxtd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3odjwvlhb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ioayndfo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nejdxydt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsxcdlno.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pkxdynrx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bzlrzgks.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mfvkifzg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vyvaskul.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zdsefjkh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3squzgnoa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qzazmzrw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ihpvgitw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nytjymzk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qvnoipdc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dzxnlzkg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zeponkwo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ycjytegt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3lczxpkkg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ltnxnhdu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3twbkcvmh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gzpkqqcf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3kderglxt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3moadntli.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3sboptisr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kpjnbwml.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gvncibyc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uksljnaj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fwftmucl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jxyclceu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ehxldajp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ylvtkhuk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jicmneec.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lsvclcab.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bnchivqa.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3rswmltns.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3efjvydic.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xfenyqjw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lmkkqdmm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zdeulpit.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3sznohcba.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ljwyuqjq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nfueaeed.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ompikksn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lmikxyyw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sabonihj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rtorsswz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fmwrweno.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kwqtawba.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lphrtdra.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3yhpxkrlp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tpdpqnqf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eymtyzvc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ffeiznuf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3diplwdac.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oyotsaqj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3eiyhldsf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3wkyuymla.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3cujgvvjt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3geufqmdp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3palpexbf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqhidsqx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3pmwbibsb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfqafeuk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3foglfwop.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tuhbvrdv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eqhcnvki.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjrpdrvv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xypkejic.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhrskhhr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vlyvhmgq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3adqbdbdv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lkgqfkxf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcowcen.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3axtogedn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aoobrprd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ynextqys.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3vkqzbtpi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jjvsvzkq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tbwwfyvf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3viaujskx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fqsrxshc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3figlbjmy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rmzhxsnn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fmzcwudq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rcyjzoln.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uinboiql.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eyabhwrv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3miobeyef.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zywgvbsd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dhykypbh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3xmnlfhxe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vxqbgbin.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3enzflzuk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3hbjhobtk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vemgawme.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3mdivsggq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wbzohuiy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ldibqjjd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3pkudlwtw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfjkpwb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjnsdfk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3edyrcbkt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dumtapsm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ogkupymj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wkstzrab.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wlhqqzhg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gvsshppt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3navewmmf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3bsshvggu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zpbtnqiz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ckuiotrr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jfrbznck.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcdfjxhg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zabtgypv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ycuzughn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rienizbs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zcyvwbex.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwlasmsy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hybfbvoa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dsgnygqy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ywdkhthm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfuykmwp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qrwilgqa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rupwqwrz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rvqrzvim.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zbpomqkw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3thznywzd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xrkozxae.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pohvxriy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cwhzoxov.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jortnaae.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3utlyytcz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3infnxjpn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3njrxgqih.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3cnawhuha.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3crvmzmpb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tepuxehm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rasqqqiu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3scvsglho.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3plmbxahb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dxowrryh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtgrjaxp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jyiirfqx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pqnhesmr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qttfvbqg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nvehmhub.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3znbucvym.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrwrvwr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lvbhpkcm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fwbdhflj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3edaodxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urivbkef.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dgsnagvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbpdhofb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3tleyryad.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3dqvroxld.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qxgyrfob.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sqnrdumu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mbmbewgs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rxolquju.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ybvjgmdb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xbzoraly.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3actdxtin.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ilbdfsor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ralhpucm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3taxmscal.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yjtenzzz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gptvsycg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3betrujos.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rdyelryb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3cfjsbxnw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jrdyjwfs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nfnufqbo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jyvtkemn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zmtgagwr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmhoyfrb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvonmme.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxhpmfcl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mephkjur.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rgcvkxsg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hcxczyol.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ryoybedy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvmfdft.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgctossa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ipzkrmlp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gbrknwxi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgbstrjq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3uyvwagha.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3baxqqipy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrubjtfj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nfnzgovs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oxbnvubl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pynnvvgk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3eqvxigum.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqsmzyfv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oexxviwq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ynuksaaa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3aylxrfgz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltzqrqkq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hvbdqluf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3iupjpffu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3blhnkmhw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qfmxxgdo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hnxdkmyz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3djaodson.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3nzilxsga.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3daznvons.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvfjoav.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzcfwcqw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekcioddt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vppzhxag.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zssjssbc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cgtnfatm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjbwgixt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rmbdoiob.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ioimnrag.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gwpooyyi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bwoxotzh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3daxnymhz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fkperooz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3klpbhtfc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wutsyxkh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aqqadygj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3eporxzbs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3uoznjsra.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zefwcbge.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lpielcsj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3dqsjovzl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqynbfyb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vabsfydk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ltqmoznh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bagsbndt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gauqslsh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqeaxzfz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiqmvylq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gpfhmduc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vjrmqxhm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eaaoilpv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qjugquso.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mtfjtlui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xsdlixwk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3gbqviwmb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uajjmnii.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tcpehooi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mxtdsbaz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uyiwqszl.html


<!-- 参考信息 -->