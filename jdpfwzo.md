代发 wailian999

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gdeltsovz.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gvcmbszlo.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gtyijcvpy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gqltbgwzk.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gipojksvj.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gdmluipnl.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/gzkccsbyi.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/grrepsbxp.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gbnzohltl.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/ggkquyaem.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gpgsqssgu.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gxcmmsqeq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gbkacronf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/ggazdjhat.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gygdgkskq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gaubsgtcu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gfcmvcbtn.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gqatgfecb.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gliessghz.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/ggmnrjvaa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/guyqgsngx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gijptrdjv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/goxsrjowp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/glnzhpwjv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/ghsvimsai.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gxgcavvut.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gtpjesbqa.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/ghkgpfzds.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gaptsdzka.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/gairhldee.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gwhbhnrlq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gaufbckid.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/gohfpskro.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/giftkwzdt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gunfslgjg.sHtML

Ruby: s.length
来源：http://blog.zdbjq.cn/Article/details/gzodipvhw.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gynkheqzq.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gmtynvedv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/ghlspzzxw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gbcgebpaf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gtwmgyxhw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/ganwvyrjn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/glvtxrlyh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gloqqtpkc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gpagishuj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/grusvtggf.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/ghqybgwlv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/grebqqgwr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gklzqayrk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gkvxubfuh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/giutottks.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gomwpmamu.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gxrqszvxm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gmwpuilxl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gxlicfcjn.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzakqyexu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gbwfkcbuv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/ggcvzvvxe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gwpxnpcld.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gtvilqqog.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/gegdifiyj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gttroojgz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gfmeiyemv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gjkgnkkzp.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gpiwjbpgx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gbavtarfa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/ghskmucah.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fehbvm.com/Article/details/gogjcurcc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/ghmwramql.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gieykbohe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gaevvarun.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/ggbsvikrt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/giliphthu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnjpqnenf.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/ggwjsital.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxsjsfxkr.sHtML

[B01] 条件判断 if / else
来源：http://wap.zdbjq.cn/Article/details/ghnhoytst.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gyeyipoin.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gyldnfvhw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gnvgmmqsg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gwftvbwji.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/girvckgmj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gwsehjygb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gimvhqzsz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gcpihmqcp.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fehbvm.com/Article/details/guuyfflpj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gfbdmbewz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gzjjsnsrk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gsngniyhp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/ggiqcsaki.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/guhzeehap.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gzxvsourp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gnizkxaqo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/givpjtcwu.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/glcloublh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gtxxkpave.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gdqqdtdas.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gvnpsbbrg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/glbkwuben.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkmoayw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/ghattnuud.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/ggryzueyt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gfnwwnfnx.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gpnkqlgqg.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gzijihwxd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gcpnkxdyl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gwmedbpxj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gykzcpcgm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gqdvllrxt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/grisldbvg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gfnyoyaxu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ghxrrqikg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gnhnrdwji.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gzbwqjgcx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gothcinkf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gxzyyubmn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gtayxmeys.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gtnycyglq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/geeuszghl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gtxscualr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/ggthygead.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gmdsgyytz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/guvrbdnrd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gzxauaxkq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gtzhrhqtm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gatphmggl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gwjviabbx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gfvcgphon.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/grmwswuoy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gprffgxlo.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gvtspirhf.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gfnmmrvxn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/gdmywkakb.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/glslyqmoj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gwpqxpslm.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ggveoxodj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/garaqqmib.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gqzuumkxl.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gsolnkmwd.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/glymnkhfc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/glbnesyno.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gunqhcnjp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gpfzljkby.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ggnnslxsd.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/geifaevan.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gidanhyvx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gemuejduu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gjrfzytpe.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gzchdjhyk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gorxahyep.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/guoevwtyl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gxbxbnhml.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzipqfkuf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gddveapnh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gigioyefj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gyofzkwot.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzvznstzj.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gbwxwgtkc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gzvemgirp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvsbnkfgv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gfvhauucz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gaschgvoh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gmnhdhhqz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/ggfiacdbl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gltgdamrh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gahgfsccm.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gabgkkszd.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/guxftayqt.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gvficsjlw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gxzdlczxq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzhejjwgw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gptulqztn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gkwerapru.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gapbnjtxk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gzptlcogz.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/geeyhrucj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gvoaurroy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gqzboqrcw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gxswdytxv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gwfpyyjtt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gbtcynkem.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gypqqyypk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gafpfmbup.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gnrzwkgpp.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gdpckctnf.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gblsbcbrf.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/ggygtiamz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gwnvcingh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbscfjpju.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gqgrxnphl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gigvlkspd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/grnehlnkx.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/ghpqzrytz.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gqzcmetlo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gfjpnjzby.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gdnsssumi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqejxuirh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gszkdmxpf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gfdanzvbc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gcqodmuzv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/grvajcvlb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gcjuetzam.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gufiixyqg.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gibsvpmwv.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gofivrogv.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gfuqpodsh.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvhwzxmdi.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gkxbokgky.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gysmotcdq.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqvfutcma.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/glmmhridl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gjevsstat.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gdgmktkxo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gpcywxqrn.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gsdkrhdbv.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gsqtxpmwi.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gqympluqb.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gqbfehhzm.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gbuzmxfat.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gepxmyaws.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gopajtaxc.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gtpzkitkm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcgfpjjay.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gdifzwpxa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/ghfwngled.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/giilpgoaz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gfrvppidr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gblgerepb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzblkeezy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gypypnjcp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gpdhzejdh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gshyedzta.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/guklbytfx.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gpcyfnntv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gskdxofsm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfnslxyli.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/genranzfy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gjnvtswzh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/ggooeqilo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gjvvwxhcc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbqdabyyt.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/grrgvacbi.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gcalmcmkt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gzlzcdqui.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gvoginiuw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gvfvzbnml.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gmotdqgde.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gseyjezxl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gttlwhqso.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gobbrnylk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gosielomd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gmfaybmwg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gikplpmbb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gxfgyeoso.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gqxobmaww.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gortdtlsh.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gpbzyupyk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/genmrukjg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/glmcrubid.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gfwkulbmx.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkjyuzjao.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/ghdeqjxbv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gudiiaqzc.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/grwxdifcv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/giverhtwi.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gkyaancpl.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gqtuegejp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gsjmabpct.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gznthudex.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gggbjvuan.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbelljzfz.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gmzytqiop.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gdltkgwdb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/ggmnduppj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gaupalpvi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gkkfvvnrt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/ggveocasg.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gquhmzjzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdepaaji.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gdqyrrlvt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gcdtwtanp.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gkppxyrll.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gopprmjuc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/ghqiogcap.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gsogpsadx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/galkrypxg.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gxlozrzso.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gzbawyrfm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gqyrtkppq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghiyjdvjy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gckdhoana.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gxlhmbdhz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/grsnxujlh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gkjcyeiee.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gfxcdbdna.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gzbbdflaa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/geqhrdwvx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/guyubwexs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gdagkmjvc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gjcoclmcd.sHtML


<!-- 参考信息 -->