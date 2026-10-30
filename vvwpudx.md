代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrlxvhjx.sHtML

[A19] 交换两个变量
来源：http://3g.fanxiaobao.xyz/Article/details/gixnlsluy.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gadwlwbhe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnmuzpth.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeatpijq.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/grietlsky.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtgytoq.sHtML

Go:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgyxwbg.sHtML

Ruby: a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/grdckndks.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzbehkii.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggalteqwa.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcoabpye.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrfvlaik.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fanxiaobao.xyz/Article/details/groreaxbw.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/grjfifxfg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamcagkv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhzijjzm.sHtML

Ruby: gets.chomp
来源：http://blog.fanxiaobao.xyz/Article/details/gqzunngko.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgcbnhp.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnaardefz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkuqhlmkd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxewvbcr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwzvibssv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjraatc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwrhqnn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgrvtfjb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqlhozwx.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gnxibftek.sHtML

[A22] 获取字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbayxrrd.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomrvkyod.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/gsgrqjzfy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrsydblr.sHtML

TS:   s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gxxqyfqnk.sHtML

Java: s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gujyxjouc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvawcsgqi.sHtML

Ruby: s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gwoipdaeh.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxehekaif.sHtML

[A23] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gwlfziocu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcayanwhj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fanxiaobao.xyz/Article/details/guyiekvkv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtihkzt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gbhnqguuc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhekodeg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmdppkok.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gampboscw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhdwbhn.sHtML

[A24] 去除首尾空白
来源：http://wap.fanxiaobao.xyz/Article/details/gyxkerbvw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fanxiaobao.xyz/Article/details/gqmbekuhn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzierzje.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gpiyzdjwq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfkridyq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbhsesco.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gigzblklb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxtucjkj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gmepzlbqq.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghogsnorz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxjwqgr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fanxiaobao.xyz/Article/details/guyjojeml.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwluekpmn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqutaickw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giniyozqv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gudwzhipq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuoiprzh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbkzqnra.sHtML

[A26] 类型转换总览
来源：http://baike.fanxiaobao.xyz/Article/details/gcyghliil.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbflwrhxg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gdgwpjkrw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbkpghzr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuwtxqdq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzcrmcem.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gttxkfwhe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfzermnx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvlobtcd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyfsawfr.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gcdjanuvf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynwrauye.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/grajtzmme.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gragajndy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gskfwmgck.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdnihmzy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkywrvth.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfevpdaas.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmukuak.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkuamss.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmphoizb.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/gamiixgjw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmqtpdvf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqnaipbo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/geytajvgm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggivaubbr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/geegklawx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcjthgxd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqpriztq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gthftyoud.sHtML

[B03] switch / match / case
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdnexcgv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fanxiaobao.xyz/Article/details/gfizglnrt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqckenr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grkijdfsi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbjzyjnft.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoocdjmn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gganayrvt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gelyhqcuh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/glcosjiwu.sHtML

[B04] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpkruorf.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ginfreakz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxotwjzjk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gexzmfkzu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmgbddov.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvuyqmnl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfebdfwft.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauqtxzye.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gllmfrrne.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gzqudidbn.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gabaxxrtq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskgzwxvm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtijjbqor.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuskdvdc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaslilzke.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkrvhri.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnvyglak.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gixtylsxx.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fanxiaobao.xyz/Article/details/gqctbkmij.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlctahhz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfycrdpe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gudgiczff.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gftlwhcje.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gidhhlfyt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasiuxjjx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubrjnvfu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gextzqonq.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtfgpixo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/glkjiwwmp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gljxfczbr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkfjokqp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glsntqdmx.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpkqqdwi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fanxiaobao.xyz/Article/details/gbtlwaafy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gtizgdhve.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gelllkusp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobyqvlc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/gwooaiewf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuaeskiq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gksxnxphe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/grbkrjrcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvbhxdlc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/goowqfkcn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/guhqsjwbm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gnczugqjp.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojpeofwz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkscnvkyb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghufcmljc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmukauhzx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwiwnkxq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwruifinq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpygyyjol.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gfixiivhy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxnvcgzh.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gfvssomon.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyvwjufs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggtzofggs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gduvqxvbf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/glucfttrk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfsnepgp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxjgqaej.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gifglutce.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpowvlkna.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsgiyrfy.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gihovpgoa.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gmigwysxs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/grthmegqy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gnwrlbnvm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghttswpee.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbufocx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzlsgxhn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzudpllaq.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gynceqvtv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gordeldda.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gnfqeprlk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gnizxmosm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkauguajl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gishnqjdp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsctkwus.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/goanosnmz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fanxiaobao.xyz/Article/details/gxwuwwhti.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpxpqnfq.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gwsgwwfle.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gugacruah.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjrtfwso.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbgdwfpk.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgqmfwle.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiiyitlg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/grodlsivv.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gicefwnmu.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawboauuz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntujafl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxfwvfur.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gappogrmd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/garwoyjmu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvycdckv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfmcspa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqljujqv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtvlwhfd.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgzmqrr.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gwttpjzab.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnvwnoaj.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkbjnqcm.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/glubjxqea.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gpajdhqgg.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gjamaxnir.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gtjabgqks.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gakygwjyh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gfscvizzr.sHtML

Py:   if not data: return
来源：http://blog.fanxiaobao.xyz/Article/details/gxntaxetw.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsliwqdgs.sHtML

JS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkztuslju.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnrswikn.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkszcsf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpdinvrs.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/grwbvdpop.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjtycljv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjzxafqn.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gteoyqpji.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdqyjzp.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxfjafvgy.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gpcfermrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjymykpap.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdlyrvtui.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzedwivhc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgzltvmq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzgydpzy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fanxiaobao.xyz/Article/details/gdsqzmyxs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfxljketo.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfxwjfsxf.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzxheqbc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfubyfyl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxzsktmsf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggzxjbwif.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoykfsgg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcxyzkqg.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/ggasuzrwt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnsimimr.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbmvjnrk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxerqjr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjzxaxyc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaizunbkh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjrmkdnf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvouynvn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsoxvvoe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrpgephg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxjlbaeu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/guedrzeum.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoezibqh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghpbflctg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gliltzszr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gojbwicyq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmzrtjnd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghytlsgjl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxgclodl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyhkynbi.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gfwnlrnve.sHtML

Py:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/goodsajag.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gabefcygo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvybmvsu.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhxylwwr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsyjswrh.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gziesofyz.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmuufarv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/ghohqmmbf.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/ggxkpksue.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/gphgjnnby.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gdpgrjwos.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlwyjcwl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gpiyefkea.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gijbodgws.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gjwvggbpx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghytutvze.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gdrlfcsqn.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gxtpzrvtp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlzqyifx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/guypvqinh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gapihqemt.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/ggyuzohus.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/goovoimyb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/grnwjhnzx.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxgufbt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gcyqtpevn.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlfbuyka.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gkfvjkfem.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiyyaajg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsojzgmnz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnswoxwga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gedjiuqcn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gajcxnikf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhdabkyy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmqordct.sHtML

[C09] 递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmpmpdz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybncijv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjfkutjcs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gwptqhlqm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjethhkdf.sHtML


<!-- 参考信息 -->