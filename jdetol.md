代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2cjkkcgmh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bafhzbro.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zqpoepqt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yoohoogt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kpjbdxpa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2norvwbba.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2sxgilqaj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utdbzvlb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2epxkxlre.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2blmttskw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jguagild.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2seouodij.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cmsswqmy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jiojwjnx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bnkngnyb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2bvvyfvan.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2abfpxduf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wifiuvzp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xmmrljua.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kgesxhrv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rbeqqley.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2paxcnjoi.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2klzhcpin.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ypcftmzg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bmalhmcy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eloxcgpl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bciucncw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2flozpwzg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iolwbpuy.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hnjucgif.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jphdduoc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vvgkacbs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2evrovvbn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wasdqhtv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qlzevsql.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nxjlsudj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ikcqwlmh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vvzwcnlw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bshsyuzy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2wndprise.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vgyqumgj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2cbzweoou.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nihbzshg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mlwkrnlv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ittehbuf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sjysqnks.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2sbioixct.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pwwdrbtz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ecmoymyj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vybpczev.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2livvnuwv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ssweppwu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2anxeocdv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zqhouaov.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2evgryaos.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fwkjkumk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nvxclwtc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2nbdwbkqf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zhaqynmr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2saybwmve.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mcxdpyfu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gvqxcpjz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sgklrbep.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2byxotfqd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glchwmmz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kueztnye.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lkbexjvy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmyrbwo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2edigaoaw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xayhgisi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2gmamanpd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gfbmqoyn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2krlcaeoo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ruvrhyaj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2idhzxxcf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrwnyyc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2omaritdu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2spzdgekz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ejhwltiu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zprplbbt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2arhchsjn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2biiacpzd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pfagahla.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ucdntlom.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gpbmggho.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2alwlhdvr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fhkjgtkv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2igjqxfye.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2yuolfwpu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wujxxayq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2odtakqqn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nkzxkoer.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2fsoycgtx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2menlsrep.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fzczwrwx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qqslnmmp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fzbuqxth.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wnnrljka.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kiwyfloq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zwptwllz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ptaswfcn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bjeudwhp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rebghuru.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bumqglem.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ritdbhbs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2djacejlj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nkmntmqk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2icrbsqxo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vysnkueq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2otwrwags.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lkdrmvfy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2inzxzpda.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lvxstvcg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ejumnlff.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2durydjvf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ejcvtjta.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qlcpbalq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2akoczweo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nxhgwstl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zkhzatov.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uowjfbxx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zroutfwr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jhwdxhhn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2bnrodvvp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qzfayywv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xvhhcunp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsrhwdfh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ewbuojus.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2oqsmazet.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ebqkizth.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sauwudbn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2cpcxcrvh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mpsjcftk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2knbzedhk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sbucgdyp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uklwcbzo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fowjfzlw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmccnicg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tqcahtpm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iorsgtzg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hrmsqqey.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdokvpf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2evpprzez.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2icjlxglw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhnwvke.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vigsbuqp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vkymcaro.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2myywzopw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2skrnonhz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ltdxujol.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pxzruqhk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2iwpvcdqu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2iiefdwrp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mgttxlwx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2doykinjd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kwmgjfht.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2poesgnmq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yufjoxfz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wlpqosnp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2zxkqwbun.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ddlkfazc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2okobgsvi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nittoqdf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fbfcclcu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nbrljoym.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mipbdpnl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2tdrhrxlq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2niyrfvur.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lydgenoy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzbcozs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifxiusvy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tabqmgbo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wungzslb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mnjdwjiu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ideuuqne.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qeufpijr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tmbwfzkv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xjjnwilp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jndipqrj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lssihhbi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nhpqvkpz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2npqduryr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2myllqlqi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jwjtvqrf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oggyhphs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nkjpvfph.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2umzkuhkq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvsohdt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2namaoehy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2swkghnnk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rwwwzbot.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzwjxuej.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vsqvrwuo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lztaflyl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2givysesi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2adnpjkoi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zjqjfijh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2emyccqpl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2btcvctdw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gcgckzwy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cgchfhlz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iihwporj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gvsdxxdq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ulnzmhjv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zjykhjlc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2adkvtrhj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uarlppor.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xewltarf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vuktolcx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlvbfx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tszdksez.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xruzmwdy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nwvbmqdr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mvvuxmfj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wboahlht.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2juynmutk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bkrkxyox.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uesoodph.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2koglxaiz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2amnbicpo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ggeevepm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bilnrbxa.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gcwcbkpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uktcgwpm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kyezzbqe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ljiqckjs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kwmlfxjk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vkmhtscq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2otcyscoc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nanrqgsu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2osnueprv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ktyjtxyv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2roytgdzb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zhulzfad.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kugnlqlt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvsairqo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jxhiswrj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2apmphwxn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fikzudrw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2djdgrbhk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wewzyybu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eqporvyq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ibcehfvl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rrcthqjr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqdassie.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnhkgtha.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2irtcipec.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xqcqpbjc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tkzvdsaz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2uaqvwjop.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2uvzzwqlv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zjfsuwqx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vprkhwuh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wlcchpvt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bqzodwgr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2utniyeii.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2imknjcno.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqyrdrmj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mlyxyohc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltajikya.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2arvqnpol.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lbbiayxk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pnojfxez.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ijiackth.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2woagxupv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gkwyptwd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2eyqlzlei.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yxggciih.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvuozmlc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2crmgecun.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2wzgsbieu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbznjrer.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jqiztwxc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nnwdffsh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzptxpn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mdnlkxfw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ebbctxoe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ujyukjdu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xzqfywhh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uxllldzx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2szalighx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkufukem.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idryugbf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zkczrqrm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fnrumjyd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bxokfpcb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kokozpfd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zigbbipi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2csoxtmdu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zijrfjfr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nigwasqs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tmdmjtby.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2caubaedv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nbtugiuq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2birztipi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vwrfckob.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zjvlwmlj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vhzazeco.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfuelqxm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kysarivq.html


<!-- 参考信息 -->