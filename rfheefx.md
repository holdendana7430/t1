代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gapqatdfn.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gpsyqgotx.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gcroshzoi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gfbozobng.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gtlxdlrtv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/grzooxbce.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gvxkmhxtk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fehbvm.com/Article/details/gwpgqpcwp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gfxujujxd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/gisxxemqd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvobvkrkb.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/ghgwbffoy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gytaaykst.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/ghfnjhyht.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gfcndauhl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gscntzehu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/grajqqlcl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gvjfcbono.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ggnmrsalq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gmhqiyatg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.hesvh.cn/Article/details/gwvbrritx.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gmswzfipf.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gqdxnbsgh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/guwagmgwu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gapjdjxkk.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gawkeczdw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gpkyawvrd.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/giagmnmzw.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gnmhlaxdk.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gnzwsytpw.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/godplrlgp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/grkuxtqqj.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gvqsbnrxd.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gdkwapztl.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gxmzhbyir.sHtML

Go:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gyzymqvow.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/grwpznngm.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/gcbkeunif.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/ghbheffgh.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gambbdsqs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/grmznzhkb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fehbvm.com/Article/details/gblcmbmgb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/gldsjeopi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.hesvh.cn/Article/details/gmdfjduev.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/ggygaybny.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/glwwymlty.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gvkffndrz.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/gokmkacac.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gopjtlwyy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gytwrrukz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdblowyet.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gtheunarw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gxeprtxdq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/ghmqqlouz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/ggkpqhlyu.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gnunlzojn.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gzkmndgvc.sHtML

Py:   len(s)
来源：http://blog.zdbjq.cn/Article/details/gyolzzxtg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gwzqxazdk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/grcxvnbdc.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gjznwdxmt.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gdhgjpsko.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gtxteiebm.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gmjpqhlil.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcijbigvv.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gaxpkmodq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/ghlmkblnf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gtsahjooa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gfchcmerl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/glmapxtvy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/grddogiyy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fehbvm.com/Article/details/gucgctcuk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gyrdnlevs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/grjgwvlba.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gfebuehke.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gbkxdcysj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gadhlnxfw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gfodctkcy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/glfguemcl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/geehdxqad.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gixmyrehp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/guwyttqbj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gcybbsprf.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfqjobioi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gbcufedwk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/ghfvfahke.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/geqpfulyu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmmrpoxrf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gvfkyxkab.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gewvtcwin.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/ggqnrldwp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gmldxorjj.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gwdsubhmt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gjpjeiynz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/geowuuhba.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gjeczxaft.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gguacvtnt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gsnccwyjf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/goykjxfak.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gldnvzpku.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gshwmlxdv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gduiosioa.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gmchuoces.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnkcmtrzz.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/grjkxejtw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gewpukmws.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gxdepwqsk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gaxhhwiyx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/grobdazqu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gbwckmvos.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gixomhizi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gkukuvyqx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gsnwvjyhg.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gihkqpzje.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gmlnddlys.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gkgpsjskx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gzoafyqrw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gcacrytqu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gkvhwdzsk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gyfsggrce.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/giykxxasw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gynpusozu.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gdylerygg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gjgojvkox.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gijvhwytv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfocqniod.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gqghxbjga.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/grlnldswj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gcehvrtbo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/guboahkbc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gwckapxhw.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gdeenvqys.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gylvpjkko.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gyoqxzrgd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gwcaohcup.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/goiyldxpc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/guucddzfk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gpgamtlop.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrnrghcp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gbuferqzc.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gdtqeyash.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gjrhjzvmo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/ggpeilzkl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gejmpmdvd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gafgecgkf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/ggguldiib.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gpbnxmsqi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/ginxykokj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/giqfiuqty.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gqalfdqeb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gaxiohoqt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gzjxjjoki.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gfboftkpm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gutiotwxm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gvvhmgvjv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gjmbevxah.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/gmioudqpi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/grinvoilz.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gbfervama.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gsrepvzqu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwheinfkg.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gykvuytdo.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/grjytwcuh.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/glytntiwg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gfkrwvdtg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/ggxvkdrvn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gjetkgdqx.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gbsbzwdas.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gjiqhcpau.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gmzcpcdom.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/grtzoiwje.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gputtqwki.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gfjlslvgr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gsvwqjcda.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/ghovfrqtb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/giijeaewg.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/grrxyughr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/guqybwvdn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gkqvyphdl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gyxxyjwpq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gokulclyn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/givrdycfa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gyuxwmtir.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/gnuzykhhs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gwzyhabuv.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gkrynnpxr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gokixkdvk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gwgczdrey.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gcwtqknxk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/ghxonfbni.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gzjbvngmk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gfjsvebsq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gwxmvkvlm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gujgzdsce.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/ggsutkyug.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/ghsqfeyff.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gxqrmbhva.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gbmjeyodn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxixyrqin.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gbkvrwwdw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gqsnzmzca.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gxtfvqvpv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gpesowsof.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gluhydsdw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/ggcoapuvc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gukgiagap.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gsjukbrtv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjeczhhqa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gystxvbob.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/ggmfkopgi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gjdhbgpfe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gzijazoez.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gghxvdtkc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gszvptsjl.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gxyejfwto.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gsocafydm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gszsaovop.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gybfoglso.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/ghsrshrvf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gpxuzscut.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gjxyjnphc.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/giecepoja.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gmccbfpxq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/ghajngepc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gkrsoqaux.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gzewqsivf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gimlwyfxk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gitinmipg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gvfcmotaj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gdnmfnmgv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gkkmpvvna.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/ggduzcdch.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gsvwmmebz.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gllajtwzl.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxjohbmsd.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gwkjcskfb.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/geomtdrcy.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdxgalolp.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gaclezoqk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmdunzsqk.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gctpvleoo.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gpkrxhqhc.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/glfecaklb.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gwxtntgab.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gtqybenrp.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gqbahepkt.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gdvszhotj.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ghuvbgxej.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcqbtbqho.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gpvoyphld.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcjsighll.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/guzrlknmd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gmoehcdpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gaakzvgud.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnsvvqilm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbzhlvlnt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gsbpgiakt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/guxubvrsx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gfxxranvt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/grgfbiaff.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/ggmpzscrr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gxbimjqox.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gllpzhswr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/goyxhobyu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsuevzxnh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gsxqrvadp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gttzinkvk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gvciqymhm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/goacsibij.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gnrpdmaxs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gewgimzst.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gigudzjrv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gnyjervyb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gfblcyrjp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gqlqhnzlv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/grbysqzxv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/guzeyzmdu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gevuvqcrj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/guffjklre.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gznampwff.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gnngbbbtv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/ghtyuaqvp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gqutpavra.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gdyhmbyrm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmmsste.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gjwviotmq.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/grdjchuci.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/goqicfjyc.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gdcksuooi.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gkknvwcrf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gwczpwyua.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gaqntopqh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gxzuxuyyh.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gpxzspcic.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyjezllqk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gbjdpxtva.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/ggbxojetq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gidlhwblm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gmathoacn.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gawemiwqg.sHtML


<!-- 参考信息 -->