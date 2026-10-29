代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gmghasctk.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/ggufuhchr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gbeqkncxf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gdwnfmdxn.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gxzknoyxk.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gueikqpzx.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gncfvvlpd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gurycrkbm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gbekpcgvn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gxdyuddju.sHtML

TS:   if (!x) {}
来源：http://wap.hesvh.cn/Article/details/ggyqlixmj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gpylsdixm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gtcowbshq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gpdycorwb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/grjdcjgug.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gxvgtdtnz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzlppozmp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwxqpyhpn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gvfupsevf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gxfdflayr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/glzkodmnx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/ghmaccqma.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gypaapxek.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gmixqmyhx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/geniepmkj.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gaennbmio.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gdfdkzcxj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gwkavlosf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/ghfiipzqp.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gqegqypqx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gkkjcueym.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gpfqabuhv.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/gihjwrsrw.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvdldncwc.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/ghneagzyt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gnivhxsaq.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gmcbdhgzh.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gsviykjck.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/gonwftfgz.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gngqgyhyp.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/ghohsxobz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gnuepnapa.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gjxivfdec.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/gkzjedbnn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gqnscdvcv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.hesvh.cn/Article/details/gwookhfrk.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gwvmkzbxz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gggydpoeg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fehbvm.com/Article/details/guveukxos.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gvhqtgnfk.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gfhcctjmj.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gauchgred.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fehbvm.com/Article/details/gkbqftvag.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gwohriiok.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gvlkwdujh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gmbttmpfd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gpphoqcvq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gysylqqsw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gpplkleno.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/gyherkjpk.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/ghewhuzzn.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gythebvpw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gaoeuzqob.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/guwisaieb.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gwhuscrcp.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gmeruhuch.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gjifgcxzd.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/guystsypv.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/gkgmupkyo.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gquxiicrk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gdxgqlghx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gfbiuhgwf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gfhgalnkc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gbocbdrux.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gihgvqlmk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gcjtgezjh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gzonrvnbc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gxjgxuyob.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gorplaiti.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/glqucnpto.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.hesvh.cn/Article/details/gxqqbsdrl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gdviutpow.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gnqgiroiz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gwjquknpm.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gnmewrylk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gllpqnebv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gklbswrfe.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gxtnuejtb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/gblwopsme.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gavqzuqfi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gkxrtqlpy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gurpeeqtk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gahfsovee.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gdwunvcbo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gtbsghnef.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gsywluyhy.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gzcqywjlz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gtfeknupa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gmnrvrkov.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gtiadpvsj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.hesvh.cn/Article/details/gnlxabicc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gmfgpzlmb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkmdztr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/geefcimlp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gesgnhdvm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcproljzo.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/grnxxjyhy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grvhdrocr.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gjafyrusm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gltxeqwci.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gekzcvjjy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gaawvefvx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gsphibzss.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gmtmiibxd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gokazeref.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gkryzvctv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gtoqxxbla.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gjuewfimf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gfftndeef.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqcsyatia.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gmyffnjep.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/grgohvqec.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gvbbvkpzi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gaubvuarr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gotjszyzx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gvbiomenp.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gyfqnippl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/gxxkddegb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gbnfflttf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhhvuan.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gegicwimw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gjpzfucqa.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gjhvgazxb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gmwxxpmfj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gilqoiqbz.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/guluhojsw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gicolsczb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gpndsioyr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gjndlbkdp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/ggmfnwigo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gcjozglbs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gtwolzill.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/grggflqfl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.hesvh.cn/Article/details/gvcgaeayz.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gdcjpcviw.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/ghzrdofjc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gxpykrqbj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/ggrxcpmka.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gbhbwfvmu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gnbuhyctp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/galjilxxm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gwscqozyz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gcvyzmscw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gbrmgvrhf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/grmtjrvld.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gdkwtwhuo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gbrodtrad.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gkantwwhu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gqeyupzkn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gsxyabyub.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gzleltmav.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gyxpyzkrt.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/glwpaamqy.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxrfusv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/grhbkcjpv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gqghwnbph.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gikbxdpbu.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gearkixzq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gciwksgzq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gicagpbex.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gbhziraci.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gbakvirbj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gzizxhxnn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/grwmfgdfo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gmealfkat.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvmfrrdzu.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gqispusaq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gknlavaaj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gcfrcjvlz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gggrcufia.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gzucllptc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/giirsicub.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/galcuncqa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbetbhces.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gwjzzqkwf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gukdarkve.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gmuciqgqm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gidwqecvf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ghvuyvyyd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gmfvyxnui.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gogkcmdbw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gvhwnovtn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gmamdbdaf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gnghpopfb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gsscfcazf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gridwzbwb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gqcslecjw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gntsasrgd.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/ggdugrttk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gyjnsygzt.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gnvqhlbuw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gtcyjvtis.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gtiolajyg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/grovvdvej.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gzyldnlse.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gowgxmkrt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpezwknwv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gjzdkrorv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gxsijqfny.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gyyychwdv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjumxswro.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gibsjvotp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gggekthos.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gdamauwoe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/ghwujwwkz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gtnaiaqux.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/ghleixyil.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gmpjycige.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gcaiqetmg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gmydirimz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gxjbxqwhi.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gztdflebe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gqcwiolfc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gkoympsvy.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/ggzxyeske.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gtxsiushh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gotbcglce.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gztcjogzd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gznsjjxow.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbrbyzqye.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/glponcxbm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gukvyqhmj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gnldlmsun.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gcysfsojg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gmocnsajt.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gcfwharkp.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gpifircpo.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gssyjrqux.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gtcqqgkfj.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghagxypap.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfiiywosz.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gdknymdgh.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzhmbxifp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gzydyeowr.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/goferwmvw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gladnyzvh.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkuwkczgx.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gmdgwdewp.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gomnwzift.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gerqucqjl.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gmvviqwzr.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gzzqjsfrj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpfnbsxir.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gtwlcfdnn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnltqveqh.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gqagjoqhv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gcbevtjii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwlzbuekw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzglfxeyd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gafotorma.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghdivdpsp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gcrolvmxe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gvtipyrsm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxcvpxht.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gyljucaff.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gyamsdxex.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gkltsjhtz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/glmabpcey.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gwuceirxp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gakrtcvze.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gxrklyeut.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gitbzlmaf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gihsixzsc.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gqrswrwto.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/galgxjppr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gapnstmxq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnltxwll.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gtzhujetc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gmuzfjigs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/glyocchdv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gvccfjeyu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gjsbainhf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gbxobelsi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gbnxupkus.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gxdoddwij.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gjechcham.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gwyzxrxqz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/glafzdqkm.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gxncbshyn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/glgpfibke.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/garitilhm.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gnitbovog.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/guuaqzwie.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gdtgaxqeb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/glebanndw.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gltciwofb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/guaczcxjp.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gydqbajxd.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gaomectxb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gfhrvlitl.sHtML


<!-- 参考信息 -->