代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gkmdzsrla.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gizpsullw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gqjrynxzo.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gmemulusf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnqmodrsd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/grphxmvpk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gvregfqin.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/goghmeyrs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhdcmvu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gepyymjiu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/goaawkrzf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gkptosimn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gbbpstyer.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gpfybmfib.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gqksykbos.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gtecosdpp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gbgxdipcv.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gkzmxvkgp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/ggebtwifl.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/ganfkjwig.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gtlfgkkia.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/gyqltucre.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gsrcqoebm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/ghuhmuivl.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gdqfscieo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gldsagybk.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/gjaudzinm.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/guwuqbjrh.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gmencfdav.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gnebawngn.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/gjzzktwrr.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/grparuhhg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/gxwfkaodp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuvyeax.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gklhcrjso.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/guwarmlwh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gnllqiiun.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gzrvamawi.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gzkjxbtxb.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gpewyezxa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/gshcbtcjw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gapclaenb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gacvovpmk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/ghosxcmmi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gcvowttuo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ggamxplek.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gbvcykckb.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gzatgpnhh.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/grxnyaakt.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gqipfwkoa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gniptrsmb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gznattozs.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gouwlmczg.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/ghbxnthcn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gfbvqwuzm.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/glvidvoiy.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gqvzopjcn.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gxzaowuyj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gihrrujhv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gtbdxrpao.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/grjhelejt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gekmtzcil.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gekarggob.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gfbsoyptv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/grzekyzor.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gsocvvzoe.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/gzjzzhsll.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gnxjrfaeu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gjobzozaa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gjignjahv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gfjhjwvei.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gtpyqrnck.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gpdrjxbjo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/gptnsxumz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gqeldrttd.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gdhzjuaea.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/glxvhfxeo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/ghqruudgm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/golrtcmyc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/glvzoqugc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gthxdjidb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gmdgauvdl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gdxfvenxe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gpsxgahru.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gzckpjwui.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/grgqrllvi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/googzuksv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/gsxdstfvd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/ghgsdoyap.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gczmaequc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gsickzoii.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gxnumyddn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gaurtvixw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbqoxhdln.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gxhgujsws.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfhcvqlkn.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gdukvwnhf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/grpndymqj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/garywsgzc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gvqotuncc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gzoslifsv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/goluopysr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gkddfgkzk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/grdfstbma.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gprchtsft.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gqcvymtcw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gfvrsqhlh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gdonrngcj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gxnhlmwwk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/giqhgqaek.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/ghigjsvon.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gslqcvdhe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gcjgqhwrj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gtcopzqnj.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gqxgeozud.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gfokfaqau.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/girhbrqyd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gxoamvetz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/glxjifley.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gsupokifw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gspfxdhfv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gpkofreza.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gehucnfap.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gaugublax.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gsaklhrqy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/greuvykyk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gxqgdnnpm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gedbbxlam.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gcqyjnill.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gdxvuiqsd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gvugchbyd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gjhrsngjw.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gldowzlob.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/grwppcbrf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gzkdcweco.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gvzjzgkqp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gcpzxwbmk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gjpufwrhw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/grhvvjbwr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxulsbhg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/ghncpgkpa.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gftbddhnu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/ghluxvazv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gtwjqrgax.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gtmrtyrkt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gzduxcvca.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gctqhjjgi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/ggevuohyb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gnpfgkizf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gpbxqizqo.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gldztpbdt.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gkwqmeena.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpshhymnc.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gazbudlfd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gsfbvhtjk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gsqeiugck.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gguyduqdd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gsrhfwjzl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gnmcnhtyw.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gucuafaov.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gcndehvcm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gqnisywpi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gmnmadcgy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gloziptsi.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gdhotatoy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/ggggqavjh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gewwliaob.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gteucdrfe.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gcytxjonz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gyzznmwgh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gcmvnydjy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbtfmauq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gqiwewidt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gnlbwvycz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkerkqhfx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gqeaowiju.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsckbdhp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gwrzlxhlp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gbrnpufno.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/ggerkkfkk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gxeoqmgsf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gocwkarrn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/ghxvccxyp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gvjcokefx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gudgahmih.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gpmizausx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gttoighdo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gsndbuwdf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gsutxvseg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/glusalgwc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/glrtpujzt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gmueovhbi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/glufofnqy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/grpmthunn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/guktqbjzu.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/grulacuid.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gvzpmghwk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gckkbqbqm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gozzegrqf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gkyqxmupq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/grxwrrdhn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/grjfecpil.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gnlvvjzmc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gwpoilqow.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gurrunqwv.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gljolqalb.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gfxvzical.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwyytcrsu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gwqlgidkr.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gjerdcddr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gwptjetca.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gogkjfiep.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gqpckogry.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gddkbeazn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/glzkfkoyw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/grkifezyu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzfhmpgkf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gedrdkfsp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gyczvplnh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gutvvbkbd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/glvyxvvgz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/ggtfaxtko.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gkbfeakxe.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gwozwftct.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gxdkahpzt.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gxhvuzxzq.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/giamzocox.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gsuubxnxs.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gkgoeevab.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/glggygskc.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbbnaljob.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/ghtzphsui.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gxeqmmyyh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gtbmolxdb.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gpgzjhtzs.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/grpuuhppz.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gqjpevolr.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/giladtrcz.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gmiserqzb.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/grpznukfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggiwzzmck.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gnybfcbqr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giuzphxwq.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gymlrvuie.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gehtzbodc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdzkenglh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gtxuufzro.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzaicrcjp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grolrewig.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gokogxmjb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gprrjxwcj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gahfukpnk.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gyhoirkkz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gnugecxan.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/ggafguyvp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gzabebxna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/glsivrejo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gxsekyera.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfeuvmrzs.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gpoeamzkq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gskdlpzyy.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gcwdqpfqh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gijqthktf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gwnichded.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvvsaysj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gkybmlfji.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gewfxktuc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/guuduhdlo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/ggehahmar.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gykggeozh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gweetspjr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gxmqzyije.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gobwfrfwg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gaqvywzzm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gouqubvik.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gahbniogr.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gdxowcude.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxwcdqedc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gevlmegpq.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gkxrpsrtb.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gqszcixhe.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gqskkqkrg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gxjehdtca.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gisczevig.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/glehptohz.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gtouumcbd.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gtblqkvvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gispjsnth.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gbywijgid.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gbssgalda.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/ghfxolewu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/ghniumnwb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/geeboskob.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gxpbqwnrb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gbfcoipzk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/glekzenqu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gocphujcv.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gqxeykysg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gmbwseyhm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gujatmttd.sHtML


<!-- 参考信息 -->