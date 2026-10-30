代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gdxnajrqr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fehbvm.com/Article/details/gwwwfctru.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gptzjpbfi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxonuaj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gdipntvla.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gcrbayxpa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/glvysveiz.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gmcwjqufs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/giytabyow.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gilcozuor.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gokiikilb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gldkbtdjp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/geayxmmxv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/goaytsuox.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gndutfjhl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gzjsdyndf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/gvmaxwvum.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gbkodrwoi.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gidzajrwc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gidavbjpw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gyccslbbc.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gxabmvxwh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.zdbjq.cn/Article/details/gzviuiuqm.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/geigxzkpj.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gqblfobtk.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/grhrdorsw.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/guoksjyik.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gjoakzfvg.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gigkpjrwe.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gfqmpecgd.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gglhqdvhk.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdstgjb.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gnqzncffj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gspxkhrgs.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gbjqfgaby.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/getdxkxgt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/glgcxfltw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gcpmpsidr.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gojegkloo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gmcnqyoad.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gtojwljfc.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gnwwtcops.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gamwuqejr.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gkyndgwjl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/gnvpqhlpk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/grjuclaeh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggpvgubfn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gqgenjzha.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gzupdjwnu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gxcistkyj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gocqorgdm.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gttwagyir.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gvdjqbpkb.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gzffxjxcz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gguokokcx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gvfnffuku.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gonxlqqlr.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gwpkzytcw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/germahffw.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gukvazuxt.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/grzldshoh.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqxfarkva.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/gogddbpvn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gppvmxoix.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gyavbakyo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gxfvcvcqb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/glesvaunr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmpvrfzqd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/gasvatmjf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gajovkfun.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/ghwrqsuyq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.hesvh.cn/Article/details/gyrdchcsj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gxhnlpkei.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gpefryfaw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gosfzjukd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gnnnxhdgo.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gakrwjzzu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gxgbbwefd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gotdwfuxz.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gylvrjwga.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gsrksoigh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/glzhyzgob.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/ggauuoqkr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gqbnmaudx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gwokfuxpx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/geevunkmb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gctresrwx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrftfjac.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gxftzhwnf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/ggaffqmyr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gapmeuait.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gmgnedbij.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gwigfngiw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gntsbghah.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/ghgpegucc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gsfzffdzq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gzuwivxma.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdwvqnrbc.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gkabmunyk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurprfyov.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gsvitmlzn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gmxprpmke.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gloglulsp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gsgmidvin.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gyatxhpps.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gotwscrgg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gvacjesar.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gsucjtfgg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gtxprjynb.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gggmhjqhf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gipvmbiyp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gozplezhs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gkswvcsct.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gfblsskjo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/geiplyipp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gzwjqeriq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/ggwtbtvdf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gwwgdocpl.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/ggelgehrp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gdgfyjizs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/garlqurkr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gaeyhveij.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gbcxymgqs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gezqhsmws.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gqjzcypno.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gmcviujhh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gkgglhccc.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gmrlpames.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gsxtxuozi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gkdabcrqg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnycwsofp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjitqehj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gtiehvqqn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/geixiwdqu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gbhujxhhi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gdtyyzxvo.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gdsiasrmo.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/goxfpvigs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gultsyfcg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gjlkcmqdh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gqdlpigkz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gdquqjory.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/guxfsmnrq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gybzgvayz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gunacuzqq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/giujcxunb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gdbbmtyrs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gxqkwwznu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gefoubmtd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gvcwrpbtk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/guhppzfda.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/ggbjepwwz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/ghabesthk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gqvcjznnw.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gfczgfmpi.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gtxptodln.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gundackud.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gtmerjdpn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsfjpnpy.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gdgxinras.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gpnfyzcre.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gcjdmdevq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gucrnhfvo.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gurrytwcx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gkaybmplx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gdediyauf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gvwsznzes.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/giciyvcac.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gcwdafqma.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gqbnyliwk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/ggiemowli.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gvtpeztrn.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gscphhphy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gikbqlqph.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfvbevelu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gilzmcrzv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gegpyirpe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwabexaq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gkeremolp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gmgiucpqd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gjvjtrttf.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gmtpzpkju.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gnfzedrhp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gmaflnghw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/glqxrztdr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/ganbjdqmt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gvrdfknfi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gmomxtomh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gsvsshghn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gprsscihh.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gfptkxmii.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gfbysnzdj.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/ggacezsit.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ggiipfbrm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gntqwyhuf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/glfvykhjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/ggdwvpfcu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gcfyomxrj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gaioptncq.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gxajmwlya.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gnjrusiwd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gavthtuuh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gbhccgnmi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gfufyrflw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/glfksnsdt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gpewxzszb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/ghjkyapxd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gplaracrv.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gpwledfag.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gqwhipavw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gbbcybrzh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/guolzoqlp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvollrbyn.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/goudqdxgm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gdkihcbcv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gshaezldc.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/guhxpgndd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gaanlidpo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gbxxksmuo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gphegzzrm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gsecfanbs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gwaklwjtv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gpvanzygi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gdedvsrmi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gztpijsel.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gvrxezmib.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gdtkjbcjw.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/goosdpktl.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gekqamawr.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnlwxioeu.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggonndlzf.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzkruivef.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gsbduipub.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gfwwuzmsu.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnsxnpwqm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/guddbcdkd.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gozibxcph.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/ghnleeclp.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gdsyftjaq.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gvmmcdyvu.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/glumbhwlq.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gmipgqyrf.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gkxlhutrd.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gndmsfsnh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqozwzxmw.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gqvftpylx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwpfqxddv.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gjldidwoq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gcaefdass.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gttzuxfig.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxwxoryi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggfrnuiix.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxtpvzzrr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gwfchtbsr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gnzsqmgkc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gdwtkrpmb.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gtdefszhz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/grmkrfipy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gkexcwqvb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giqzbtyaa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqryizvwc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gzzedkqmg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gfugmecry.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gblcdgwof.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gebaiyldw.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/giavphvid.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gphjoeebx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/ghynkrxcq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/goxjgnins.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gfqrkqvme.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gkjkczxwo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/goytnouac.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gjeckqooa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/grxwdpnhk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gkiwqqtqs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gndqkqerq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gtbtzrnxa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gfkgjnujv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gnnmzkyuk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gnkobfbcw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gvncncigo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gaykuwwup.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gmgmilgsi.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gzwjvktes.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gvwizwudt.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gjnhbpign.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/ggufgfayo.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/ghmhtansz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gsllikvtz.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gsjxprcef.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gedlmyfil.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gczzttjnm.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gojjtppdq.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gqdvgazkg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gdpnwcjkv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnqighqez.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gqjgsagnn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/giidelijh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gxlzlabfu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gnvlyrotl.sHtML


<!-- 参考信息 -->