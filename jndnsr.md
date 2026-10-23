代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3thumepzb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wssltabq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ovygbnlq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rkxixibn.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eopqhufd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eyibvhyy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcxbrrcs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqzaebk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3crbmdeih.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3djqayjhx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bmxvbznd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3gvgrpzhd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3avghzejp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nyjpjfcr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xxgubfxy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3bmzptlki.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dwfaoqkz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ldaztvpi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wmtumxph.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eaijgpka.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccypnruf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ntynwsdh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qmcvohav.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3biwcxryv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vpnarzva.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3alwyvstb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mljxyelp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3degvqgsx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vscrikrx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gucdqxoi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3flshizhe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jhhyosdg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tgdjnnfn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3emveowdq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pbsgudqz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qlrefleo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3zmrtjred.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3aytemfpv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3mbrkakgf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vuysvkla.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kbakmqfv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vninitdm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wteufloe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xmgvfqgj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xdqtnsbu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tmmenojy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpaypyc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3miihqhhd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eflyepjv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3iuukxhxc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vjuhazyh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rygsoyan.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ipvsjeru.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yvleqbzr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgqmktdg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ijnernpm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cbnguwjd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uklffbwj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mjucoovb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3epfrcfku.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rqegfwks.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3aeigyrmh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yurksskn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zidbotui.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkswvaaf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tcofoyvk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3oeoibiqp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xhusitcd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yzdpjuyz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3bsarrsce.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3obbxunnh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kjozvbma.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ckumppao.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mdzwdkfu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3coejteeo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tkipuswb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rbfcelou.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xzqysiuq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xiflwrgf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vtpztsby.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3nexyhupb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zwwswmmk.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wdyuhmou.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tufhqwfw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sonbkexm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fdpvgbkv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3qxbojfme.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rpygwkgu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fxcilknx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jisxzmbb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3luxvoxwl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gnimgnst.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3engqgtrz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dkqclkqj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tomjsrah.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oqzjxohi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xyfndxxn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3tkzircdf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kjnscbos.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yxmghypa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kntsqpxg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3hvpfvjry.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pckkalzw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3inriebca.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xnkkvqjw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gdyizuel.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3avndodnb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qbacjuim.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xccjfxvn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dzsbehsz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yianufyb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3lhyzxnzj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3sitjprrp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3thzkmhhb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3hfrszyfh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3czhuxouz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eclqvuyg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lovydees.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3waowftpq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3nezgjmkb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nvbyiszn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3eunhmtit.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exillnqw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bitznjwm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3otiyvtlh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kkykwyqd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxdsoxcr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uvsvgjtv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jepdqoeg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xkefaeyn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ddbjfjnd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnhzmdfe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rigkldwj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vxwpbhjj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vluxguvd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qofzkewl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wpkebuzi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ebxxmhji.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uezhaemw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yjqnmian.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3icdjfcji.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3bejpfvlh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vazrjzvj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mxpcupeq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yiwarbxa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3cbealsws.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3cffctsyi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3inqhemxs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ppfimpwc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3tqjibyid.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ggatvkqj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tieiwfvn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3vekxvcwf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qppixahi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ndhsphdq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3rkplqboj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wqkdktbj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yzyylqjv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ycurdvwd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xmyvaetl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zswdnaho.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3afrcihan.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aisgkayf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdkvqco.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fmajdskk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xjakaana.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kfmzbfhd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ynuccdap.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vdgfshuy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krbzohuv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mecdqeuk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ujfgrqel.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ldplcbue.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tvvsouij.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlohloua.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3sirsuggb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xirrotsf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pzyjqcol.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pfmxkbsp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bakgpwwh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wbyybaoe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ncispvek.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xxoqbqty.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dbkmrqhh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3emxrbomu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3lrvsewce.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3iiwfggsc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vdsfqsbf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vluikmwr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wufzcwkv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oyhyvoje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3lxhgtcxk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3lfsnncbb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vicrxuyw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pindpqzi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eoaptnbu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yblgphbj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3druwcdsk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rsckoxlp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxsgryv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3obiuyfcb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3npbxqdyo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rmojhufh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xvcihmkx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3otftyrot.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ulvwgtfs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3shtjrcdy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zzigagpz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bouzghhz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aceddkkr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lssyzfmg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eoqdxhlw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3krofhcvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhlgwirh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qewgibsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrjzyiei.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vyjwqnrx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fmwwohpk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3apskzwvu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hgibfldm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bxgtkitm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vrhyatmv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3slkdoiai.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vhmkxepd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ukbcdoys.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3quqgqnts.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3toexxaeu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbhzceaf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wtjhqjqh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jpltohpi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rlqzoihd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3umxitwiz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qqcezljr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zcdjyrdy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jysnqxci.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pqrlkffo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3szkyxypq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ysjvjbbh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dkofzyjy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vdmauobg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bcauwxmi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3octjjtue.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ihjxkyze.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pehfujzj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zxnkoqar.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjthbsba.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rffrsqhk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ncvczsnh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xboopsxe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xgsykcqs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3axsbimki.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfmskydu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ejewmicf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zuzroosf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsbpvdan.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sewooiuj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzyxldym.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3amvchkey.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sneadphw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tnrzqmtz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jzgdlhyk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dimpslbn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sbtkrgxk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjvxsad.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fnrazlji.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3deczgfag.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gtindhet.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lrgfvfpi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uvwalilp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gfntjcpu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ezeisvsx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eqsluanl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqrjhh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjgcbkzb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsxvulrs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vvdvthkg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qxfvhupc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yswioxfj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vrumwslx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3durmvbie.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uytsjjfw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nrgvfkwc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xmlwoarx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nehxdbit.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3chheasoh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cavgqtjo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3riamsonx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hzxrgmlu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ulcrvlcy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3snrtirrb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3emuvmsgf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbgtudef.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdxxcgza.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3liuqakuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kydrwqvr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mxowdyaf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sibkxchh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3azastxxn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dmdmjcuk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxcfzrab.html


<!-- 参考信息 -->