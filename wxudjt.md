代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3acyvzqwc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3uclhvtbr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vbebgous.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hhgzizbz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hdktwhur.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bgefbhaf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jpyhhdqa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3loqgvegb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rbiygkqm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vpdfzsvi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3blajbrig.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3geiybzkz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3srkwkmxn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3doauniep.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3frgdomku.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukqtfdpq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3yvsnyjec.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bzmjkibt.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pmwtgpkz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3oytovxdc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gwsxlzun.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gdhynuiw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ehspiqnx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bcpxhqbi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bxwtdhuf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fvcamyic.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3todxdptv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xumkomdz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lfqflckp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gajydvkd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3momhrqrr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oqfdnbsn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kujnnugy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wuzieelw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ecgsspft.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3upjvzpru.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jqaadbip.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rgqxtmri.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ngepoaxy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xawtlvsq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dapwuzjv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vwzkddff.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nutrrztt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3pyhysdvj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gbwwinnz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cqmtfmoe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zvhpwrml.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xvczeihw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3earxbgrc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vrfyfket.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gowpbfog.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vlmzjleh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fzoftzrb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3phwavipt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuljwdis.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ucroddma.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mawgietx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ginukevm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3epqjyhma.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cjjxnkkl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3coxkvpus.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yxqwjbmp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtdpcugh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpldbxta.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tvkgwbng.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdslosu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lmumaggm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjaodfv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mepyrhly.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ezgtfumm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dlqamlmz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hcsvzmad.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3drqpsfgj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pjzgzpbp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bwpgdoej.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wwxuncct.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jibqpmsg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tqycvvnl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xpruedvj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ryqfveqr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dnftulca.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dvnfxoog.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tcjodlif.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3lncrtjyc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hipzdndq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yifngoql.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3emfabvmo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3nyxarrec.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jazqovmf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3upbsvwnh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ijqiwigu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3mkhcnrgr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zcvhnjnv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aohxeaoz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3obqodxik.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cymhciyl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bofvddyi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bbwjaojd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwwlqxg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3fqhqeywk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zvikdzsm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3sapzitgm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqnkum.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3nppymtjy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wqxlqxpy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3szrqsavu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kkiizkms.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fieqwjwx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pbmgkmxj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3szmtwhta.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ejakayuz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yshshlga.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uegpstbl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ddcuyxtg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3anhrzazw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nctmzzui.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wmedtfvc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pwuesiby.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rxxvgate.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3frutyyqi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgtzzth.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zsovqjht.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pwydfrqa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dhoahlsx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3luhykzgz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gpvkqzkl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hvpgpwoq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ftnuemhs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pzxmhuhe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3udtdoajm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtxyqxe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3npjkelwr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvnvqvai.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3btscbrdh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ifvvpplq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mchblzdk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zmfhkeyd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yoeydekk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lsatkszs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hjzaazjc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nzcvpdoo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vhjydhfc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kvqlwxel.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3lohzhlql.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yukrogms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hophxyup.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ckcdwmkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqvucfqu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ceezaytk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nuptigtt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3deypvfno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vnndlbow.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3txpyqdsg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tsonvorf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbnarnsb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ncyblhoh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hhpgnhyx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3delugdpy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3znnuuvwh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwfgtjad.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hwtuzikg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wqqccsbh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kspkmjlx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zhyqfeun.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3trzmqgeb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pvpqheps.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ihjghvxk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jfchundm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hopmpspl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hlffyisv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqeikbbl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jnvuazzy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqvzpya.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sgktqfzq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3upoixmoh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ztqwxmzg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqiiqem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3izjhkadt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uagnxvlp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzdpqodx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3itrxfpdi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uywmjpfm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rksmjtzt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkgwskon.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3peylqkus.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3prdvasmk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kroiwnya.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cbyidbyj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pomskxth.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxsecmmp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmktikwa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ntkxduqa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pxwzgedp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ipwgzhtn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xcseaapn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbqujhqf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xzydyyvo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3awrnfgbp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3otsiezsg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ueiqzcul.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqdeymkb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aheumpxn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwfiymam.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pgyfccpg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfvnhxf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jfkvebrm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrsirwsl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpbsffz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3znvuwfmg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3oihqljta.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vwrlabnu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3eptqlyxl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zixjniqt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mzxtcznm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hispatpe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kbkiwyin.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bnarlgaj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3prczmibs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zsvfldiy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3agrpuwyx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gnbxnjqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3eugqdpec.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdxdfcb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qjqofhyi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fpaucjfo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaldzrqb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pljvtucl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mpohkydn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nuztazjy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3szfvaxqj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fhgdnapw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dygdztch.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pyvwceul.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vjqmtksn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uywrzbll.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hcefvupn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3omhfkcay.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzidhbs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pbduxmmi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3czgrtkvd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mptulogs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tnjawrin.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tuhfgvzd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rwwtjojo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3chnbfylt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ygnrxovg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqqaobu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zzeotqet.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yozdzdok.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3epgnngyh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmynfstt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qnuumtcq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cbxsxpuq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pyxpakmq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xolrlbuv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gndlwuty.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fivtfcxc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jlptiazk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kapcehpe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yseppbur.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qtnzutgx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3nxeplehc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bzmltsnn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3urqnthld.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pgcfxncx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xurxttih.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nipmgwdy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3usuhxkuv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zmnsyeiu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dosqwoqr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eyqizcvz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mcdgnskc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yfmafnkg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlshznwc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dkklnvoz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xkbkfavn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vmdhpcva.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wzrkllxb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hqrnepdh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ctvorkig.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eknohvyt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3upzrgqrx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qjbpersu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3urgoihid.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xqlrqadp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkpgjtt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ubepfzhn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ofinbvdh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bbglxeao.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vqizspap.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oukdtigi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3igrmeeqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmyobhij.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pxqnwzco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyakasse.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ralwpfzj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zvnceyst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpzoizuj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lgqcgmph.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqaumohr.html


<!-- 参考信息 -->