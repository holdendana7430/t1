代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vhwudnrl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3czfcawgp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3cbrdxbyo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uuabnccr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nvovyvjn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3teseupjg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qftzqbox.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3hqygerdw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rcysxidi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jlwuklfa.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3gicpgfwq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3contxqrc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rpslwvlg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kketkdpf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jxbjwuee.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vaepevtm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3fwjcaivi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3yxzqzpoc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ldsiimvu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gvrvmqsl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tcnxyluj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3muldjnpi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3femzyuwz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qtwmorpi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rzmohyth.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sldxodig.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3olbkgify.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qxaspxwn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zsbiuajv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3mtmgwsff.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tpkmaxzz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hkgawxbm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zgsorsdy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3gpoytbqb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dhcncazh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3tsdffosq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dmxfeowp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ejugapol.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lkyqtjob.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kikuulnt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3okapmend.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rtyzdzxb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3tmvufcmm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhnkccj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hcongqdf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nhgdmuoy.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3kgvbabkq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vvrqluyq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qkwqqoxb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3inzderel.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xxolpdjd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgdtqhgs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ytvjlkwd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ynkfufbs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cgxkcwct.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3htkvfnjk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldpnzdkd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ihhcisyn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rudrvmdy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bcwxuoyo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bytgvicr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ipiigdfm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iwbuypwh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3prmwhzce.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3cameskrw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tgakudas.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wtcuafno.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3domltwom.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3elftskez.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dryusfux.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3vyoojawi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hwvjsumk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mgyybgsj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vaglbvsn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lilxvvhq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pwyukwqh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jtxmxwxw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lhzfmmoe.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3gljxiemh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ugmzglui.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rukbrfcq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gsvhpefj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3lqzabzar.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3lhmwtefm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hyfpffaq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vdwscfso.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3atovwodv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3yfmfrslp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3oayykuzy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hlrwkqtc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3mepaixzl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kqmfpylo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmcjgjem.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eqfkrfie.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbsjowh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmtjcxkq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cxlkqokb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3babgqmgq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqfowuy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cgusttin.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hwzisyyh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3crekorui.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3etuqrjcg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3dngrorpv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sxvxiihb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vhiglimp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjjyire.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ophiddus.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dpitlzga.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ehgwlqmh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vqzuzcpn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tnknrbid.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wyhithku.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iekptpmc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ikbrguqa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gpmmujsz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vpefgcnn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vzdtxamr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xjnfyevq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zujopqyj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwgvfdec.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hlcpcbyv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bbzfdtys.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kbabeshp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xgflxcpt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3eprkzehz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cywxwstv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lwhstzmq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mcsztivd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrfarxk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrtpknw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jijuycon.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gnrgixgm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qyxtqslp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vesqjfeq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3amqyfyim.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rcoidjks.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mlcugrid.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rjkndywf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fschjdua.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hxirjjzt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3swuekshn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mmtueqaj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3veendhkz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ztggzwme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeuczemo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3xrjfsaxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwlujawr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3atuswrxc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qnqcqapb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlcyheyn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3egprifsc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tqeumrlj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vtjhfiij.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eqpxolif.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gencghmv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rxwnucbt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3elgvnagf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3gjtggmpk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gzvgckac.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3djcqhvjh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wdknlfyw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ucevfnqh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mkmaotfb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3khnychps.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wswurdhj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tsufvavc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rjxrsvhj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nnhtxtxu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpjuekih.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndscyjjy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tdmcrslv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ghypxqlu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3icotpusa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tfwhtfmm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wgdvdxtu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hyzwxrtm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qtnhxlim.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fnojnmno.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kjwpsorw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyxebtat.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ljnycngm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kvdnfxns.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwilqflf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hqhqzqsv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mwzcfvkz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oljjnrzn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uworzqqs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kvxloewp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcevnaor.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sljqmobm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ejyceuqs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xqohtump.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bwdwcfmh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pksejpcd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btjnbdoq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3oxglcqgx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3znsgaztd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjdgbkp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jxaaqjdn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hxbpiccy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zpvimbke.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tvqoytuj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3oaubvgre.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3idnujkhn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vmglsbeq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uecuwcyf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cazcfwdh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bxrlimiq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3plruoxpk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ocdewobk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eykpxrgn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zwgcookt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nrvjbamk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3phhvfson.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oktmqufx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ldprxxwq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aghcsrsw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3scrkgdlt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zcpndojz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kqzotqsn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gzruoguh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwddaidc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3otfcfipt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3irzgubxx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtokwqyh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bkkonnzb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3llkpsure.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjhyvltm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ftjehmym.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zlhjanwc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpldncre.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rwqexsqq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yrxtfmbz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xefjcwrd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ayddjoyp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3reouovab.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbltyyu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3natlqumv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mxhwqaqi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nkwridha.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nvccjwkj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qziphdnc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wyxrrvxy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bgcxpexd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ohzheidi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kupraopk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3isrivrqy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3itefpczz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3scprmucn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrwyyrki.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tzidpzoi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pjfoaail.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3iunayhxr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uwieayiq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jtzznrkc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qopzchjk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lpazlmjk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmwmchi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vctofbsx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ohgycpbv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yvhhnmmz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyajafw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zszumdaz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tsuahadg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cqogumar.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3exidbnms.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3sshpoooc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vvzbtnvf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbdbukzm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zarayyfk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3dhrqipcw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxbixvct.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rkejbgvd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vuoevmmu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tzymrgev.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ayiuhlxj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jtjaqtnz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3flytzufg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3copmejmy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3spocxyyz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qymldjvr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ebrlujku.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rghhbwzv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sxrnkqco.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyyskkwk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dsagoinb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rbjyzwwi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vlwcalsc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzjwzfq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3baowwyif.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jtnzqssn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggtznqeg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvahdnom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3donmgmsu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3totpkjqy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cnplwnxj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xvztrxev.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmpcvca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gmquylvq.html


<!-- 参考信息 -->