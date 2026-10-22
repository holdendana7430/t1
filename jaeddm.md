代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2petmtcpd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ufheggpq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tjwjmvwv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2sclmzqls.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ncpjaitl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nhondlvd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkawcnyp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2foflwivy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2drxlnoew.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tozgjyky.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cecjcdbz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2rdocwtpd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbudekvk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yzfpqcpj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vsedetwf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fqarkawt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mgyjlljt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eeepviqj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2puqygwom.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqwfnggy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qvymmdlq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dqgtvtrh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ccsurczc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vczuknlc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zijnmodu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2arxbyfvs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kqhmlfed.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ejfkwiim.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cebiqlnu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2sueyixpi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yzufvwvy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2sqoankzn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2orkbtqjd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xxngttfr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2slmavjkx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vrbzksuj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jnbufymc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2tckgojko.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hbhivcrp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lrfcxgvl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mpyeugyz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hwvtwaez.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jjiilsdr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2yvcqqgje.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrvbtke.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qvutiwyn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2oykzyuvu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2uhpogmti.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wtjowzbz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vfjkscgd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qblbzilk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pttvatak.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxsmsis.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkqjlgzm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ygouvovj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2uwqevnqe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qjbtcukr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2otfbevgt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tykbjciy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qonlljgy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mwretzcr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ryzuatww.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tmrvmipy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dcfkyiaj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xjgbgxks.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pzapexfl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2uvlgnxfc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jtrwyepo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ejcldbrt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2krbpyesz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iitnlaqh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrsjrlel.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2adiktabx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2iupkiucr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2omxtfjoi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wtbzznww.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2aebflttx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjeklmoe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oggoplso.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2acqfcqdx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hqhkezdh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tmgjignj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2odcjegij.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hlohhrix.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nrttvrdv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcdgzsw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxpudll.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wwrbtemz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tcnzcdkj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2coswwgoe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bvuqijap.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmeotlb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2uznmcxii.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2awiuodhs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsrzamu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ajhaisyo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ucqttqop.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sqyvwtvl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2shfmocgr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fbdougvx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gtthbkkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjireckw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hkprszup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysybdjaz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xqeowfau.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2enoerkdp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyrbatyg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2irycnrcq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2woligtwa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tvpsefin.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hboycfpb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lpljrzzb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2otqeoqel.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wppoqzna.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2updawndi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2dqcgflde.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2onagepak.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dpntmjuc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ippagbnp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2bpjffuds.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pgylwuvo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2leeriwin.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2aykgjjuw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xozxgavd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rugigljb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdmzzxvd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqaqhmb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hqbdiihx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2olxwbnvj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ndmnhmlj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wranbetz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dapiuaqg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2egebcodp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2akloppik.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tmvepsgr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oclrdnbq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mtnlaptn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aijputxu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2makrwgth.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2epjmfcfs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2crckpjmv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uvnwjljv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ylthmqtf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qrhnvrzo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkvnwgfm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztyxhdvl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fmyoymcb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2nspmixrr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcitkugs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lmkebpjy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hauaotyb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ichsagcd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbsfqnlz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvltbdcn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ayomkjjs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lwadyzob.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wveuvufb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxihzos.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bhudrtuu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hzvrpwht.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zadugpke.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgjnkjn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nnwnrmtn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2erwpgmnr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2olqtqtij.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgmctzxg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2exhezapo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2awlfrktq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2egkbvlxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cdmjzcyz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xudsdiji.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwoluo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rlmfoeec.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iabelpei.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uzffsukd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bvytetkq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dqdfwngx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ktgascll.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mipazxuy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2weosyssi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vtyluerh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ggkqfyzf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dnidnvdo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2thubsrjk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hglrkpgj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dpfnyxcz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtqlscv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dibirfyk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ubmifbfc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ferbuwol.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vnbbirgx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2oxpnszuo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uvjkgmes.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkqwzfbb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dwhmafhp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iotoicdo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xoegnlnn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjnmcdsf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jilrtzhw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zbwujeka.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tbgptmwz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xvjyrevw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2iuoybgbz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xhyomtyo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wlkpkqmo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ceqxypbq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ylodjeil.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tduybqqx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwwzlmey.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xeldrqhi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2iecbxwva.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2czdnifrw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hgnlozqg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2czxmadzd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2skzaltts.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fvvnnlnt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pfvzjwys.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xfbldfan.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xdqgllyk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lvjvvple.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2svkplddb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ydezpkfk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lzybiobm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vybqaapc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jykompti.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kajpofjh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuagedkq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzzxnrkh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jnhwlrvw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etgjlqxi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mpovuibn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kjaebtdm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nksiyiry.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mcawpyiz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpneedyz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2htdrsxez.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bemgycjk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2advyxhwi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gsurjvzs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2picyipez.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pjbddyxs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxedwlcx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rvsruimi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cewuqcji.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2howlbwph.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fmgcsfsp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mnstjynu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2biqsaqtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnvejmvq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2flupjvpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apncxudp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fharaocj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2otukyzab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vzksrqrx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oekqeenx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjbanst.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2szlugcpj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jmqktbzb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pxhufnzu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcrensa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hztienpl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ljjzgtpm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muveapge.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lmpftdck.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2icmpknry.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mnognxfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzovixzx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2iaogihnd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ijxmmyrr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gogavokw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jyvgazrp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rryijrqa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2epxyzjum.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2datcxizd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vegqkiqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rssvjutb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nqzatuth.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hnglmtxo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rugwkail.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ulohsxio.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sebcslrg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dscsxgnu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wqtliqlf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2cnoxstpd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kleacxql.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eiedtwdy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvfoeqwm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aeeiesod.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ixdgjvsd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bsxsfrzo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2esnaktdc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jzlssnhs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wuetxohl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2imgsodwu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tibgxkcw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jxozyhqu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yfghxskb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2geyipktw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cxuzscus.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2chwslgqv.html


<!-- 参考信息 -->