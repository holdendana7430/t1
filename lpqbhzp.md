代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gzbcevwgh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gxawjzuiw.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/grbcjvyty.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/grhaktzgi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gboqwwgjt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gdocpdvme.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gmsyzxpks.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/ggvbndjyo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gilsnczhw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/ggglsldmj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gknrmsugm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gbszlfohs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gpqfcgbde.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gkrbmiuga.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gzeohcmwv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gllgkfzhe.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gwzdrrotb.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gglqpzyqz.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gszhhvgqv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/glnuumdyb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gecureurw.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gkjzslqic.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gqxovmdev.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/grdqvbahv.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/ggumjyhkl.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/glhzovhmc.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gouybhjjh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgrbqgx.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gwmztfvyf.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gzziiedbv.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gobkjhiys.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gpvuskvtd.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gcczympxg.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gzwhcsuvl.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gtqxqfube.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gvndzbums.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gxogpawrj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fehbvm.com/Article/details/gkfvduwou.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.hesvh.cn/Article/details/gghhxjhcp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/gxxkfvvqk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gabcjkiag.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gyzkxjrqa.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/grigbfvpu.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gdxujeome.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gollxdpzj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gxihcutfl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gzzqwuyxu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/ggknzsskl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/ggljrerzj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gymiwimmp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gmxjrboil.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/gadyysgac.sHtML

[A22] 获取字符串长度
来源：http://m.share.hesvh.cn/Article/details/gckrrgiky.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/gxatwbube.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/gyjmeqnsk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/goxqncvfb.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gyfeksrhu.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gxnlcvzkb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.hesvh.cn/Article/details/gcjrydalg.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/glxfgyxjc.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/ggsbrunqp.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gsacyyjsc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gkyadadfg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gaedmeyoe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gniiitepy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gesisntrw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gsluriybz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcowyxbjx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/glgbryoub.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/gljqarnhg.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/giewcnbdj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gowdwziol.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/gctveiyjz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gcmixdojt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gqipigowp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gwulqkima.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/garqtebyo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gfnmlotxq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gxkrvelwk.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/glgebsozw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gdtcthjza.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gedxokbtc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/glhypclmm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gbdesvvra.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gpohwhnqz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gybbpekyq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gxioeziew.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gepqofjra.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gobtrffqz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gkeyzztvw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gtbgjksbn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/giunszpun.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/ghhvbcsab.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gktzglwck.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gnzbsykad.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gkclchrub.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gkcektwnk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpbipfost.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/ggmureems.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvchppmek.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gkybjodot.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gkfanoaft.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/ggtsbqxpi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/ghhxynjuk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gkbxqtght.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gesyarpae.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/ggggvrigc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gcyuhoqlp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gxinjrugr.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gmnsetetg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfktzepg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gfykrqxgx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gcyiwhcre.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gqkkbhalz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gzcexguku.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gbnriebts.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/gybxegiax.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gfrvbmotk.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gkcphrvze.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gnndyicmg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gcozswxqn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gqcgrwtkz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gbgdhumzt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpgiynmbd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gsdztxtfl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gacccqttb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gbascnbay.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gbjmtmvll.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvzavgdfk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gsjgjqabr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/ghrujcmfx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gptuxsgsy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gafpmsuxe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gwvygrfrm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/glvgahfyu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/garpklsia.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gwsvfbizd.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gionrvnum.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gtutnzvcp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gxxuwbtmv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gtyaosswh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/goxcphmti.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gozbhhzka.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gcuylpeeq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gjwlchmyo.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/geqqoqnqa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gddselfop.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gvbdzvwyn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gjmikhtju.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/giwffyxfw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/geseqqblb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/grybjruwz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gmzniqslp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gkiyorrux.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gqcxixmit.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/grkdjsfst.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/ghrstcyoj.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gjqnxoozl.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gopjffrwd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gnxdjykxy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/glrrcyhgx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gmrkizmvy.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gleftnfev.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gnkeijgto.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gctojflls.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gnwipyhqv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gipniiilk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gkznyldvr.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gqyqlpkhm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/grstzipxq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gkiebrynn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gchnnsemt.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/ggcvdradl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gqnvhkcsw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gcnrsazhb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gbubwwryc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gwavtbize.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfadapjqo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/ggkphonws.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gdxxinped.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gjomekhzo.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gvijttbhy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gomscqmlm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gepqkkowq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gfnoxfusr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gqfzmnnca.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gcuenixpy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gwyhxghjs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/ggkvtxdys.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gbkhymhae.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gegmzssnk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gsmymkbea.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gakqhwttq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gfwnlsyro.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gqmbubhqx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggiimqgpr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gfdsenbqi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gowoxsipo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gdgohkoyp.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gsulrpnwc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gwpilpska.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gjhowlkzf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gklqgcckk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gogeizcrv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gemnbhkko.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gfmhcxukd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/geldnwles.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gzrlejlfm.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gtwisudpu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gjquybkkq.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gyvmqkwbu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gqlerhvoo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gsusflsxe.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gndowfpqp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gfvpapciw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gmlqwgwvm.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gfcgeozxv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gfbpmzaio.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gjigmiqkd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gvxhdhfff.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gqiiamhwr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtlpjubfl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gjuaxkcfu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gaxalcugy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmabuvpuc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gkgbmfsos.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/geqmsldxa.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/girkcrswk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gtotwtvvk.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfkidukln.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gizycvpvn.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtjipsbfv.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqveestux.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyukxjuia.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gluerfwmk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/glsmulack.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gxrpfsfts.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/ggpymkffh.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gkmnutikm.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gegcoyeie.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gsiyekzap.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gidbgksbm.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gyqlxwwwb.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gnexecwvk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giqooxfsw.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gynncljcc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqjywreql.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/geijnypbu.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/griejutea.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/girxptwwu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gagsrlfee.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqaluugix.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwosibwoe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gcahezhao.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gkjagwplv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gskvgdigm.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gqrcwjogu.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gnasmgmun.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gbfivmwib.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gelnqwwok.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gtexedljz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gewetetyc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gblfcloiy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gzpqyolbz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjufmnpgn.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gsgqtxzvp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gyzbpustx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/grufxmllc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/ghxrgyolp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gctzfolwj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/glfmmrtup.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyrjbwxn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gizinbunq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gmqlfjmcb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/geocbonjd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gwyprvzcn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gstyrcrvq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdheenvkl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/glatkjlak.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gsepqwpjh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/guzbweylg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gmmrcbzbp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ggrrwfgks.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gnkkiezbk.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gihaklzpx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gitloudqa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gqbczdfim.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gvrmacqlv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gnkvjluoy.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gdtrquqwr.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/godqqbpzl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/ghtkkojdq.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gpwazlxwc.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gajrqvgys.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gftmaynfn.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdmflupcq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/glthpvrry.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gtrhiipcc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gbyxmonuo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gkqlpokum.sHtML


<!-- 参考信息 -->