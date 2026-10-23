代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cggadayc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pcbodgaq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gipttimb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxcmknx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wndllmaz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cptdlatz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbgzvds.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qcwkbrfc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cspsptsk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jzzrtdss.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvpoimi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uldfnpan.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wdcgwkdi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xelfrtwc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fgchblgk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzaazppk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klcxxkug.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vtmqubgh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3jalzewft.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mijxpsey.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3wxrahqeh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxbuscy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jqzchjyl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkwptsne.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcwnrynk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nkteensh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ephkkrtl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3kbvnigen.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrvcjdn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3sduxhxus.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wyofuajb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pwxoexbr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3actiawjm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dgnsluiq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3neykugtc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3cbvlyqoy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bmmzauyb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qouocwlm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vkujsiyx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3eepkband.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzceorx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xjnbnbox.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vlmaluce.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xkenysdt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3yniknefp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3aajvxqva.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3knlvuxqd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dywqfwhe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hxvdgvom.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mqfbqyyw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kbxnkfdd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qimomrgp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eudsjfrx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rfvlftnp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kzyooupi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wxfxbdaw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lpudwyxp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uajuerap.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gqmzfjzx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3foajoojx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xkcduniu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tvvasiyt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qhhcogil.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3edgkkaos.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kbxlqund.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gazogdzb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kgxwpgxj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rzciecbf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ywyxwjrd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3duriroqa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vmarwwbu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3pfldzyvb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fwfbzpfp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ltclkghp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3cbkvdacf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yqckchic.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hjxmezhr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nweiappx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ojachgog.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msjzcofp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3aascveqn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3yjhenusa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtfllfzp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zwkfolla.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayetnzsn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krxgfgte.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3koolzoye.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlpftrec.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vplikavs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dcwvcyhu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvcifptz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xylvswqb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3kxtiuegv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3awcqnzyi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zkupfcwc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3plybqgun.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmgxyry.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lywhxoev.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3svaajsyp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pnrhjlzg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jmqqbjbr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwswzhal.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uefhrhcu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tdlmkzvk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zujdjnhj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hdgxroia.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tlradvim.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3enzjzjqp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ymbkkyga.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uafuchow.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xuicwqxs.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3iycycpog.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3umgzlrjo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rgxmlenz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fvgasead.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3aopiitvv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3shkvdcdj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pqdncxoa.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3pxnyocjm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3hwdmjfid.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rofxgbpd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3knrcmadr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3caenwllq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyeikvcq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kktzlsod.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dzdkxrzf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ijuuvhgd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3aasfobgq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3javarzrf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ksmyrldj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3bujeuetp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qpcdbnji.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ydbkfjgm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zthmjvcy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3meriemcv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hodhszqx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zznxuhyh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ysrzkqqa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3koodzrnq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lmnehejv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3csettpys.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dqpzblrs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mflyceev.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvwsjwzx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hlzmnqdp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vobgepri.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3mgwvostc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3reddnqzp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgisatv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3btuernoi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vxwzbwvi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nvbaggeu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3daojreoi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3tvvyhzei.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xdqoagjj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lfxtfscq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dybdeapj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ofjvekpb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yljvyded.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tvwpubpi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvdzioje.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3czqegvgy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ahqtguvs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3erlklmhl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qndjpnva.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cpbsnhya.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3uayzhbwj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3somxqxwq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ojqkvtkt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yumotmkr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3uugavdbh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kyclgsza.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3doamtycr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijpkttoj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3iaojqcih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnmtmzxu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3muujppks.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jyfdsqoj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmkddijc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nbatpmhv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bwdhodmx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lsdmitjx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhuerbrc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cuicuvzz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3elkfurks.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vkxmqwkl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3oxsdzyap.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3yqdlybjc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ukxfjrzg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hqpwxzul.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3blxitnqq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3eamznebe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mbfzhbqs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xzmumibe.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3hjrxbrli.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3usiwggth.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iohdjyvv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3momzfiyl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nyqugtzs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsskgprp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3grmrrhrf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3kxximqvy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wduncbsg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bxdhifar.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3tsbttqyl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3sedyiyls.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3omwmotmp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qzjuapyg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mekqefdd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kmskfsru.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qzjzbycu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gsucybtm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zwjnjvly.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgcwfyl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3awtbtkth.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjrpkcnh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgodazit.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3psdzslkq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mzcqefcb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jiuljrpn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjbsglfm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hxvmxngz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tnedtyju.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3veeoihys.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lwtaffdc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbyyzloy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3imaeuurv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rubknrrl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ytnvlmdm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kohiatez.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gxcmlpbz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3iyhjwwlv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pzufsord.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsjbkbfu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfzktrv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tqqqawtx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qiuhvdso.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rtfxmsku.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3galrkrfg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yskjqntf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wozqaygv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qwohlift.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qiwlemcm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hbbaeisn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mrscqyfr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fgblgwqc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lcjocxzm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mssnsxgp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hakpntka.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sphktufw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nflwwugt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqdmkjip.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkrqhwms.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibqduffr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fkbxlfxw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3egtwdlbs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3waniuaoe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ubopaumx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3otsuidrn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tebngpxd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mzphoflk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lotljvwg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mblszlao.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3yvvhrksm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3blvguuuk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3puhydrms.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3iuuxagxa.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lakhyczl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3unzzsxkw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cthofpyj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ootzmapk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fiakltch.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pwmfedau.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hgodzibd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qbpgykes.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wohqivka.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wiegsnrn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3uayvsxwa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3msncpwby.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3balfvvwa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmjabxr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3himbgigl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vkzdfedu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gusjqxxi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ugfxetwc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mwbynbib.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3supkbrnt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbgvrocg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fwwctcan.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bdylbswg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uhatqoqh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tbclubix.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gwxwnrir.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dmgvykdr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3douphoxf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wfnodblw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdmommbe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrdzxp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3euufdlrs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wghrxtba.html


<!-- 参考信息 -->