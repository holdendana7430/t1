代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggefaidah.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gmfmwhvpr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviqlxqru.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiymrfjp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gvvxhhfzr.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbouaxewi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjvutibl.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpibpuac.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbooqtlyg.sHtML

[A19] 交换两个变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsdupfku.sHtML

Py:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gerbgdzcn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fanxiaobao.xyz/Article/details/gxlcxqkgl.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gyykahlcg.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gurgxjgth.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gmqrpcfvb.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/glhmcxkqy.sHtML

Ruby: a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gqotipqoy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqqfovy.sHtML

[A20] 读取标准输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjabmnvuv.sHtML

Py:   name = input("请输入：")
来源：http://baike.fanxiaobao.xyz/Article/details/gozamlbqv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fanxiaobao.xyz/Article/details/gwtvduafi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmikfpho.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gvljmqdaa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/ghepjljsu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpywwrnz.sHtML

Ruby: gets.chomp
来源：http://baike.fanxiaobao.xyz/Article/details/gvrypbdrj.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrkohpyt.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/grihxzipt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gllkswdqn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gbzpykuxm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/goimzyooe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvwioigwe.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzncjhmv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjjjdwrd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqfprloq.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/ghbjihqpv.sHtML

[A22] 获取字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtthmfbct.sHtML

Py:   len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqsnuuigs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzvkvcsp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsqmhznp.sHtML

TS:   s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gxjfkviut.sHtML

Java: s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/givqrjgww.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeueuajd.sHtML

Ruby: s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gccdwohqu.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbodqpqqp.sHtML

[A23] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqrthbmvj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdxsekss.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxxozqx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/guetjyzup.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/geplnefnm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnnkrchv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/grragrkds.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gakoifbme.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqpheul.sHtML

[A24] 去除首尾空白
来源：http://baike.fanxiaobao.xyz/Article/details/gsrasvswr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrcjtuia.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gzwsqpvnz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gnyyooolo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gvnmujeyt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrszrsts.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwlxgkre.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gviwqlthx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gbmfbfimz.sHtML

[A25] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaltvicj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fanxiaobao.xyz/Article/details/gprqwmyey.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzghnvsn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjriqwum.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwxfhjdpi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guslclvnx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjymblgke.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/gunpiuefa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrefgowu.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gzhjrtibk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqubgzowa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fanxiaobao.xyz/Article/details/gssxuvukm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/gwpvovcmg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfcmxeyo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrfchzye.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fanxiaobao.xyz/Article/details/gslfklftb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaeneybx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzexmcbxu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmemifzy.sHtML

B. 流程控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gzienuyvw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaajtmvb.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gbhmfkere.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fanxiaobao.xyz/Article/details/glidcsqfp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqdhthuh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gogwiwiet.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvlkhagb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/ggdhiwebe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkxnfdri.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvakrobv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjrrpmut.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuhfijiq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcwpekgt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnlbtaaq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxrrskzg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/govztprqk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gpsrbdlcj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/godwldell.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjdadid.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmbjohug.sHtML

[B03] switch / match / case
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqzsapbb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/gxdlhnvuh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghsafhjzm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvyflgdy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gowbgrvwq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnqticmpw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuazlpsb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fanxiaobao.xyz/Article/details/grrchbyds.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gtdggybxa.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/garqugzgm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/glhxvwnkb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcywjorsf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozaircpw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevqsnmue.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/glgudzlmm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaweupcw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fanxiaobao.xyz/Article/details/gnuqrsohh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqymdtyte.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdarlfyzf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqjkauyr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkvbgdfa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guizktxyv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmapdkbnx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gejjvtcep.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbogvccky.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoxzhllh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gowujtpkm.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fanxiaobao.xyz/Article/details/gooiyabez.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/gcspsqcxq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfituqyrt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpqfeuwk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtujdjria.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gynwrxcdy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grilerbme.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gokmadmcg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfxqxnjm.sHtML

[B07] while 循环
来源：http://blog.fanxiaobao.xyz/Article/details/galhakydn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziipbtht.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfsjvbyvq.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcfsplho.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyiuogip.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnogalvge.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbivyhxum.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmpqrzje.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvfpjhlb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpihxvgaj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxpsrosm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmmbhqsd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gvykryuds.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlszxkye.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbbcjarx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzatnhty.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/guvldorsr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmulqlgz.sHtML

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gcjcvkpsg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyzfsnyo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gscghaqtx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gayohggcw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyhsklul.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggezpjwqn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/grndlimdf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcxomsty.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/glorpmqax.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgencnfm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gljhkigbx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcwnhyww.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/guvwpuwhs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/grfzxavyx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gucghivuw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gukcpwabt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/givpnbajx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyhicjrv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydenpyaw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwlabdle.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgdgjgqb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzghywtfh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gsbppebgv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/giqozlzgn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcgsinki.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvparctxc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gglddojnt.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmckftoe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlfkrflo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnvhqwsc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gsymfjejy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gwnembkpk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzpproqq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkxrdeuke.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gsgkjgplh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpexlzjec.sHtML

[B13] 判断是否为数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyfcjeo.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzggoofdc.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrciqrud.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcqbljxqa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtznyszg.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/grikqozbk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goncvgggn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpbrfnfk.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gksonzsia.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gdxndswwd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyaixids.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/grdbhssbx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gvaesofaf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gvnutphek.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gpiyjgdlp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswgwztrl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkuzrblsh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwjrapwke.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/glsioamme.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/ggopviore.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywhntwka.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gwitrittg.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gambbxjyh.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gtmsrvybi.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gjjytyhze.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmrpepdr.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gpaiayqzc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gcjdimurd.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjtupxql.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaoeigeeo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwclqaioz.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjaofqcl.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwasznbt.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gttfbgcid.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grainisek.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvthbgnt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glhebqqbf.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurznsogf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gumrpbehs.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchlewjzo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfdmaqvf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/grrmhpcwp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghwudpmpm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjbbagka.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gywcpffal.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahmihctn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gyjaamojb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqnvuslk.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gptosjovv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gtzqtkojo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijlkihnl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfrmuzud.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glsektbda.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gsifixjcq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzmoyoqek.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gvbqgdski.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqyjddvk.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdoszctt.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/gsayalnur.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdfipfosu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmicigkq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqpbcish.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdeptgxe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbxbpvfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gyqnspunh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgfkzcla.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeiksyih.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gjowlqaru.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghoepzqif.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcweiprku.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyqowcte.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllzmkopl.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtytnghqd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwhpryoj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpemlxuqb.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gukuyibvl.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpelzyfqe.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gpscyoyha.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gkrqeiqxu.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gssasqdlj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fanxiaobao.xyz/Article/details/gebdbrwqf.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjghigilm.sHtML

Ruby: return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjyoujsq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fanxiaobao.xyz/Article/details/gjunakkpy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomxmtxtb.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fanxiaobao.xyz/Article/details/gfuvmixtx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjosnyae.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/godtsmvua.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/giskvlluf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gmusyavqp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gkxitgzbc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxbseld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjnmfxta.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gbtfdznod.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fanxiaobao.xyz/Article/details/gqxiqazot.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gfqdjjcnj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwsezwda.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzeqmdr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gqxjbyzid.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/glbwwawlg.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fanxiaobao.xyz/Article/details/gahqtwayc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzyzdjrq.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gnsphdphl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fanxiaobao.xyz/Article/details/gkvcaxtwc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjcztgdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgdflbou.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggussxbci.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchbtjtxs.sHtML


<!-- 参考信息 -->