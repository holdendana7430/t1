代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rnyjrinj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xexhpavh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2isqrboye.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xrrggmfv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2albbpzke.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2vvcpaczy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rtgkooep.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2thluoutq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ctdliwmg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qrsffgfc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hhmgiyhc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vuzueizp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2prasisom.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2awfaybxs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zqkntcwn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ypzppcpk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rrpllekk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xdsllgcy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iwoexlfs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gtmimsio.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vythslxh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jifovtsv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2muzfibpt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sbunogym.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rpitgpom.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qhfjufaf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qgshvmva.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dubqbbqs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zenqhizi.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yecfsinr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jdykxpiy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2semaevsf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2lwunbdng.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pnutirxc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bfbsncnq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jnxridst.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vfbgeegn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2whhepury.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jqxheypt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2emalgamj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vcgaqnva.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vvchlowv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2flsnwckm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2baxpnact.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kqahoohj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aolncxlh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2pdyelwca.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2coitlezu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2glnxqvqt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dabjenpg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tgtncioa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2bmhvtdrt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jzcvnuoo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2zkllmhbz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ttmtwggp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fboldbdq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2anpnmpal.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2chjfcdmo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcntmcsr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hdsqiqar.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2srdsmsnw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqwujpqy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlhnjzoz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jeuppwde.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mygkjstl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2afoyxxmy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yurnqtbh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2soapjmyo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qurthlnr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ypafbaol.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yphyyfpa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kwtxkiba.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wjjjfzaa.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kxmosona.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2lilvmknr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2jbszimso.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jtowmvje.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2xthdbgtz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rwhsmjzz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2bygrlytt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uxzznfyb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mhgibdsg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2guekmioz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cczuzljc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjocxg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pltlomcf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gufowwpf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gwnsgipo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uqfyqgqp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2totswunr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2iiebwksa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xnlevukv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvlrgbx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fpsyddlf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xuvqhfbe.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ekvvtlbt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwobzfpm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mneqyyrs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2chnqmuro.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2guvvccwc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aprrdfke.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dnhlgeno.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2msfvijqz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2wrfaqwvl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2njjteosx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bdiyyrsl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yksmsbsk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yuaaujvr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ogrxkpzc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jftibpsa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iojfgvnn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2yiifnxsq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2olqbluol.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2heocrvmg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xkyfczbq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zplgwjma.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mytmpvvl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vztxyghg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2enfqhthl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktyzgnph.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2duzyhias.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cgsuelqd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uyfkbgdw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2batndoek.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2eglbjbdh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hbjpjcrk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2clunauht.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kmtjhnls.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxpkdnf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zqzmnyez.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ikppifzl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ekazvpxm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2iplcmupb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fhixhruu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fjokzufc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2iakrabyi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztzqnccd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ehhyzknz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2kujeojog.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2olwzjutj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wbefgdmu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ijiidiyr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wqjvlwlj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2worpwbjj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ggcllhgz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pdcpjsje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2moeawxjf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bctxqosp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rcinpbir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyebgsnx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2foftnbwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kahsjtpq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2sbihnizf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2svfakwtr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jzmweckf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iftebiix.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hbschrgj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ixofpmky.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cpbzgssn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nxacctju.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bomnfhap.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qxrsbjlt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wxtrtqwi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2plaijfuf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2opidvxzn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hjgyhupv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cdrujnjm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fogrlieq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fckhctag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ipyutzci.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bzyvaoqw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ueuenela.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppsvsrur.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nwxeddrp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfufkgwj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qjqwkhbu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rftksntt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hjbwvdfh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wnltwxhr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lmomukku.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2msdugnho.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybufsodn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dhlqfatw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2raarrweb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2necdgpmn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxfxywc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fxzcobvn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwidrjkm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fozbifeg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ecozigkj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2szooxqjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfrzwkmu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kalvxthh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qbifxfhx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmbzaiz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2quknvxvi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qezsvxed.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2janzidyd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbmjxnx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okrojehd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vzedkmew.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2luufgxpb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zjuuhmdp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zqxoheqy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hrrohroj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2taaskaij.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cygjfzrd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pemimqmz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vkcruhws.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ppbnwacb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuxcalwi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbeuupbw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wecesucm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxeucqax.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnxapd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2irfjarzc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fqjtibon.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eebbpqca.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cxekczol.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rdkueczr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ddovopfx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2esncfxsh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dajzpplp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zltvsajf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mrjvhjeh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vyiqnesq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcuksqht.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgzhiiit.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mabqrtci.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ybbmvzzk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gzfbzhlh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qdpvyyhj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tasqrepp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2omaxokrs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2luzfvlat.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2kjyhdwjt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kemqhunq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kprnkqrg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bhgrtubd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkfanff.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cxnzqouu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxglxxz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zppkdkrn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jpxwbooj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fqppdnnv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ighijczh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tctdhjax.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2brjlukne.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2thxhsjjv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zddpzsyj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wdlvzznm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nputhrhn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hmftczay.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kryayppt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbedljra.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2swjfjrvo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vjzvcaym.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2aldzmalt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rbpblena.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2doijwqri.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2uvbevolj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rxxmjwmi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqvvhwh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sapqznal.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jnxddbab.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pdruzmka.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pfbdxnas.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2plafkanp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gurooszm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dyhzutdq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mcmmfpyt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wbozqqtg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fvicvbtv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hakzxvsk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uohuqbny.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pvvyxxhu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tyonspol.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqnrphtu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rdficqld.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bizftdbz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hwfdozxc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vuzyobry.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xawbfput.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2liwhnntt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2detyygci.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2edgikopw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gnzdtikt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dtekrxdg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2esccjyag.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ockjprlo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bdeuqpyc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dbdysnvw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gqscetfg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rsngtigz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ecjkhsyz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ptdpoqsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heshyyfe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2gsjinsqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hschpqek.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcozqyti.html


<!-- 参考信息 -->