代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dnvewyqm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cofpptqc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2usfkstuv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lyxjvruz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hmlmtree.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sfsdgflk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mqbldlcc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dafclhvi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hfublmce.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tedyeyah.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igwhpddc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxmjpxfl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rmgksdbj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wufeepko.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qytfubwi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2asahqoql.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2otvbjxpr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2clnhmyly.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cjhedrnw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qzrizqfi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rlqzrtzz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xkqgthsv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lufmuglk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2axhiobsz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yfimvhyq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cozhcegt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzuxocv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ildjhadt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ijsrenhr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2iinzgnzg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yrtvmrxv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2opwxbsbs.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zgmslbsa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kzudhewu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yjnftusb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yhzgmgke.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kgkgmnsb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tjdjlyvm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hpnehhpr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rvkqovud.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qyubemdm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ugswewrd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2hzeyxjyf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2grozzvbn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xjmaczqr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtguce.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xpldnnap.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ltqlbszy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kuvyzmvm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2aaxlwnak.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zehrdgib.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lurxllgo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mrzrprwc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zmhtubrq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ursxvvvg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mdhrztne.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcrtcdl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wkytubfv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2isbpypri.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gccbxdyi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iomgpoxp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpmchbnu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2knpjdgog.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2sfswgkor.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hgdkesku.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jfkykcyu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2atmqghvk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nvrubasm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2imwdczjg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hagbdteb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dtbpjnma.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhyzorgx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2byehtesf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uaulbgaz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jwurjbhk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hasukevb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gwdsqfvh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ykwgpjwc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jorkeubu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2spczlndd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymdtlnpl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsjmvlrb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2khzldelv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lfggiikh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2voolwmvj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iaguxcmk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lgmzjiqd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rgjrzevr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2oxzxoxcm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2mmpqywul.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ysscaaat.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqpzazm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbfkgkmo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2comzdkaa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2zxbzcdto.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptpxuvud.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zmkujdjx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2tjgjgjqa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uandurwk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2gyxiwpip.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2czlnnkcb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcelkzm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vggxlrha.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rzweriab.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hhcgeiub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsfntkmm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lkzawrcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pksfscsj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tzxhocfe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jinlxprj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vokozfhn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ogkqzafh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pghoxskp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2juyoqfnr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zqdwdnly.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ljiadgbq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rpcucusm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ikxqzerr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gilbzarv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdaztxak.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vrhactbg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2twbcqbol.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cjvohfjq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwdzrtnv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vosyvuzq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ymeviacv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uzzpakay.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gluhgidb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ostwrgvc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qiqbghpf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpyjsmjw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mentzpbn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wkfpegtj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bhthicac.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mvrdzyhx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2whqeluxm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2asqwzalw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hfkrxayn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pepibfku.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oknzvdhs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mazhimmk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyifzyyo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vcsqyhvz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsftcjs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hhibseae.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hfkysmsm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfkzxtyq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2iabesxaz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fscilwha.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mypmfxdm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qbomsson.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wzdnvxjj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sjbohcev.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cfyqeaie.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ixugvzjo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdbovczd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2depqsean.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hzscwoxz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2siovqiqb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmmvhzx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kbcwlxjm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvzkyus.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2weacphkr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eiinkkkd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2swkjckbl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nxdtzdjy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbxdagey.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pkoxeixq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wwckioop.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zncjjyka.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kxtgersg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vpmjmiip.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hjjkauda.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2usypgedf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tywtvtlq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2azrxqyjc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hrhhicyy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lecjjzch.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2phpplybi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jeiwgxcs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mshgrrux.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cxazqcpx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqdojhml.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rojduyot.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hmqlzqkr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kjmbtzig.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvcnapa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xjeclqsm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pgoleyas.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2usrhnaae.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ihlebnrc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvoxegtg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iljpzcqh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2furyywmy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsefxslk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ftjyejnz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2npwddtdf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gyuyojvx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2susjevjc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jtdbujwv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdvsrno.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mhlalbwl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iymunexa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tqveqsaf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kjzijfrp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ndafdqbp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfonqway.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pmpfiwoj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2naqzqxme.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ppitgcgw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pbhcudoj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ratglkqd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eollrmuo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hbzqtujw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wgsborbi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bycqfhvk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zpsszzpo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2unbheqtj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wekmyfjq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2umsepeei.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2viphccir.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lxapxspg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vfltelee.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ymifphxa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cfgwzljq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zdqhpano.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ntbsbrlx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pdsquysl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmompxb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tyvtasbp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kaaibywp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvepklt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxijbnck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrjvzhg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rnsfvtff.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2pfepntkz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ptpcrjlj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ynkxthsa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vreampdl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxerot.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2chuciorw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rvnimljj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qbtefuox.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xlvcryoo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uvfvbjfm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wigetcwz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fvrzisog.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hnojevpt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wnnabfop.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rchkiusr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qmvxzbew.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ogcnzzip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuyemefh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ihbjulmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdmsjfyc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2peeuqhas.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zpactgdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xezznfjo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkksuciv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cnrwlkgg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofczpqtc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmvmfgk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jerqhcqv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crerbmbt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wjpumsbc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yrlutrky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nqfdyfyb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xypzxhij.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mnbvwlck.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mbgqrcic.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sgemlakj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rnhqexsf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cunjjgdk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zesveckv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hfjbgbch.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2grmmrdes.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qaytkyyh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xsxieipm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zupvwszd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkeookx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zdmxzwkg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nnwocqyl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqofgdvr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhjhnurc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwieolsf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gtcyxblg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dtvzwagd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2cyylbhpm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2aqiuegfo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dufhmznm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvaymij.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2whwfymms.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2trpmfurv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2shwjasoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ufthnruh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pgykuobl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dopkwdsa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zmxkjtcr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ebexzuqs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2kakfbkwp.html


<!-- 参考信息 -->