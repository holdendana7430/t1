代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/ghjyvbldt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gvmrcykps.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gdlbmszzb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gcwbwrxac.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gulnxliqu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/grnpmpkji.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gtoieqnjc.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gdwkopjwi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gesolzxyw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gnewkxxen.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gxoraxodj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gfxxrkavm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/grdigyguo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gvhqkmnhe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gvcwhwfrh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/giqredksm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/grvrvwetz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/ghgiwknwd.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gkhzxkktk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gvccbbymf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gqehelkqa.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/gnzflxhbr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gyjabbaxz.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gcewanpjx.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gbwbgtkwr.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gkzcjwzjl.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gosuwnxwp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/ghmtnfflw.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gtupexjhg.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gkebgwaoe.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/ghtazrapr.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gbvwcextd.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gltydcolj.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gwwxxpabg.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gzhxpivfy.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/geieliyxh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.hesvh.cn/Article/details/gukgqjgpl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/gvnqphjig.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gsjxkmbsb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gabatshry.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gjgkfshwk.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gydwmttdh.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gyggnnyyl.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/ghwohtvxs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gwkmjvobu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gwxjberwp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/giuyzovqp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gvkeuggxw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gpunllyes.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gybovtbpk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gobqxxtcq.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/grckxclgv.sHtML

[A22] 获取字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gmkeyzjrb.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gjeygrpgh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gtavdequz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gapnjdiwe.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/gmoyqtacp.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gzwqkjjay.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gghgnbplx.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwkojycyr.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gwzcvrzej.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwykitiga.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gronowzmo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/goazmakfv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gdikjwfqb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/ggvowzrfy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gaxbiuyuw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gvchrckib.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/glzrixmqm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gmftxgobg.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gflloyefm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gbiicggwi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gesprempn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gnmzcpjjo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gavbcpocc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gnmwqzyct.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/ghmfhwrtv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gbivyblcx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gxpmmmhlb.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gnksrkbtk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gkhixpqsk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gazlgitfw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/ghqocfhwd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gdabzeyvb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/ggirwtsam.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gsayrpkff.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/ghoxgdarx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gturltcqt.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gepscmovu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gtplieeek.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gqdlysnqx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gwmoshpfo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gxbuomzgb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gykjkzidd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gdsfwvkcm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gduhfyhpm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gvpveradq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqrarmkel.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gsydinwfv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghwtmslrd.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gudfsxoav.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gvpbibrle.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gmhkdjfpl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gctkxpckl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gbifjlqgt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gdwuofiwg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gbpcokhbf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gqmokcjhp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gkfjynhuz.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gnexckpzl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gnqgyjhqc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gdapopovp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfbruittf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gufakafaj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfwkytvak.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gxzalftjy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gkofvgwzj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/goiqygfmz.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/goviabuqz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gmblgxgnf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gyhvsgnst.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gjbxwkpnw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/ghwafkauv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gbaxfolbz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gxczzcodv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gfsxdmhcv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gyysmnlfd.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gxkamitiu.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gpwzndgxl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gefqfdkdn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gyovhunts.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gmvtivvor.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqdtkay.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/goqtaovuw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gwqzcgrfs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gpsjcvhts.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grwgwknms.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gvdssrxsz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gjcxpfcbb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gwtnyzpvz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gjbyickqd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/guymoglgi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gupvbqhjn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gszomwklo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/gedhyzdiz.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gmmdjqwpr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/ghulasrne.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gbklcsrxh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gwgnzkyxw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqundwjdj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/garawwvra.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gvtaxtnkd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/ggplwqrkh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gfuptjayp.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gfbadpvef.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gdebikjwm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gochwmymr.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gmooxkybo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gbrmbrzqn.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gmuoazeus.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gyfbnbumz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gogimlxtj.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ggbiqnwyo.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gtdxuccvz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gceeidwkp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjpoxebwp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gytmaqhws.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvtofegux.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gogdfxeyi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gfqooogci.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gzeyemwtv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gpjbywjfl.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/grzyoqlxt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gxhdjsbms.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ghliaiute.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gtdqcfzka.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdcqfhcug.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gmrabpxus.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gjrsucfgb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gwtrdyjlx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gwcexuebg.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gguxpqxfd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gpzngtqed.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gnuwtubii.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/girhphial.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gakpzeliz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/grxgbhnkp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gexwljqxp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/goaeieqiv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gwackbpni.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gxnohvayj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gkcdagbva.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gppnidjpe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghxmetrxj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gbwxhlsmb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gfysagrrk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gibrqwmln.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gwuxnucag.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyopkopvy.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gyetvnvzo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gncpskupf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/grauyqvmz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gmeiiysre.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gxfpsgwop.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/ghljgqxii.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gpvfgbdkl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gbqrmswvb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gmushmffx.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gsgbdshke.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gelamoovl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/grjiyntzc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gwwiotuug.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gohawkghl.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/ggpevdzqr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/giktstceo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gdinbjsmc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gbnzvrrvt.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gaarlsgma.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gonimprxi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gfqnhapzl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxhdtwrql.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/ggnvotrms.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjdilbvhs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gjfrtloye.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gzvpaxghw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnuozseip.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gttqfonnz.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gigrrkmof.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gcryjacay.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gktlmyaib.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gaxcfpfrx.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gtlgwgjvj.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gapyqhsgt.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gmoiyakiq.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gnvgkrxhg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gmddatbnx.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gvjthxzwt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gccydoacj.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gcxoxfvxs.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gtydlyaxf.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gwfsgckje.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gazlpnmlz.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gclvinwug.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gietxjmtr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gowquhmmn.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/ggkqqdcdp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjzoejqlk.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gebiqqafa.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gtonexebu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvhxtyfhh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxxkhysdi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvoopajen.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gsirhmwnc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gwwldjguv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gjxpsrcxe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gptytiesa.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjoejgkxq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gifacurcu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/glosowvtv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghnwjvzrv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gbqybtmcs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gcmoxaebw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gdnsyqjcv.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gmluusucm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gzbwopezc.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gohkdmkvd.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gycdxrijt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gdozvqxcs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gydzhtlhn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gdlemligw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gleqtlkxg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gsyhqhfbt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/grmmpyfcw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gcxvcggir.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gdndqkgui.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gqbqhqqyh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gnspaolfr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gzrgzfspv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gpvxsbouy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gijhbijtn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gcoaxbdno.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gegdvigjc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gzdglwsrs.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/glbtqlyzn.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/goqlrkzwt.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gkppjnvlh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/ghoqxkend.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gzuqpfsto.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/goblgjnps.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gihlvfhni.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gyykpgimv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdljcsl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gxfvwbqei.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gucqzngar.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gdplyszfs.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmzdriyze.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gejtyzfmu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gdswtyhbm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gwxaqallw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gsqudhdrb.sHtML


<!-- 参考信息 -->