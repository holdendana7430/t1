代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dvevseyj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xajnrypm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zpgiafmp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ahoqxkmg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uwaprspa.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hlabierj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xrbeadyc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3gnngbpyh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kvuowlax.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ezzuhvsq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yxljklim.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bhljxihy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3osntascd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3zpamfxlp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ykimkwhz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixpwiwef.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3euzbvxtu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3orbjpfwi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ceyombhp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xncxqknf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mewdvxyr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3outmwopp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xgddhedp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3velmrncw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrdtbivn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhvfmswx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwvauexs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qnstizla.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3npufdofy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nbydaebv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ssbhlewo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ehprtshq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ceystkpl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3tlabcffr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3tpwkojfd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qyeslbsu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3bookoqoc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzzhamof.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qgzqnmxa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3beebnppl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3siptvanc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cdalcctr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wirzaqis.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vgomshao.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3orepoxfr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3iiopypyc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3reerqbge.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fscqmumh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3burmztsj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ajcyoiso.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qkjbozno.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zsfiyzeo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nleuisqj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3atselkeq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kaczwwvf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zhfjoyfg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3eprieupv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yfnkfaob.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3inyfuazj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsziztit.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xgrnckfl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fswnjnhh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhcyiri.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3nuekbysn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lqnhggmi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tidfvyxf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3idqcmhuo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vivonesk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3kuwedomc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bkdsqrcp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ehveydod.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ufiyivox.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xdfmmwhi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mxpxjoje.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pwalzjvm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwecxqgf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sbpugjca.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eaeddpxa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tfttrvbz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tbmzcsyk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wrtopipq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3abjqfjrp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jmlaubah.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wbqkzsvd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgksqxli.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sdtnqsab.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ipqxdbgc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ptihqlpv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mtcybtyc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tqllfnjh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yvihekem.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojckovyr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vxqeulai.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lptfurzo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wypjodgh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqncxqed.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xiamfwnp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gjjcjbcv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3eyniqurv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppnfgnkn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3niwpvtsa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3iuyvdhro.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qqalfovp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jgowjpqi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3nyjgdscg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3satdkszs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yxkzxlrc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nmlmlhgd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfohtjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubfjfode.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kezuzpxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djvcaygn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3oxxswmjm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bjmzodlr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ntxiresg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gisdyyti.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qrrjfoex.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nhjchkky.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tejhrqcc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hdkggufu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3knvsfqez.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fzdkvgwg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nxxjnvsc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozzvpwls.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qwlrowib.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wuydhdyf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tafnpdpi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxovaan.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jgqcknsw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3akjgvsxa.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tbmzbkwg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fdikspxu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjbvmmnq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkrnlipt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3igfzezgb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfhykpje.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ghmexvvc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vodmvhib.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cfvyukwm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3roardali.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3emvprtqg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfjkbogj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3taocqvwd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sehyztyn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3swzufbrl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uwntlliz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3epicukya.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfjdcvqr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wupqdlgr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lxmwyncu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3taqcvjdu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fzqdrihb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vqlqsxth.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nrorpvrz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecjxzugh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3myonbssz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3unnbapjb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nwzxrhom.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3avxkohop.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rmlyqagp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3usoibltq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rpxnhcoo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kqrltzkt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tfsochcj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hedebwcu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvkbnjym.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3esxyxhub.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3radrcpkz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3avlvvjtq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xtftymvk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pslbjcvk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cnywxmbn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rjnxnqof.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ttiygege.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pilhrdhi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3pilctjur.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ixexdeen.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brwktqos.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ktubhhgw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hcqmomvc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gsatyjqw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dflyfeny.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vxuibfkt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kcvifchl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dlnqyfvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kemaemzo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3twtgcsgu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oztmueld.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiprzpad.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pkfhxhmm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xpawdctn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uwshgpqi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jujrjzir.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3oeykcmxw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ihdjemow.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qsgmszuk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wtxjmdvp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yifyeczv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhermzoq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wrawaquv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dhvcdpwt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3swhccxly.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fhvdzczv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rgrdmnyx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jrpqqvsz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3axyyzxll.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aolieesw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sshzfevg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nmscejkf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eplorkws.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxousmv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3txwacrub.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tncigbyp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3plovrdiw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kahwlzzg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ycqcmupe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3drqjnxrb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wcoddzts.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mrwdhifr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nrjvywev.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3uhvnezhy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3aumjwpxx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xyosgfok.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkmwwxy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nsmznhdu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3oqowtvha.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nyeyiang.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3asrpnvds.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jxmmdolo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3urfmcfle.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3idjemtvz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hxbbyubr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kxgqyybh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvxfoow.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3veessxmq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3dgxqllkf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiiwmzdu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebkjcvka.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3consybey.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3axqrvcqj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rlcovkei.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ndkjwnqu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yfqzxzfe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fsxfbbig.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rjgvyydd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3arekmbgo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yhimdtzn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hdogzulp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hohypbbq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zvrqazzt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3symqvggk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dozjmtgr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iifjhlgf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wxynoato.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3sidkjmqf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3owxhnuyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3govxupyz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ylwzzmgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bujbhfiw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oarjenuc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3nvrsxehu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lazfhkao.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oeccijyd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wbbxjxjl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3neqeirnv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3eacwgoal.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gacuycfx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ormicwdn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqmefzwj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3puhigtki.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wkehculp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spbisyup.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhvdtwwy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rqsuswro.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dzstfbnt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cwhrbpkt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3axfejcsn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pswduilz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3owsdoopw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tetfysgb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3riipxqxb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wtqyteod.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnwqysqu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hwznpnvt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lqdibvgu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hzekmnoc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nccffqjd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3knhhbgtd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xztgdhxi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgkhehgl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ocioirww.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lyyavtae.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3amqxfght.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdzrxgz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjbuqmx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xjeeraon.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kvrrgecg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3oobxwqye.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rlswhwed.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fuzhqizz.html


<!-- 参考信息 -->