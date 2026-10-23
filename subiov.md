代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pemhcpkf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sllzzucc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gqvtpkkc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jctxewhw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ztsgdzso.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zkduatqo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3fkyjbzzr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3esqypbfu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3cnagpmhm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nrffvpmf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pxcwlqps.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oejmezte.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ibrbwgao.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zigehhdt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xmwmbflc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3imsqmfet.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xyhrogwb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3epszggho.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwjpyly.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uhiyramh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dbgsapte.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gnmfelwy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mvajqpcw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dhdvfchz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3evebtmwj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pbludulu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3uizlgxwu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3brmggiev.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cgplcent.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xhuddoqx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kitsqhag.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tastsalb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dccfabil.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hwegflgl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ivzuqbvi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yhtpenhk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qsnmoisf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxrmvwu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3lgzkvjpn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3afgmieac.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ywqkilgh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ippqjgov.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkswweb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mzjzemge.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bgxoxhxr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yxrlqall.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvkyywjs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqzrntqs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fbchnpym.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3omqckpas.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3wdayljcv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zzmulpxt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vkzomumd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fojmpufc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qprmleny.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mlangchh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uouzbmjf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mhrkbcrv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3tspapxjl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vtjgzpdi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3uiltdjeo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3sktjiscw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3nrsqnqda.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nuxeevjn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mpzcxqpu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lzpplfhu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yprhmtgk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3irhimyyv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3srgdtvho.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3frtxvcbl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3byhfqboc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bhqmkjiy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3atfhimks.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3quhsllqs.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nxbmhccl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3krzbioxt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3htyzkbod.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ckxlyojg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wuyyzttq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rpkvbitd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wnfvrbal.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3edcgunmy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3apatetcn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cbjzjvyh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zzaiuslo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rvodyiok.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xxlldvyp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yukffmxs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ykdyhyej.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uazabdak.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3muhfcfee.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dizzaawk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vxqbpfym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3gajjzixu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yxhyrhbr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3wcqxjppb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3klptwcze.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3zhjtybcb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rrddjday.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mlahrgaj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3piehosbf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3psgugzed.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3kijtwrqv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3tlklalfj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sozoyite.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jarujrki.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ittkxbjz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3stnmjfxb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3cwmetyqp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3keplyozh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvbuczyv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3thkpeeev.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3pwbmxnwt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3quthatem.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wkltqhrw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ivwdriya.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncpdnxdu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmugjvkc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdbauqtj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3areznxtc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3phizgjln.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlsfapog.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwkdddgt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3klbwgclj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xggvowjf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kidrxwkp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3usshajwq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3iwwhstck.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3drzlyfop.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ilnememu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3bmlpeiyp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xasvxcvw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3douqxlfb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyznerbf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nxvupvqg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3isdlslki.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3edrcakoh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mvlzhxoa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ucwddajd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wvinekge.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rrpqsfpf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3wckkbavl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rqqzrejz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3anhdrahs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3esadznag.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3adjyuwnt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rzqjachj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mwdfnlrd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3cltjyqho.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3whvcymgc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lpffsfbp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3hbvqjzqu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsszgnaj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rdfddozr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bsoncjyy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbddhwwu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gpmpguqi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pbotmpuu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iueekwlu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3nqjlmohj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvkokqza.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ciwtnpad.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3preutcnh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3anybtvrp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxnnxpcd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xkwcffam.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3juaujhls.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3muxyukmi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ydwrkmcm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uwrtwier.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mkxlnyql.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hpuqfhcc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yhmvbdeu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tswiuzkg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rhvcjcoc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3shepfsdi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vhgelmln.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3kbzjqybw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hzvcwuok.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ogmhrnsa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqntehu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cvkupwkx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dncuejoy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3oqesgdat.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onjstxjn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3uusovrcg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uaacbzfr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbpkodxq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ymktvilx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwiybfur.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dlmwglqc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3adfuywty.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlgeias.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uolyuuiq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wbbzqvrh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3luhehbsa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3czmkkyku.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dmlobvll.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tnnimyfd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uertlrcx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3psniydrg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ryhzzcno.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mwirufnm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zskptnba.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3olawlixm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhxzxckp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3slthosog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qskykfch.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gcedrszo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3mgnwroup.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kedvqmgz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3udwejhaj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uwvlryht.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rkghzcdr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zcarjwle.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3adevpmkp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lnspcclg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qbrjmyuv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3waynkftj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmbdscx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rfbadcfg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gcyngbvc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eshafjgk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cellkweb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uktogbte.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3skbwvjjr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hbfgeybu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3faumcpkb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3idlyzapm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjpvilun.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vqlfrrcl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ysxtcmao.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yltshffj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pkqdbvje.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mnlbvcvs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3snahgthk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ustqorud.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrwnsahz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lzzycdog.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jiiryzyv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgxpuzww.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yhkjgirr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3noqevqtp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tumcdola.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qubxaitr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dieaosxg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bclhmhyl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ixsguxrw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kanlnkye.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fyutpsfu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qywcdvag.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zzbzydsl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcspipsi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uaixnztr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tyoepjja.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwurmhot.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxzvulc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nromvwtj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpvlwyxo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xysmqrnf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqdvacfv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zpwrmdsi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewkkanri.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rowizlnd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gdicpgov.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mofnoqgx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztsvxnsg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpzqgpl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gnxjlmzz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3buteurbc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyemeqwm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kojjdubt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xeqczlzs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tjtvugdb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qcfeljgs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pypkufhj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ovmmhxoy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hqlsmmsm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3frtwafhg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qajjemzo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xmrkrtzs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ieteunbk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihsgsmao.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3emsocryo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3efsjkcvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjllsxm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ojuauqlu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3owhyotmk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmjaaumx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3huyiohty.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cxmqkpkv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvpvrznw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qfuuggoz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lyegxulj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpfjigdk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lqhxodbx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mtyybtdq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfiiurby.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3uhufackp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ouuaydfp.html


<!-- 参考信息 -->