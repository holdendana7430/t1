代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hiwpylyd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2swvlybox.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gqcjeygr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2asgjitxk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rdttnjoe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iazntrtv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ihzthopo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wqvclizz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2diyjqqzk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iptxhxgu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2esxuqhja.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xpzaotnl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bpjxsmbs.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zwpmavse.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lwmbmvgv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2fqnqizzv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2meejanbz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2beepvebt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pnezrmck.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dbcdvrng.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2csupgozw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uuuvxbcs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tpycdfay.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pjwjgjwm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ybukwwhs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tvbzjbzn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gyyygxcx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jixdzczs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fackmlsg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjopglx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qytcexjb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clbkezjd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ffrzsunp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ncjairct.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2oeplcxai.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oxgbkslr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mvrifwxn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gjcieqto.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wwmcqvdx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzfotxfl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2czysrrzi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkfysmzb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kzvykpua.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2wbcxjmch.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2usjulrkq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dsplcbhl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2bkfodivu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2haitjxmw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nmkuxdvd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zpplklrn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ymeamfld.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2llmutsqp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lddyxtun.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yewvlwfh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mjiyzmiw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bsyslwbh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2sltvwcyu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hegcvxoe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2krkbzvvr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2kbwsqhnb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2rotwglks.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hwcjraxk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jcdfwiqf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kfloawzi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tujpglyi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cxvqtuds.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rcoxigxp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ilkgpxti.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wjuwpcdd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xagvnxew.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lpyrsobp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lvjhmnka.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mrlgrxco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2jtuaczpr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2odhlehlo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sqkpkbdj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gzjznmiu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fndgttua.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xihwpoxw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2khenexpa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zflquqhj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2puvsdlnp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nhqqejtq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gixmanvl.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pmjyzzrh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jnyvdrdo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xtbnnvwi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2upgenawc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hhmjhevb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uyxrwgxz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2vhvosthn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tlkzhktr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2uebzfapc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vgginyqp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcixkvsh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfqoztkj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2cawmpbro.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mzxfwgxg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2giwxvksi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tgnoiwlu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sxvyxadu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkqbuyno.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nkbhmlza.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bybllkag.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhenvhnx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eqqjqdil.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nynilkje.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbuvdteo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zmwuofsf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjyhsmq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bdxlonrs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nlcqjlyr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dopvrtaw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ygjlwewy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vuukspgt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2wwuyggfs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pzehrmgu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhwpyonr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pesmlmvp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2snqyzggq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fayfsoxg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ibdmwvop.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2mvukqsqr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ihyirxqa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hrrhxfql.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2yxvrtojl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2szdtjiyp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ouqlxyss.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2yeneitop.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rerytmzy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2xhlyhwvl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cwqbznal.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2flgwfaob.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wguxymzw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2nufrhngs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vlpvycpe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhqoojkb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2orchzikf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkappgzg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfcgepk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bumzpsir.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2icedaabi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tlhnghvx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pllknzcq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xnowwicv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fussntgx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2mqblkdne.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2njxjofsn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wuodnmxr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pormgppk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlofbwwb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bydxwxrh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jabuelsw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zgeuoykp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2llzmrxom.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gcmsbekt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2egvcklkp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2belqkykl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uakclbdo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hrbzqeof.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uznymxms.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2calgvsbm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hsmzcpbc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mhnfceps.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2udiiicdq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2chohrfdr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fcjndile.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zxdtyktd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2blzkaobw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lhhurues.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ptnsyjau.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qifrlaix.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mazpxrwy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkfeoskv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkkltdn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpixapp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqnscpgd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sirwfutc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dzmqfwhv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qunsjyuq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xgwlrvgb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zepglnmn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2netryzfr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2daicssvt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ewjvkxog.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2osnqndlx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hjnoibms.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ubjkfhjh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wbfdhsmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufgqcpaf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ifiapqlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrobwxcx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ceeemgdq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wglyanji.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hvedmwlz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bljauzlu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2waegfxqy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2suwhdlpe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2noluadps.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ggjzeqlw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ycfdhibk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yrodhvwi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2exrgrtdn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2etjtutyu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kfjgtwei.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mhqfpgqp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cprggnqe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2shmurrhf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jmkodtfe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jykoofvl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xuhfqfqm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kysedads.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ubwesvtw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2obtyzulj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2joagywdk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pbfsexvu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vderhiot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2anmorocq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gnewkrlb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhjeorfb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rnidxwsg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuplljfv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ftdltkqe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rufrsoot.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqvgtnij.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2hyiusahm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mwygiucm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtwcxycu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tdjojmyu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2afxmfctk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmkiopm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnajyqmv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jdbozhtq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmgpwess.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rtjhqcpa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ysfmblmv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qztwqpao.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2spdjbafm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2eisidefa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdohgxj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmawuzzw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2szuppsrp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cayoclyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2capphrbb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lkufiowz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vqdutddt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2npiigfvu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztexanni.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nosjhqni.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcoehtcl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zibyoqer.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2djkyezxc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2exmzaafn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqyifyrh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pitdqfli.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lkwzqqmi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dbagttsh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tonsiwoe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2adpnpbia.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tijwivkx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dufmjpmo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hbkenwut.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cmthwnqy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rzjenwye.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jurweant.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vacwtsmk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwlmmaz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vmxtpynf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jphvkwje.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wuugfuct.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2irrwspfz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fosmkqtp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tzzneeuj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hexciffm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jutcmzcm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oklomlvl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cdvapejp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cewklhaf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tptilbfu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2udxbzzpm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ddrjyprc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2difbdupm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ppjjupmn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jliwsuxk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bphbpwoi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qwfzbbgx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvjjgtio.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2accalhup.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2owwfcamy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tuzzlxdz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdxrfwvf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2majkntqh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ofjvstvo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nbpehfbk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2revxenrs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dgyjtrha.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fxkbpfgn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2chokkcgc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dzwtrguk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kfnocqqp.html


<!-- 参考信息 -->