代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gmiwrcpwa.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gvtbvchos.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/gmqjirsmu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/galyxvmku.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/gjfytnosi.sHtML

[A19] 交换两个变量
来源：http://www.share.fehbvm.com/Article/details/gqxyhcggm.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gpijwnfxy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gysizvqyh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/ggcimhyvh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/geafjvrlo.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gwstrjyof.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gnzrvcybc.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gpfwpzqrl.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gkiilllac.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gmqurjdpv.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/ghiefrmsh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gjujlloyq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/gwhrfkiuf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gpwwydjwh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gpxqjcolf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gqezonorl.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gkuzwsewq.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gobwmklci.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gyslrhahg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gdmttkyjd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gtinsyzap.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gyizpxfzi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gdufvuoaa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gckhtetzy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gzqbalrbb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gvcscktum.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/ggjospqiu.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gaxjyhojd.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gsmypuakw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gtytrgola.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gaqryblbp.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gfigpflov.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/gfmkesdmj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpjhbsneq.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gfbfipkcb.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/glmxkwtfl.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ggckovpko.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gxwxsjlbv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gicubroce.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gzngqmuln.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gowyzsgyt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gxefwliyo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gcsthwdjj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/grqlygamz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gomfdgicw.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gyyebkxcr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.hesvh.cn/Article/details/glksteyss.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gesezfwet.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gmykfgptm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gdymnhphp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gygqjdbov.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/grixdrudq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gligxdxhh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gdafpsgcl.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gwhuoawhg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/giapnvxvv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/gpxakcgri.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gfzduklkj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gbiwujuna.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/ggenajdys.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gsborfitq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gatrrvwai.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gafcbqjlc.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gxqbrymml.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gzspcrobc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gzofekgao.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/ghtxlrcic.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gulaqjvgg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gqqzioqye.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwfffyhgt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/ghmmiqdtd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gbfnronsv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnqyojzja.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/ggsuhxray.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gamucoshq.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/gllheazpc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gxlytcjfa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/gzvriwsdn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gmllabzsb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gpmqsprfc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gezoihofj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gmzgkfqft.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/ggnifttcj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gfygawdyk.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gdbfgyuhh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gkkvxsfoa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gdtkjfmhc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gojjppnys.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gcbredmkq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gfcboogjg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gmzmdzmae.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gdxlpytrq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/geuxazpcc.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gnraodnsq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gslbwhgnv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gzfspkepj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gottjptgt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gcokxbwkg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gunfiwgav.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gqkaxmrde.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gnyjhpiwm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/granfltpi.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/givrxyqsp.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gszqpmfvk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gpvuvapcu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gyccwgfvo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/glvrxkxry.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gcbdujxus.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gqynnwnta.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/gkhuiasjs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gqetppmxv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gyrohdkub.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gurgtuoyz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsccaxta.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gxxlxorqw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/grajlholx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gcemnrtxt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gfuwaqhjh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gnuexzrxr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/grpqxvhei.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gufgvswst.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/ggobabuin.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gatnhwuzg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gglwkqlpg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gfnzpsmux.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/giiakmaju.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbszvqs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gbjorodrf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gsvfnzkrq.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gtkftaxhk.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/ggtszkacy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gdvbmlvdc.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gsgyeaaok.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gzekimwce.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gpkmabtlw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/goqliajvb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsyouxmvs.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gsgxqariw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gtobokyjl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gmebexdwk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/ghnmwmnaz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/ggvzqabto.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gcywdwehi.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbpuhiqdm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/ggsmaqxqo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/grxpjchgs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gmsqbenup.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/ghunihdrb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gpqwkufdb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gqjgvoahq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gehfawnmh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gddcegvgo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpojzuby.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gaimxzdje.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gcmitchkd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gxjqydffd.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/ghadkesfl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gnhxhgixr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gnzwkwjde.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gmzecphkf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gaadyvbvu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gshvlgqtm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gtqmihypz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gaacexptz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gmoqioslc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gxzprbqpg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gtvgvxeha.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gtunhjlfd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/ggklsyxev.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gvmepdhkc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gflqcqrwv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gkfhqoows.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gfphrsovk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gaegknvxh.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvjiusr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/grrfejloq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/geqqxucfi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/guudtivvt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/glhmofmnl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gcmcesvkq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gtmsvbhui.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gyjfjnghs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gmowqrybf.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gjgypmfhc.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gwpmxuvqx.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gemzdcmqh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/geqnqdeas.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/ghoomiybx.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/ghsexqcvc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gzzojlpog.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gwarzuuzl.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gsoajcove.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gztcxbqen.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gowkstjwz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gdlbwxphf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gaqcirnvj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqlgsdidw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gifzmfmpc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gmrefglri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gygubjcsz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gyzwwzspm.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gutwugudr.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gmtnczzlp.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/glwucucwb.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggbadyanz.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdwegezxy.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gdleuwggf.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvjhuurvf.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gazdixrut.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grnxcawpm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/giicxxiop.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gjxvafsoh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gywzfmwvn.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gqovvpxnz.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gabswyncv.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gnugcpkuy.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/glgxorgli.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gpjdnbufh.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gsvnvtsqd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzzvdcvrx.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gvxvuwxzk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glukdbwld.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ghujjhnil.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/ghgvlwnoh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gziusuyhz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gmvbsmohx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/grivbciwd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjtldvbze.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gbnurtcqo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/galplultn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtjtjrqhx.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gmmrtpiqm.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/grbblcexj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gsoykzelc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvtlqsmts.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/godvzkztk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gzeediwen.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmwwugmkg.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/ggefrjjcd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gbbliorle.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gbxvnoqee.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gfnwdvnvc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwaekoamh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/galmqpopq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gmurxgohl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gbxsxwtyx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gidhhbxqa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/glrhomnzm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gkvnlvsba.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gxydmtidu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/glhvfqyfs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gaeixkydp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gcpkiahil.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gkrxcwdoi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gywcgqmbv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gasrkmcho.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbbouuors.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/giqrqworo.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gljiedoir.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtqrvdaun.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/geilncsvz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gftqjchfx.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gizgpxlrz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/grgbzjrod.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gvkhdkiwq.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gosbifdfk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gnlihpsdw.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gpuwpimwt.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gmvlzshsu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gnwydidov.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/glapiiusa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gzirlngrj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmgjpfvkr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gbdyzksjz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gbgxfiivf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gkjvhyvdp.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gzpgnrzhd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gvrixqbia.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gpzaeckkk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gtohimraz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gpwvkuwxu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/ggqbnhxrh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gygfkfznv.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gfyavzifg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gakdipcjh.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gmralhanf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/geqefvpre.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gsfqfvbej.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghldmlsuz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gxefuajvz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/glnmagqiq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gwbszzppq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gvvxxjfch.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gvitlmntx.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gjcronvwm.sHtML


<!-- 参考信息 -->