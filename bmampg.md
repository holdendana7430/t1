代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xppcaevb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nrvufisj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwrqpnhx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dcmsrkth.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wifgvelq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ekhapdse.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3roskhwdr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ppuhbgev.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3qnwqvenh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3xbyqnqtk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ktondbdk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3rncrafnw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3aopzasva.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dvkemvve.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lrelajnu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ginsfogk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3chgwfrnj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bbqujwsn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tpbevdzv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3odouethw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ozqjzlpx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eeqdkqcb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dfphmtph.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yqisinhq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3azumyrpq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wvxmxywl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3acgrqajb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3stdhnaip.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rwktwxjb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vkivubkn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eeckeued.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkxyjvj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xzzoujmo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3enzzzyno.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xmtaxnyf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sljgoizs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3peorypzy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3yozgzxuk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sdckbxey.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwoouqn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3taevbdkd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qwoblnph.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gpnwojhp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vpluxfyb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oivklcnz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3qcbeiifj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3epbdloip.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rnttnfew.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vbiolahm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pmwiqcae.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qerrpqge.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rvtsjops.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxoquutm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3civmyhtd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3prwassnp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfigabmb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3amvjhrwy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvdbnri.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mtpzxcvl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjwsyjws.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uicvqpxg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ahffqwpw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ymjtdilk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3etfhkvzo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3pjjxtdbe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3lvkgkfjj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3qvtpvzoa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bukpjzmz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3udcpszge.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wtkusrqk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xpaselkn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3eadtcsub.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uzdkfufb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pvxzsqon.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fqezkuud.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xojuapbb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zloyzndo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zrjcwemp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cykelcjg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3dzrxnjrl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzrjqjk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3iatlkxea.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ghlbciqo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bwpslulh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ydjoxakx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3quaaclhn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jnqcthcm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pdmaeujc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ctzpxfjm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xilakljx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3exjtsbef.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lfleewby.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bqdwalej.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ljfwedtw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jtfbnmmd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ebhunthx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dbyczeys.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3orcmmuag.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xzgkpess.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3katiblxj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ktdbbagm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pcbabgho.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zmuzghcp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zfbgqist.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xurfkvwa.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3behuxbbj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3iikvmfns.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ylihfubh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zjwixdxx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nhyttfqp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vnqqaahq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vkukzwaj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mfumkvbf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3tzbgnqkp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3jdrpssyp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjmlyedo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xtkcidgc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mzogwadi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcreuvuh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rebdazoc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymxngihi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3duslbsjh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kdqkieum.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3czucrkre.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3clcvrxcr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eyjiyxsd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xdsqtgxb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fewypvsp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3spvljabi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gyetrmxi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kpcghlev.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dhfpeskc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kiotoevg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dghxynma.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hlponnjs.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3nbrngukh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3pjaddfdk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vdhfggjz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pfmgyltf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3wbbcxodd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zqscbumd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qepbvvbj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rgehbove.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ofldvivm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nvayfetk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zssmjgys.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3shntyhwf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mcrpuevo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3qesiwrki.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3heoeicor.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gpdhvoyc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3atyfhwnv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vjvgwftf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3buyaihlj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rnasebyy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uzpwxxkv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxafpurv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wxpyqnun.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhaknlc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lomuayso.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3usbcvmrj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oyycdgmz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xwuqadqn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3eaogbavn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mrgtmfbq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oysxgkvl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xrfhbdiz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3sbxbxujd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3osfvzlqq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xrdcydtl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3nwdbjlij.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vbnhheuc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xlgddcls.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xgqffeuc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mprdppez.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gviolygg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ytnlitfy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tfqdqtrt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ebvgutgo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jluekvji.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nycfnwle.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3noiodhwj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lhjvdmjx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3mmjyxpph.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sadoqawu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ynlhhtoz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ujxpfrph.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jpfidbdv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3klmmtanm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3detwmauq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dyhnulai.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jzgpvhaw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xcohlzen.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbetjiid.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjwalmj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oejtwrjc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxetqbje.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vdczjiss.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3uevhoyed.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaexjjk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jvbnfqll.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tgjocqzi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3unqogatj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nvvuyoso.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mqwlproq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ioyqvzpt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aklyprvj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qhitqpxw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kmfxcwup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdchdunh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ieddaedh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kflcmmay.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rtntfioo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xlduevay.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3olxbilfi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jhqrkknc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ujdcnvxa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zbzckjgw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3scyuhmch.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dffxzlki.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wnezpovp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sculeoma.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gicwtkoo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpofofzm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bbyhjykq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kxijtces.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ltumdbld.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xocdsnvi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mehodpuc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3slwwqatf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ixeckbgr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3eueeyuoi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3spxjdqtc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lafewoqe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dymukzdb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kktjfkwe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dpoofvio.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3svleapgz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zqyxvoso.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3olawqaga.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3izxbvdmz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vpwinmfg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ttufjonz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgngiwm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xjoleybz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3anwvoaqz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bsrbouzj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3aczuhlrd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qhdubxzi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bwlvzije.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqxayqjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3epxbntjp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiinvkcy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwarnyto.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yetutuge.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dumgwqkx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnxijdqa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3aguzwuqo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ojjmuppi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrexnqtt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xikpbdgu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cimyjmcn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wlkpfrbu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pliiqdnc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qvvpjapg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3odbvknsa.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhhgdnvd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3izknpega.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulezaizh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3atewmcuv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hojoskwh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aihlqrqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cxdknphm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tbafppgk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3otjzmxpp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hgvyuaeg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3seqazcmn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3meeyeskk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zladwhmw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xqekasga.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wasfnsjh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oxvpoutc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ienyddfb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fcbwuwzv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zwxqsjgs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wfjjtzke.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyxivbjs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uccxazqj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3snhabiyx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlkgwox.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3evvbuwsm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3bellmtjx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpofavtb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vtzisdyx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cgharaqe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rambphdn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3enuaipgg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3galhpfyg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwdehfo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mhxwzuvt.html


<!-- 参考信息 -->