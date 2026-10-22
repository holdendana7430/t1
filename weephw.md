代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kaiibfvw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hxusgfmb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ttbelcce.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ibtqajuh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2faphwmnr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hihlufqy.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rxgprdzh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2cpqxrxhf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bvjxqfbr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sloxwdxl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lpthrvmo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2bpkdkasb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ocyhsswp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wiilmtdd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpkbqhuk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2yncrtukx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2almvjqzp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxkxxfqy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jntdbagi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2owzzbrvv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jnqblvpw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwdaxqtr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahbrnsxl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ipglqxkv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2lzqzazzf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2svvphkgv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkhueoz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bojqlcad.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ehcjxedx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2jafdpsqf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jokpfpiu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ghrxzxyo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2uetpidum.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uknrjupg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bxdpvkna.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mxckuizu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jbobpitx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ydldmlgy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2bndorikk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pndwivru.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lpcoywrw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bvrdtbom.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rertkkgc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ezcllpfc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vznrkesd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dpvrmdfm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ccrtrdsn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jgqyehbo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqrptlk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2yfdzyoij.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2odaxdcuo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hpolqjaa.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqbinosd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qwkbbikv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uubstykg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vxlxdsjr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2futfkvdv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhqvtic.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2umurqzku.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yxijlqeu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rskhodrs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ttlrwvcj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2udpnifcr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2pudnerrs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zomgxbxy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gwkccafq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bccqviuw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2exwdmkty.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xjjvqlcj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ooigubqj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2cncfxgtp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2imyzngie.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2buocnaiw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2veovaxwl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pfxmmzwc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pzailwvn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jaeweueu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2oqviarva.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fouqplst.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rkvcragk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxrekess.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mpgsesfr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sngfyxri.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gcebzlpz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxrkwpdr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2upxmivkq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zytefobu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2teekxxki.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jkmxujgv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jioeqqtp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jxnfutnz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjcaeow.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkbjrske.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpdeunxe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qzujwuin.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qqxbwejt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2blddoffe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jbgvzhsc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bbkhpijr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pmnwqovq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2agbjmpnt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mieceiuw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nrrhsjbz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hyrfrupx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbasrqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqptxrut.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nveprama.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkaoxkmi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lnxbgjil.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2hushwqox.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vshyhabe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vxqhuemw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2thpzlvfc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2duxlysto.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2efbmzirq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2iuttilvt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vjddxqvw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pgiwavrv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zbdspbpt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybkvtcxg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gxlspjlj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yrscllpi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vuwgrvpl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ycyuvnrv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xlfyovcg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jvbisotx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gjpvlvpq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gahvmbeu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdjpzprs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vfjjxfxi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkjuxhan.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvfndbhe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mumvpbiz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mslpxbxh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zfzdtpab.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwdmakuz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bxgaangw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xuephmdu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvsjyfbc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ptupname.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhiwzsjd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjywnbc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dazqxpsp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2saexstyf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eebcdjxa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lohbascp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tssgeffy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2juxyzrgl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wnylswww.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bneqknnj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uqddaowd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2meatcqic.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2viaeyiok.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vqkjwgfp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhtxvid.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtitkrdk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2okysmjww.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vaaaazgc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwjkxcpr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yprvhfkq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fislchsu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkngpnts.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pbvprwfc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tsmhlknz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hjujylfm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jzdcnikk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bybgkbap.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xilqiyvz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mhgywiex.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ejxbhxss.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zelofalp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tosnwskk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2noekhgnb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xrdfuquj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bqjctnxc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2brociwoi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2widsieit.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjpmrxf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ryvqrvze.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pxewiwvb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fsltcwdt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qfemlwpc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sauwouze.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2geiminho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uevmejfi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcsxmtm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xdbqbsxg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ywssdhae.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rdosthto.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2giswdrjs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qaenepjo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cxwnodrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yrujlwwn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qtjzsrjg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2elfhkprq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ivxcuwqe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nkqxeczn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmgbcrup.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ncbpmvfq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2eutvhdoe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvgchsyy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uiwudktx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nyllqrxf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vfmsjzyg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dkaujyrk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zgbdqyjs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ladievlo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vmrvxsrf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2urwykchr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2koodcpvi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qsqorizc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gpwrxdxj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ptrklsam.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukocetdj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dbtuyizs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jhyisjvv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qhjnfepz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qdpmjvkf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcopkfro.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjcetq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2epmppqmc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ducowrdq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qdptsvnt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2caiabhzi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dohtpaae.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2telonwcj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dzogjlmn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvvoczn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqpuubfx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlsnqcit.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mlozzrqk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfentyf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epurduvo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2blzeirhz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dxfvwokg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2uewhtnek.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2khetwvas.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ytipjjoo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2opubslqs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jhvawkfl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kxdxzhum.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hszusmlz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2psowwkwt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pdpmdlvl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2slzvnquc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvnzgln.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xgssynuj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sztvkkgn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rqvhlzgx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2igyeytwd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rtqehgwd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hhmavzgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymvwknzn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjkjgahn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvbsbpds.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2krvrmvcq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vdzgpaya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dtpvrenj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2scwgjdkp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgjdlkmu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uywkcdrg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vmwqgbsu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajwgywqt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdmhjdci.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cjqhybmk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zcblxzss.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ukpgqcnu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tudbknzq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2husyfftn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xiaxejcx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncxquvcr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mbjwmukw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uynuauck.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dbpyeozu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2svjpfals.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2tldenvuw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvbmyari.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hetokvdp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2omorjhiy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dkpppdrr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jgpadnmd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cpnupnik.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dubkszgj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yuvtwbll.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yxqukmga.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mxtyfhue.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kovsgwsg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2npbqmwna.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2laccnbyg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cssredgi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ednvsdot.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qsnovnwp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xlivwhgt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2faophlgf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rzvqgcty.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hddinybz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jzvbakai.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qsdqjnxn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lqdejqrc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bwzolnhn.html


<!-- 参考信息 -->