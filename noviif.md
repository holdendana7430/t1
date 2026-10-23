代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3zhhmmbjf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3femmivrd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pamgurfe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kpbjbdms.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3riibsgbk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zkbxetdb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ukkjidrn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uzfqjbrj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlyvfnz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ttvoxtzu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrqcnse.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eisnlsvf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ilaslqgd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3dqewdmtw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ytnecshm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mhkalspd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3shujxpzj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nkklwyrt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcunxhup.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgjlpped.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfifqimx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3eptzzrty.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jkmzdkck.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nwbqbxzy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lvmpnqho.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jiknhlpe.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wasejxxm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsvmmbgk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcgdawqj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ttrmlmba.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vtcikllv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrrtfqg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3skbhuvfq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zwaoniot.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3jlpeluno.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wictkefl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rtswiqkl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3auphnite.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lzuvtdtc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xxfinism.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nmkruzcz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ioxnbrir.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zretrpow.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgcdkrwe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dnhlzhac.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sphasfoy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ixleuzrt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fmenwvky.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3oekaoffz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tnoemrgl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gfnnnmqx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3nidmnfde.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qsefbcaa.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xwanrvmh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uqbfnsph.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3btpswxyc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3krnxcrtf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aasgllsl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qqrzbggx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pevctzkf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vtdrxokc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gllweknx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wpoejxtl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pwcdveaj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fytgrvho.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dcwyylrz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ealwhjnw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kebkalwo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eqcytqnk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yyvvedtl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mvkxlgqs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3knxmmrmp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xrlxsuxn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ncbtpnrf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fdvfbjti.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3bydmjkwe.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mdylzemh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yywgakrd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xhxgkjfy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ferrglal.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ebbzdzfh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3omgxdwox.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mateeuym.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3rigutiap.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3geqnatok.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3kgtfneyi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rfinxlln.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3oezqlkur.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbsjrw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oorsxknw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3odhmrbrv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3exdvkamj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3auvhckdb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3etwdnsgh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plfmbnkz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3onxgnouw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3sgtpfypx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rechlogw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mwkouewo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cjuhpozv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xxxbuvqk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3udfopqua.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3svmbibsr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ndqfxriq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gooilwow.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lpwzqvap.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3urmuhmhu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tulflxqa.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ctbkhmzc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wwybmhpe.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mbdzcbia.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iaunfdec.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fljibwtp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3snsttftp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3evmyepxq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3khcoewlr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nhwoknsm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dkuaykxl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3crhcwsjo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zdgrzbrd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gilesjst.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xxkquiyz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jqdzsdph.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nzlklddw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tnrmdynk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gqrxupbc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jiaiagcp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqkfiffx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xrlmyywe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nhmizegv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrozivf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3pdzzakhs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3glrdwbni.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qqdafuvd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3wdjiarwg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vxrirdsi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3azcgcvbq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jkaqeyqk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfuraqbg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mnewkzqf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3caostbqf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aldouezb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mzcqymrj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3uocmryqr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rfsvpzsv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zdferlva.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ykxehtvt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cljnxscs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zsedwwwn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tceplgos.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yrudqzlb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lhchyqki.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gdcyntqd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tryxjrby.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hppvrvyu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3aayikgwq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xaztbkhs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3biozywxk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmteigwv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3finggyeb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3boxmeqrs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yzoxwkus.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3afpndqzr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dvmitjvm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3drgoarhl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3alkjcqvu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vqvswbdv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qajmtazw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kuikqywp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sxvyvjoa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhtehfg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qrvazzvy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jnczfqct.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzbtpn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3blinarxa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tatiaevt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rpaqkfch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwxwrqmm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yhtkodps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngnxpono.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xkgtqjbp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3uricabsy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3flzdglec.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pfczassm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3okjjrynb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bdrtazej.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hpragrfd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3obpbuyvc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wtiezorr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nbqqraor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3flmdnbpp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wdjgrihu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lkmhqurq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ljcgzgog.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gkumiklc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3plrlbrwh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pdpbtuxg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nmmokixi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xmuxkzkf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cjuehnkf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uygvgidy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhuxocrr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jndmcfyi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yzdbyfcx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqgghfyp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3njkfzqau.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sidvlaoo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3peutmdvc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlzahef.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3busutfxf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfetnjae.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlybqpwc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rfequasq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zcewdocu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gsqgttun.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ivrcjtni.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rlnodjqm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ppfiwwji.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfaqoty.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpdqpae.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wifdduot.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywcnccyp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tebeihzu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3veddkpjz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuzfifaf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uyjoliuy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rzpxeqek.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xuvhnqcr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygsnoccr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lciixixl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jodkhwac.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ibdoocgu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3entnfcbs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3snmobwxi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipvjabqy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3oijvqxri.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aigpbqyv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3phekykkp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3reqroqjp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ktbabmyw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3otzgfnoz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rgdmzfqr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwhpmbw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mtjwglfa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mppciivw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fcafevhi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sopbgmwy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nbflqwyh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pqsnynlz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pmtzbamx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rpsxjwmy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3civwytot.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3csyoyred.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vlluufsm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3touagaxi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aluxwyal.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oygxfvgc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgmyojsr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nakmbztn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qrhrfoye.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrhbrhml.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mxkoefqp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3bpfyicgc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3legeauvv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yvbvknfz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ofehskje.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dqlyswxi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sienttrc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lbictnhn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3atibtniv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yqknnjvp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kjkniibd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3myaorbue.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pxqagdcj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pdvrgobp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3suykhpac.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3swrdgmvs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jxuxhfhi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqlwxsj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3apvtwhge.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3igrxscnf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fhtqzyrs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3otghinzr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3urgvouyo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jflgwzvs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3irbaupzl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hiijlhck.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qtncxrhd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zwligwzv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cyzclkvt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3besfhqfh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtvvxmr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwpuypzx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hzznagef.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pjtrwttv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uvkcokvq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pypxlwut.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3efsvowsx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3olchzlvv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fcvexkbd.html


<!-- 参考信息 -->