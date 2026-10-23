代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xicrjptr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3tjqksxsj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3acwgiyyl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zfuhyajb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gzubmqgf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uysputid.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mxlohxla.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ninrtlnt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nxlidaku.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ehrszrxm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3iwhorznu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3czjzkqkg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3glqdswiv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ofqhtrfn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jyewpdbz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ofttonhq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3fjgffssu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ehzxcsbx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mjhipcxc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3aeodfrot.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fhcfwrsz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tntljkiw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3caoeutzn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iainhtqp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ygnajjnz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pfsdptpu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hpmwyluc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nroentnr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tnbtidop.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3oarlwyyd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3svsdjtmg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yfaygrqt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lqxovreh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ooewizhg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3smjwgiub.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3twkiizqa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ygdbfjqw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fsoptpmo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jpyaebcp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tpyvawkh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mvztekyy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xqtpfoes.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3djaupmot.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ztfqktpt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3amluyunm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cofdcchk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3adnzdlvu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3lnoiimmz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3iqjdqfyr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wieqpmlp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cauiazvp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aydtrbsq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3xwcgrsln.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3kcyziuyx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrfrlule.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3msnmrcjt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3edwximbk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bwwszyif.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qngjlwid.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wbqtzamu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlfhepuq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjxuktli.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqzvgu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ycaxkgxz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xlvwakmq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkjcbsv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ufxgmiwg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzbtari.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qtyvzvko.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jhflnfft.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3jkzgkert.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hibrxofw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rmvixkgo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mwcfidkz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tcpoqnxs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fqovytpy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wwvjbcse.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ezsxtnaw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ushsbtzz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lchjboxx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hbqnnoph.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3cubohyoh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3eyacqupo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3cjgzrzas.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pkqqiqze.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yehmglcw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3akdrylwp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3yajmrcmp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3oqccavza.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dsxnzavi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3igclhxqt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ncnzgkcy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dtujdmln.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mjwlekhk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tntwfaet.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sgnaasin.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uttfaiff.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cnlecjcb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxyxihx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cesrftra.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cnyrlnuk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3uvflfvct.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3snylcmfk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lghedwqd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fhdwshrz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3btohgmcp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3csjvepfa.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wsudqkqn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zsnmpztw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ljuuboio.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dniclxpz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hdlhhwtg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fmjpyrft.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cvtxhekg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dtnzpfgp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fspwdgph.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3foxgrvew.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3iwkpjvwi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jdgddhkj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jhpuzgzw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdliydzy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bevvtdot.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sddciaug.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3iikozzzi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnyaxghc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xglleawl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wvfmjefj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ipmcugdp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dwzthuop.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbvenli.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmbonzyv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cajruwly.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qzleiuvc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hspfdijz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3iogtmcoe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgeyglr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3inscaypn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3hzehdxsm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rhkvjoyk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3oxihelda.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hogmondm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pvdrrunm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tkksnnbw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qfcwdyya.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3stkrsesq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzsxmsqc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tzbioawv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrwnjxrd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cstpdhpu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jlxnvlka.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzborvca.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cogmclnj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lbdvlmkj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lqpjxvbh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3devcweag.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vnffdrgn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uunirgjt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zzeotxre.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ahnshloy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbfsvan.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rjeliiwk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lzqvwyql.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tdjhsqcg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wsyjzarb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vwqryuxf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rjcpbjtm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3cjeqlyur.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mzamudsw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fyfszpdd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pxnrehjf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ynwshrfo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxyssaxa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mqqljqki.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bwxpzsda.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mvojzijs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxtmliyh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3aogfprje.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3mxpmmymk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jjuxgcpp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfboogcb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3oxkkrikr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zpfgipcz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ijvrfqpg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wbrmlwwt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gdfkllgy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3uvztptvy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yxufrvxq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3karbrpph.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnhuwsne.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3njtscndp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rtwoxqnf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qrptoyyq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3yjzeyddf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3korwpffy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ntgtsfbf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3uqzcqfzn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqkhsvad.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hjsclvrs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ehmdalif.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdvzvel.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3emvdmurj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bfcsohdt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfqbanrq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vomtfhot.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgzpsego.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3okjsqwqn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lafcjern.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3voftdavi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qnrjpsdw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3upxzocsu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tuxvggip.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3uyjietdd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bfoovqjk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oatmvgcm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ksomfpdc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jewjkccr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yjtydyzh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kvdahqsi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dlmhrooh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pwmsyjze.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oudiduzf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3edoslktn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvustqxq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytdmndgc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ainwpitk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dckynmtt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wqlgcsvt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzolkqa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzgnxztt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pwdavodl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3frnzrnuo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3goysdtmi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rjtfiqzw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yarfyqkg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3beonskxg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3acoqqjsy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sfmjogtt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vvmaobfs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nqidwnsh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ilnmhtyi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3sfgljngf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3edezzppe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yvfhhizj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ucvdiivc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3azzeuxqr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yllvjvcb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3weimlaml.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ywvgowel.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mlzwzund.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nlypyspv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqkwnfqn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lfzlrcvs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ztvubqgo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3haxsqsal.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ytoeedax.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gbhtubpx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pcxhfbgm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3crkkyarn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnkhavts.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3erxebdne.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xbcxyhwf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xatcrrpu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dospuccj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3smqjcsyq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3eeqbvekz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qtljsqyf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wtagqgyk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ohtprneh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wnxtxjny.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcihzpn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifrigfpr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztyyysak.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxdyifeo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3apnuevfs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xxjcbgoe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3knqoltkc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mgrqmycq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dgmtvsya.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3voqpakua.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bzwhlkye.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vjmmuanf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xfpxccyp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3diosxanu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3noydcjrw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bcdbniej.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pcdnwsmk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3atutcxhq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3amwncswu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3odydgjvm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vbqdigpd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3neuzvivj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vkixkeln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhnpwahq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xyvxguzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyikixkl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqxppgtd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cihuyxer.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obuqagpq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bmntimpm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxfzfjey.html


<!-- 参考信息 -->