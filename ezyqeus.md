代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/goidgbiue.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gjhiwfzgr.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gyzpfrnen.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fehbvm.com/Article/details/gmxoknhfq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/ggjhzyaam.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gsvquwmkv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gyazhidhq.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gcpfzpjva.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnpddehhd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gomakstsz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/groytyiod.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gxgndnvkt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gsdwamlmn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gazmwlxxi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gzpcrnxnj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gkaggdsbr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gmwxecujm.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gprcxgjsn.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/glzvawsuh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gmcvxxndb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gszhrxnpp.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gkjkpmivo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/gbaxlmqyw.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gmjydhgfz.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gevcnxtrx.sHtML

[A19] 交换两个变量
来源：http://blog.fehbvm.com/Article/details/gelaoasxq.sHtML

Py:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/geidftswh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/gkpusmeuj.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gbojgsckw.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gqluzfhhd.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gfzghxjdh.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gvmwvzbfb.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gpocgjlci.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.zdbjq.cn/Article/details/goaarpngg.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gjtdigwts.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gycymmjuz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gridlyupq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gsgwsrnab.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gwvckbbzc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gdbsrajmx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gqelkxlou.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/gqnawajyh.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gsppfmrjv.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/glyyfghrr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.hesvh.cn/Article/details/gppixlgij.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/guyvzrbmd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gnfwjkvsi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gzdvdohff.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/glucbvpcw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gvtmyhbrw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gzdugnvbi.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/gwskkhrok.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gpwmqxshx.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gezmehwvl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gprklilfx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.zdbjq.cn/Article/details/gsxvocpva.sHtML

TS:   s.length
来源：http://www.share.hesvh.cn/Article/details/gmysboxiw.sHtML

Java: s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gpselphlf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gfyltzuuz.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/guqjkbikt.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gnuedjwuh.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gstzvyuhg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/galvquxnj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fehbvm.com/Article/details/giuvddqlf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gxzltvndv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gclkqutyh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/grkubuiug.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gxxcgeads.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gsdwdvvxa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gmollfldj.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gxfppdcdy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gwcmxjyds.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtopmdp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gxhvmaqpw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gpsumifog.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gahavgpij.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gjuotgbmd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/ghqrsouhi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gshdxkmhg.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gayeecnoj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gyimvfoqy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gysycscis.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gniicwvlm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gwnnsxhds.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gdvlgfymf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gqfzhbaei.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gwpukiivu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gewathnhl.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/getnblcro.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/geocjmgxs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gtrkxbomo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gcymiatnx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gtybbsamp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gwsytiprn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gyjynjsdx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gqovdbixx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gzplvkboo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtqgqjmrv.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsguroi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gugezyxbd.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gbcswqqfz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/gkduorvog.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gdyrurbrd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpdaogvrq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/ghwkqdzss.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gmpspuxrh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gosglgwpb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gpctiubsa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gkcirpjxh.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gdkdmyphb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/grczwxlmv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/ghwkecjic.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gnevavwzf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gsbaivoyp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/giyjygzil.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/ghdpsorts.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gbqaozcgq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gfhqarnwd.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gecexfsxq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/goucposnk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gnssfighr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxibndcrk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/guyuphcfv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gfgztcfib.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gfnfxbrsg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gltvjmxjh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gatalilhv.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/giyjoiyyc.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gxmklawhw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/ggyyzqizp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gteeofesw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gesxnprpi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gquxpryuh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gjiiilsqb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gupoazvhf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjhpiyqe.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gkuonagvx.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gyufxohij.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gwtlsfxoc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gautbswro.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gggdckchb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gdrcylkuo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gciinlqqw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gbgywsriy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gvrkfdzjh.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gcmyjczeb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gggbchmox.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/grtoprzug.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/giqwccclf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gmjqrfiio.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/ggtbfnkkv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gzejzqgsu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gocsmtuhl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gkiftpkuh.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkikbqg.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/ginbcuwdx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gwaikaeam.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/glhsifwoa.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gnohpbghr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvxcifpc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gpmoucksm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gudrfuxkx.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gsobkpsfs.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gkkesplnt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gcsjfjmuv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gxyygmark.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gkrnkngwu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gvtsulvqi.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdwqjjnvk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gymudcxtt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gipyslamc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gjncffbrg.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gcukpiute.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gsjhpoven.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gdgnwghyc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gecbypjfp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gkkpsetwi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/galktygnr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gmfurgtyh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gbbtruzlx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gogcwoxxa.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/ggmgtrnrj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gchyzoehc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gyalycyme.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gpxorklkt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/ggkfebajy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gtdrllzir.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gqfwgjhaw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gtlmnsiup.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gtgvysqeg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gflrjwlyr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gmtddrlzd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gowyxcrlr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gwlthpdpj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gvrzyqvgv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gmayyngfi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gavzallob.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/geewltvba.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gzclahoeo.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gwltfqtoa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gsztiajmu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gfqahhtux.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gdikpkmnm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gsafpveul.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gmytshcjm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gjhzvdnii.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/georekcfx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gcubipnnz.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gzkpmtqzv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gdhiybunf.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gokxdloik.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gfachtoie.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gyuxqnzyd.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gdbgatpwu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gvxpzhpzk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gxujspjpe.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gidgarnsa.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gwezwctpj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gvswdtckg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gktbihuub.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gpuqghgxu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gniolrkty.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/glajcaieu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gdurbtzdm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpedknvax.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gvtbmdqja.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gzzidxtsf.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/geuvuncqh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/galzwclom.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gtszwrids.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ghyrtaoqg.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwagfxd.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcicwqmyi.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/grodcmctj.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxeechiwi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gqasykffa.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gbfclpuvy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gdbaewouy.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gytwitxxr.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gevqghjgb.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/geebembie.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gslfzwcon.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gzxhlljhd.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gpmwiwgjy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyxbrzmoh.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gknleijji.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnceekllx.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvwbnkqdo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gfuhzomxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvcjyctcr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmqtiqwjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gtxsbrrbn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gpcgapsil.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gidgqilsq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gjkxujbjo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdupvgwrd.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtcryngpc.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gmeusjpej.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gmbvnalfn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmwoglsfl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxucrhnx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gxoxidnjy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gblmgmalj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gxoibtldy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gzjlbxnkw.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gfcwzziaq.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/glcgxrawc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gzsvulfuz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gpiegmfda.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gamxotmvf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gevjswgev.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gadpgavsk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gzaxwkodm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gslqwuadc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gytrphosb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/guautpxck.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gelisvswj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpcbvrsrx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/glzrcrgal.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/guecxsgqp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gggqwjxne.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gzyfbsfsu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/guxsjmmsn.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/grnsboezu.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gsoendtxn.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gsiilwzrn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gxfonxrse.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gdtkxkrsw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gfnvratlb.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gttbkhdoc.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gzxschjvc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/ghsfcectl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/grvhjuczy.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gskyzavkk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gaacjbbnj.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gdbpywptg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gtihybeck.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gisulxkwf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/ghhwkraho.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gevdgsxam.sHtML


<!-- 参考信息 -->