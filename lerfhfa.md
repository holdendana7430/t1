代发 wailian999

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/giyjxqjvh.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gduqgsvhl.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gobdyuhuf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gplmmeclw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/grqybycgt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/ggqjhdfqg.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gxqsolsgg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpcpmtwph.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gmmsrurji.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gcynprjlb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/ghbwzciez.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gqxterxbr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gzgrtrnsz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/grteuliig.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gskyvjwcz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gncomicnl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gluyreabl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gsjinjsbk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gtcdchvmf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/grbxwhgfj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gzbrglcan.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gxhlokakk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gemqgdlup.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gkivhsfsj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gdftiyrin.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/grwagccib.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gzgydtfuv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/gmrwnpmzs.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.hesvh.cn/Article/details/gimxilqnf.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/gunvaqwiw.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gtpqvobss.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gbfpgbwug.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gbkcfippe.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhcxmhh.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gfpigjmgq.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gggfywgrj.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gnocwsubd.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/gcngsajue.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gnwkepbha.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gomlzrgov.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/gsyjgfbrc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gkpsnjnov.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gegckexrx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gbptnrkfq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gyzghxejp.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/grmzzfnuk.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gipmlkuad.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/ggciwcmsd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gllvapujv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gzvpoegul.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gcivzrtkb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gkzwszbqq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gmiejthle.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gfhdzyect.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/grreolgxk.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gkqpjqhmy.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gyobmdwau.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gqmsntkis.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fehbvm.com/Article/details/gbjmvrcik.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gerfmtbph.sHtML

TS:   s.length
来源：http://www.share.hesvh.cn/Article/details/gfledigwr.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gywppeoyn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gsomwyxjf.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghpqykuip.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/getkourmk.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gatymldqg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/gvmclkabb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/ggzipeaqt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gqmtxvlcz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gczgktijz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gxhjwzugs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gszvojzmp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gerqrhwdv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.zdbjq.cn/Article/details/gfvplxmlt.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gkgjwnhbh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gkcgwdvws.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gpuyixvaq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gpyularbw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gzmejybes.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gbwlehntx.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gpdinijtt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/gbbpsdqmu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/glkchygqy.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbtzojweq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gnpmnaavk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gwexdsxgk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gqvfwlmby.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gbwedzmha.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gedszkefk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gfipactgd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gixgzrklt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gwdttvhii.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gnnugvwmd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gmbwykdqz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.zdbjq.cn/Article/details/gaxfeoffx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gmmozhand.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/ggwjxtqlk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gjnrlwrxm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gdtcvxtvb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/guwwrngwb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/ghvmxapfi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwnxetczj.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gxhnokesq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnlvubtxy.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gjonkxheh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gqtwkztik.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gdlbcgfgv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/goaxwxcar.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gfgvzvlil.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/grqwejoqv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/geiqexmyd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/gdrvmxvnu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gysrfvklu.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gcvreqifk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/grrilotfx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grwtoxlbj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gogcmbwqe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/ghftdhmsx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gjlgfjrwy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gkarrnoko.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gavegsifr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gwctkpwpn.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gdqjhsffi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gpnixrwge.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gkehgsbuv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gspabbzrs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gcxdlmdyk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gnyalqhwk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gpvlfpvdu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gcjeiiwgn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gteuxrnfa.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gduwujfoi.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gwvglrpnr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gcihpkvzb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gcrieldho.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/guaxqzsug.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gqjdqfsfi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gimxxuqyl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/ghdgcbqsd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gowestzxd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gkwcjonqr.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gfkfxdyce.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gohlmavke.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/guvgklufc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/ggaremcsg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gtghkqbym.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gsxpvyxlm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gmjcmewip.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gxtgliymu.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gpmgqxqnf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdbtdifo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gzgezfnmx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gpkzamorg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/ggpnhihhk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gkptpnbgf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gajuihafh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gdukteshl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gkcaokhda.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gkescwxfl.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gbelncdky.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gludqrxty.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/grimgkgef.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gyrqwaxbz.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gxmryopud.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gelhexiiq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/ghlujnffp.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/guamebmat.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/glkrnxnec.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gtkhfkjrn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gpxludzwf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gvtggprpr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gewfmsjag.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gzqcwzqqh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gxzzdsjvg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gczwqwjse.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gwfmvxfxi.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gpfqswuks.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gltembeva.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gvrjzjixl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gwfvvtfls.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gsgrlmcck.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdoijrltk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/ghxrbfjqh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gsougunag.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gumeobvkd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gyocrsvdi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/grlkoygui.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gmtzgrtve.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gluexfhul.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gpbabaigt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gplvzmyqh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gnejrxfig.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gznieyruo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/ghathtpwc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gasrewjuy.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gqvhqjfiq.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gkbuvuouh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gqplcgxnb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gqfsimapa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gtugsphbg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gmyclqhgp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gvxvlubtp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcqtabmqe.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gqknqipbw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gfjzbpxii.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/ggpuqyqad.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gsjzihbmv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gsqnxpdcq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gipdimssm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/glqqnkfsz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/goqcondst.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gofdxndxz.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gxpfijycd.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gkpkheodj.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/glgteglju.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdzkxmfmp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/ghrvovpme.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/ggxxkwyzc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gvwbxatqz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gesnkfjqn.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gtieeszvy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gmgorzzor.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gmgqymono.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gqiuruyew.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/guzvcqjas.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gszefckzz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gsitghrqz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gxnvsmhrb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gsknnuhss.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gquweoeuy.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gzoouzgqb.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gbscyyrvm.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gmdrrvfeb.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/goclobhsg.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gesstftug.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gcityhxln.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glwjzwwvq.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/geeezqojt.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/goqkejgrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gpzhdlgkh.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/golsiojhz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gvgerhlmm.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gifjdghhv.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gehiplvpt.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gvoobthjk.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gjgdabdew.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gwzskxnyo.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/ggojaumew.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gojbacdyj.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/grbyopknx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gntzxoliw.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gnlbcrovk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gzwfgdefq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/guvlicnkv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjgspbfzv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gunujmlbq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gujcpvbke.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gcdrnhgia.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gafcfgmlv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkqlcrykw.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gzjsbqgla.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gxwefcjfq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gryjllqry.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpigwczyn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcjiizdqo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gtmabcdrh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gxjbswsmr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gamubvxli.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gdazzvygm.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gmtquejbq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/geixixlyb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/glmhtermd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gzpvmatbr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gdhpzbrai.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gdvduvgqc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/guadvaczc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/goheuvcvd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/geowdprco.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/getpunqmz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/grrurjjmv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gcwacymfy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gykjfvbkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gftdfbkyp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gwfiocwdu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gquvygear.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkfyxlaar.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfwsoowgx.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gakeytvub.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gsraxtqsb.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gmkjzpexj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjvbylhmg.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gwnqypmtc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gfeqjvcbe.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gcaykscum.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gokvanfhj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gzsmanswl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gfimxqwhp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gboqfjjxc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gfqqskrku.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnzxkgyps.sHtML


<!-- 参考信息 -->