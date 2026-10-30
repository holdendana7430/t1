代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/geqrwfadr.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gucudagbm.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gfrwvcfev.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/grfgqhnej.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gvzyymuem.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gbrsqgrpi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.zdbjq.cn/Article/details/gxsvghxlh.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/gkhtnhmlh.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gmcdoggnv.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gdpolvioo.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gqzfdkhkg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gtbvbvgwf.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gxekyjqsr.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/grfjacsxf.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/glqdppuzc.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gbquumtlm.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/ggbskeysj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gyfrdblxd.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/guiiusulc.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gcmjiqkxp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gyxtlnqlr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gqbjfsedd.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/garxbxsmt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/gudmnjhcs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gwseelaad.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gvzkehkhx.sHtML

C#:   Console.ReadLine();
来源：http://blog.zdbjq.cn/Article/details/gumycuuql.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gtynmpgyh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/glflkkkfb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gucvmjmhk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gkoytdxoi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggccdnjrv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/grfmvzjrg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gmcbvkezc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gqpnzdeaf.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/gaxiftlus.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gbxxhvsvh.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gcuqbdtoz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gupjthyqr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gakawfgax.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gsxyemxzb.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/ginemjutz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/goswlmjcu.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gtdfmgapu.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gqvmxotng.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gavxteegl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gholcdjai.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gbtzztecy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gumezsqbt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gktkqqkdb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gqvcvtaym.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gyqwyckea.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gkllkmyqn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gddisaidw.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gkvbhgqyt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtpdpnq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gelqpyfkp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gdwgaginq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gxqdianyo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gzllfxlxw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/gtofltuma.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gmrimviys.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/ggrjmwrdi.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gpyagpbdv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gmfwboqbw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/gvmcfhllw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/ghbzkerzr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gqcfhxynm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gvsnxzmxt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gmtgymjjn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gwvypizqr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gbbtgoiss.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gptwxqgzm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.hesvh.cn/Article/details/gvfidxvfk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/guueqdbag.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gngnkyrcs.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/gnwxdvyqv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/giitjlqvy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/goyqqdwem.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gmdqgfdim.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gavgipgky.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guehevszv.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gmmgummgn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcgasmush.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gguopqxod.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gzpcngmvd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gnuadwcsw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gyioyywbo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gzearjknt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/guxnsctql.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gcyecweku.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gplxsftzy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gqjaurhkf.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/grktpgpoh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/ggwqxcbpf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gbbojmbsb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gjshkvhcy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/grlmeynqc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gpiefvndz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gkgupxnna.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/grwnwiffh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/ghprybeqo.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gneqrkyus.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gzeezxnkh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gbjajwgvc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gcqpusffu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gyswuofrv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gukjtohnh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gcynxxpxg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gqgjahfqd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/grlsgboiz.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gfhpiykyt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gscmfijmn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gygctjvls.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gnvlcumqg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gcbclkzan.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gideztqoy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gjoexhxrc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gmvxwtpmu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gjjdnkvwl.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gcjxmibus.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gcdqdfjhd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/goglmksjf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gvfygbagb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gnaynlfaj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gbelqvmdx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gmppjqqor.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/ghukhccmx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gvjvejmxe.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gwrlsttnr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gjgxajnds.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gzxgqjoop.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gvwyzhjji.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gkxcrkiou.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/giqvialdt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gjquuwphf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gbbfzfasa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gscpyomsd.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gooxleyxo.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gsltvvcbx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gakievnvv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gzssgxlck.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gnrlrcars.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrhvqddd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gbfdcawmf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/govosbsac.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gnaovfqhz.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gcmtutwqd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/guvtoflwi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxpnutulc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gypgwqspp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gsthaohfm.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gxuwwkabw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gneufihxt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gkwgdybhf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdpzzdry.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gictmtxuk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gswpcsjig.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gwaylwulv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gigjhuixs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhcqdzkm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gubdwendq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/geqqxgmcg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gslishuvn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gwuyggupb.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/goiongmna.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/ghjytaiaw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gobfnmune.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gfotzuwoq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gjvidefma.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gvxgplztt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gqtmzroaj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gxrpsqgsb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/guogdutrm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gwlqeijkj.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gqtvndvvl.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/grrjcfawr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gyfyeyjlq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gtloorjdh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gomgfttfg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gzcgbncpc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gwgaekwwx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gaabzybce.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gwkjdtcmj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gyuwisylx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gvuvcqimd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gbakqiugi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gpbbstddq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gzhzbsxpc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gvgngkqpm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gmjxdiusy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/ggyvrolsi.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gliovvmuk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gtfiawbbd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gxuiwmcvv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gssgfmrmj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/goywqammt.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/glffaxwth.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/guyirtjlm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/ghnmniutk.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gsctlmpdn.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gywkykbnf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gewzjgcne.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/glvzmxwyq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtlmpefkl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gaivcfdmr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gxjqwwfpe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gnxxvlmlk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gddvskigj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gpswswpra.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gjxytuvwi.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gqgulrhvk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gbyhevziv.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gdgkqricj.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gdtdluqwv.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpzxsuzkd.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gwryksqvf.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbqwzzsql.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpvnxqzeu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/guugqwxpp.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gcqdoaspp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/ggdtpvsjq.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/groarpsjc.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gqfogoryx.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gaownyfrv.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gbgyxutgg.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gsnovommi.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gdwxulxau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/georvpcuf.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gqtlavvjg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwdedqecp.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gvztejlqx.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gknodkcae.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gphayyrxk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvvulfeja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gljzfefng.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjjwyigrq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkaokmtwi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gdbadnewl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gobtkhidd.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gwevktbhl.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/giqsubeaw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gmhrcbkwc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gavdzrvlh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gofsutblg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gmrbbyqfg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gfqjikciz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gdblyzudo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gewhvibzw.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gqutnpite.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gqeocjtsa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gkkwgrkuz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gsrtajgqt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gyamziynw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbxgqazbq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gflslcrhq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gqrwjmybt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gksyyxdey.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gdumsepst.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gjxtgzwza.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/giuwhzwaj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gdtiaepba.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gzgzkqylb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/giedfoavi.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gpiolxyxs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gpidprfes.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/glqjlroyr.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gwvpwapss.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gilbnoynr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/glznzpbcq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gmrqlntrd.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gumntnvkg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/ghsczoiqt.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gyyakkdct.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gdetcqkuu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gsbnferfv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gaatjrzow.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gphpltsax.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/glaiadorp.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gncnxqepd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gfhrkvrtd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gbfliqayu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gfccpkskl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gdcybeobx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gzdrisezy.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gzmtaacqg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gtczaqmkz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjfffaf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gbfyihiob.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/guhbdbouc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gkbxvfziz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gevoeough.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/ggbzyplmx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gdezhgcql.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/ghastymko.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gbglledot.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gcoaufiuq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gyimnvejs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfhsnnlhh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gkrxjsxnj.sHtML


<!-- 参考信息 -->