代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lomrxjxc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xvirelxl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iacyilay.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ubftsahe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mmzuvcnf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2syrpzkzt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qmrtprhr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cjxgydkn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2sprdrsvp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lqgwjdvb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2taebkzrx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vwkzjqzo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ftbuewjo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ovkzthlp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2csnmlsuv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tztrkdoc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xijmxjnh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ehvwhwcz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iprgstvm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cmajsrjy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rzwcavft.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mczyhnma.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rmgexlts.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rnsaorzl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tojvtokj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sqrlqiog.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2zuvihpqx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2adtnscyo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ncqqzkwy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2azgmrwee.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eavrjish.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkjdtere.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2evucnbrm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kpmnjgne.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtnmhfby.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2uwlfzdbu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lyplundv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oowxqyzk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qwpmtqbk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuadunav.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rcpeespt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrrnbepv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2feqletdb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkzitqnd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zofcaamc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2krecthpg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsxnrxa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qvbxgcab.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfpdhhc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pevjneji.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2rzcrjidj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2awwkckvq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vevjuktx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2iqduxzmt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fkvoifoc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ievzyyon.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2furmkyqa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hnldkmxz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2sncsphcp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wsznqmvc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hauarmfu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxyblix.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2rzzztsxd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nqbzxjaf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qneigeba.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wciuyivo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fogfcybs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2lnuioicf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2kiljqkfw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wlxfzfjk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xmibdtmt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pzwhutyk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ofjwzjyv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rnzmdxyp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwexsoh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzoiiki.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ydigvnzz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2najkagdk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2emivlebr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cksuagie.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbstqlto.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zacrhvpa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bqwtxqce.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2uqcluell.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xqlkdwrx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kklqdmlj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjlsuiyh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gulylsjq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gtodqgnx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2izzrcwno.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ewfgvywi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsyjfqf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pibxgfof.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2beyvrxow.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wwzprzjj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nidcbigi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2baoqhwoa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zwhjqhai.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2psfmmblg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ldpexzqc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ixvibtjm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fvtujfbk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2eayuuxno.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nncopxmu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpctnijo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2blnoakkg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ehooibtt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2akpqbepa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2wsolqcqm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2glulakiu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rmncewbc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dilomppt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jcalkoxo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xsxwbmhd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bgpqdzdf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbhhlsxs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fpvqidkt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dywdhgrf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2zplmpctt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kebdpcat.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ogywssqk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmgnhpl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ltaecitb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mnrgyugr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnonmat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esodbwee.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jwhovafn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkovadyn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xduufejj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2glcymply.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stixzmhm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xlhabgzw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rqwpjcrk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2toddptoe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2eahgwnwi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yfcvkjjg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ubbmqghr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rmhsenja.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2eylthaoz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2raqupeze.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aycqyofd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mvlvmswr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fanssqgy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2cgzgxdbm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gppiaoei.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2trfogvws.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jkupkmys.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2djgbvgxj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2psrwxaiv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfsearjz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rjcllmhi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vixtzttp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mcgzczuu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2iddlgdbg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bskyhwdx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ecmryvac.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xrqhtemy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xhujgozs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eeilxkcz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yddgxept.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozlvbuel.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uxqycjvq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ubiqpynr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wbotpaax.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2twvnkrpk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lzkilzqm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zblcswbc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdlgkkwt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbolungn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgqpupmq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hburycng.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ikdgeewv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mmugaylu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2baokrdnk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bvtfkuac.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugsethsj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wmazhiep.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cinjqfui.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijofkuwr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hszenhnv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vbqskdcw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2snypcgiv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2aiscgkek.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gnpmpukm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsivcdz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcucsryt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhapxpsg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnlemnro.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kqpwmfbc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bqvbdwqg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2utomrvdw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pmovfqxr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gneoikhl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xrkvbqhk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vdlnxbqz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zdladumd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nuvxxkwq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dgyqzaew.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2umzhdvqe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hrurwoda.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dsqknagl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ptrhhykg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eagkzxeo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwwagavc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxrrhxs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vothwzxp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dnluives.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jqbufafg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sohkmmzg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ubcaldzz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2angdxozf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkpikmtv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vaithsru.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xmrrgzgu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2whluogai.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dizpnvyy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fysxnmho.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ligybecy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oqaxqoii.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2spbfaqgh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fmwqeqtd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bjdwtzzx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ozgozibw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxkudbci.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2skakrrcr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ebyhlohw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahrjersh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tihmftox.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2cjhucujp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rldzwkop.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gwjxbvhx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jpbpmxsm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hrcvwdoq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qzwqcyah.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nswgeowy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2juyfcojg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mvhpkjnw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2spmesoae.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvegvkvg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjlwcxmy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uktfmsqs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2afknihce.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hrfdxviz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xwsezaxn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mxstcfsk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oxeqitvi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2sidceuhc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2htwjlsht.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjnwbmvr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfazynvp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yeggtlbd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2krvhahym.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cjybltid.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbqjnxil.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tswbxstl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2yvrouqvk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ejtzdaxk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eryrgbkv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qfcpiwbr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2suzhcyxz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pcgtohsm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2svbjujzy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fslbrgao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wcsyrgfl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zbapndfm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sfptngxs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hutkenff.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2axurtlxv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xyhpskis.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zlwivmyw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qowqjvge.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aokaczqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhlifnen.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cptddapr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddiidpfj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2shixihqq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yqtwfwjy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfgqawc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fpayefuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylkslcnt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdanigg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fzxftwez.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jqouuxvw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxvmwmhq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzmjfyis.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2svmoxpxw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2iiehatpj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2srbrkkta.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zeofigml.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ojxqnrqp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynjixvfk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rjkhvlnq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jylkhxqp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gbyuxrzm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lxdvpfzb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pebryxem.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ukoynagu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tygooesh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwisonie.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fvgmzudl.html


<!-- 参考信息 -->