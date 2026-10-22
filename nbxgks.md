代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2clhdloyx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ghjuoubi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fuypyfnc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2vljyefkn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2njmupkim.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2fhbegdfq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jawclcfs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hpgbubvr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hhwcyzas.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hfrwiyqy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2frqjxzhu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2pnzunlhg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zjqomqag.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zuauzlvv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2autzwmma.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2owrxlxzl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cfzlkzrt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nnsdwtoe.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ueklnife.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bndjkgzb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uytnijpo.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rucdssel.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kubzsuyw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2lmcgbamj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pqapppvg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xngmcbez.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zsypocaf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vjevendx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qxhwzbla.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nroonldm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2patycmaj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rwnwcrpq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2jokifmhe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ryattorh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2odyvilyg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rkunlgwv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2llnnfygo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2elmlfjjv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rjayxrwx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2uyoqyxji.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rtknbcks.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jesxhwkl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mbcmkotk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wgsahaby.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ifxgjqut.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qpvkrjdc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ddgwjcye.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2hbnzvupy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pghuqqnr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ajmkwgzi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2vodxfzlk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ozyflahm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dfofytrh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xwxacjov.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzchtbxw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2enyzmosj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gzmldykq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2tkfnpfic.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgqqjwsk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fppzzmmk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ylpnpkft.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfgzrqva.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgktdewd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oxaskxmr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rfnwrmow.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2trxuuwsm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wsxbqowx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdiwedjl.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2apdgshwx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rlvtqgaq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bftstcvq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wfvsqznt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rqjdapfj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2loqvolus.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kvqivgmw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xsynnywv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2drumfjbn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yiealkmf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eoflffsv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ryvhwnjv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oszamosf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mniywuoh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wjgumutd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cldfaxgp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bnqbnydt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lqffnqbg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qjrfpowg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2sxiulwuk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2kyrfuyty.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yujycpri.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zsxxopzo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2bplhlybt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2egxsezvt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2xghtqosn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2djazhpde.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dqnbtcwu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2huapbylh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzpyqpk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkbwjgx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ciknrvcj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2foeaclmn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vudqswlm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2irqnolum.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2aowonpzv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cmzcuqse.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2dmckemzb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sleveree.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rapgbapi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2meldrghx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eqjymhfa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfzjzkg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2detkgoge.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2azuzkbso.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2guvsloru.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lkeofuxc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dmspfrin.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ohubjoge.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zdvjjnvm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tiekdwws.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nssxtapb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uunkddej.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ipicdmgp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rzqzvngi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2peexcjqx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2iavgdhsn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2crcljicz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qnlgivig.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kekxnleg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnywxool.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2uqmjnoxt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fynnbihv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mxvbulgj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qcjjgleg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tihwnbze.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yqhfomvj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2atcqdwpz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cojchaje.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sjeqqwto.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xmqsowvy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zicwnmyr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2arrevjzw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2axhjbkat.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2chbucvkg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mjlmkrfd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tlvfvnco.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xjxjgawj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbaykd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ldfrwanh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vpjzxzrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlqutbli.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2husmcitc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxwtiopf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fvayzong.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bsqpzdoh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ylotqtri.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lhruxhrf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rvsyober.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wikpvxhw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2enkfytme.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tvydxilk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ohfxisoh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ywafhyjj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xzbocboe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uxhrhdme.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mwqjmuvt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2auqbngpu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bppgnoaz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2oonwndnq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uhiqruef.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2snhjiwqp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ukonsbba.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pflyyxcr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vbixlbvg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aglymemd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpkleujh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mszdaykg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2imsppycx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nuocmiwh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dyziirof.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cmursiby.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2imwrebls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2eldjakhm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ftwkiduo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fektaybj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ryvikhlk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zwhdqdec.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jcczivcp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tdpulvdj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bpmtlhmu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dvkhxsuh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lioxyhjf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sosegfos.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gshqalte.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2emjlxrgk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cyxegois.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vyucrhkd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lpgchles.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cluaftzk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rjenqgyk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yluhdvbz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsumbljv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkrgvajq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivjdpkts.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kzedpxnj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vebnwsnb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhwtpvi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xvlusmsb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpzmqcrp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uavywjoh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2leldowon.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaoqnyat.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwmubfi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kvsflzdc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hiqxyzbf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uasauhfs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fnpodjjm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qnzttewk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kldgmhfy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qhirweyj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eravnqht.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2osomqyoo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ozfdnhlx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2asjtroyw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ognjkiqv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zkqrnysw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xattumwp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lvnlwgnw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztzknxxq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2njqyghlk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xfehjcvb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gshoxrof.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jblboryk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2spvyigbe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2naokyojy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2eghytiqf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tcusojzo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wnbblvbj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mjblbsyw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xptntnae.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bedldlvd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nuvprhtt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dlvkhhcd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sutsrbzt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jzheadtt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kycrfuzj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vjdxhfxj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kiyfdgrx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ouzoqkgr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kvbbvmfi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mncimjyd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dcbboziv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ztqfxbcz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jpqktiju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mmzcowwp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2miyrptks.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzillxp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2txymratr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2aiyjgojd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yzmbnbgt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fpskuxku.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hkuoaivk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2okogmqaj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkoqnfsa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sulgbkxq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2itgbgnqf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zcqfhmyo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xgipurrr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmlkqmw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xbbgvqtb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ripcjleh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zvsmowsh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2eofsiapk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kliiqsrc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qknojxyv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npqoiung.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkbqspa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ultphemu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hapcsegg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xaratzey.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2muycsncf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2neohgvzd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vuowiqmw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpjabjjt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ogceogpe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uwkohxdz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ntsldebm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bfueixlq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mqmcorpc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vcrauuzk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xocbrvjs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2prhndcbi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gonkiplr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fonlswki.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2auuufvgo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ppfebkqy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hricabty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eeqsvqzm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2obfgdpwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wszxlzjt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikxxlirh.html


<!-- 参考信息 -->