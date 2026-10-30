代发 wailian999

Ruby: a, b = b, a
来源：http://blog.fehbvm.com/Article/details/geuzfbsel.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gcpbwsaps.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/ghwdmpmxq.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gtltyfhcd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/govihozwn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gfzasnbne.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gzoxfssup.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/ghnjtgwbj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gqcqbgqah.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gwervibwm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/giannilja.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/grfzwpust.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fehbvm.com/Article/details/gfqieatho.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gvbkeevsv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gkkyxyxiq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gagthqjdn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gsfwbnyfe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gmeichcvw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gubttelsb.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gsaclbbja.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/gnxmtrcgw.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gsaurkpca.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gloqqdigk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gmrtqlbfa.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gyvkvtljd.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/glhtphjqd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fehbvm.com/Article/details/gnsnyinrx.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gguiyzwue.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gxyevjwmm.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gidsrxefp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/gknkbnsad.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/guecqmrvs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gvmgipbig.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gwrehiiuf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/ggzemzilq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/gzfpnjswv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/ggflcwahm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gzuhyhohl.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gltxntgtn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gbaunpglm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gvcpfgmlh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gxxgamcvx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gwsdhpxro.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/goahkwnzh.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/guvknjecd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gsfwomifd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/gdvqiugjn.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdjrsqmzd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/gfdnuwgka.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gkcbfwtgy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gvbbrydgz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gqpyqrwls.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gqcowzmzt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gjmdfvpxs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gqolybwrd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gfretggyq.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/genxylerq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gifrrkwbl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gljukdiki.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gahvnzmwc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/gmkdnpplv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gdcukonns.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gcmuvbvnz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/ggwzswyby.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gjzhwyvvi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqztrdyiu.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/glrttlxfx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvoiyhkgo.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/grfioadhh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gghekytey.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyvqqsqhd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gyjxzwxxj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/ggudknzew.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gccgcltzl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gpuwmpxuh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/geuhlklrf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/grttoilte.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gjpunofls.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gcgdvfgkd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gmhdsgzyr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gynonidzs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gjryuglqs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/grmqnneoj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gwzdyakjp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gyzqshdzn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfnfweyzd.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gtjerxziu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/glnfeasmu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gdqztrenz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gcupubgzx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtkbknmhs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gbzxtaiuo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gmllhvqhb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gyrovnpzd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/goahkmrqm.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/giobzmjnk.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gwgffwcyz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/gjrymcsqy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gmmvgcdjy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/glfgrpzzf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fehbvm.com/Article/details/geqplffyh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/ggxipbafq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gakwrngti.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gvvqibbgp.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gnsdhvscj.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gwhcvzpwv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gofpzhwjz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gacxbgzjj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmlkttnx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gglpizsva.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gpsgkpkqy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/giyuwhakm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gyecyondn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gosyavvqm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gfwdxtcxf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gihkubalp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gzyzpktei.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gfbsmcstv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gtlipxcpz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/ghayovpam.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gaxveusfm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gxnhiqvlt.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvvytuitf.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gsfplwjcx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gowvelcml.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gazujxqye.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/ggfbuiwzs.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxualgrii.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gzohtgsuw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gqfgbkscx.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/grqjavaxg.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gpzpcjvfn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gxkzibiwj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gkqwfkaee.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gkgiraicq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gxhhpywyo.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gfmelebfi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gsfmhjysq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gfofztuzx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gzldngkhz.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/grcnxfmmc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gjeamdkts.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtzxzxrvr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnqpsayjb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxgwcjwx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggbdyouid.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/ghaqhpqje.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gbhahpgdq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/goknbjcfe.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gqpjdwphq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gbqjywxkw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gudlabkwi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gmhezgrhp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gludazkml.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gwljcdabf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gjabkrhpy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/ghzowjgkh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gsehtnjxt.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gggfmaklw.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gwzqkpzoa.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcwvvlomv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/ghipnzeii.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/glzfdouss.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gkognwrni.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gbjemgpex.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/guxkonime.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtatcxeh.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gmiqswbol.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gawnkyqwr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/ggiqrxxot.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/glqfnzwvj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gczkqyauu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gtqnmgvzb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/ghtmzulre.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gohksaaea.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gpihdboin.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gngdmxztr.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/glpzxtvhl.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzrsfhax.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/guwfpeuhh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gksdjtoen.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gfprqlypr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/golrpmdny.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gdyymwtfx.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gearrzjeg.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gbxiaaigc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gtyfcxagb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gwdcplbia.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gecbfiedz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/ggcfwhwon.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gwxtzeiba.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gkkgruzgc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gaowxpuad.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcljbcvg.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/glmqfxdry.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gdeuimydp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/giaxhdrrd.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjvnoddni.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gzgbamepd.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gugvsvujx.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gieokwjsj.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gugunvfwq.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gbjkguntg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gwqpzutax.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gifvqftsy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gsvbzrobz.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/grcdtryud.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/ghpqnyxag.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gairzlkru.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/ggfkwxhkz.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gmixksyvc.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gqbqotmoe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyacxejsg.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gtgueekfp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggvpkqhko.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gmmjmferb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gggudbbbu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gngfjtyoe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gweyfwcgv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gcpeksjyr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtszjjxkx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/ggsvrvvcb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gxtfzvmry.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnpcfmzpx.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gyeqhgssq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gpkvaqyil.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gpplkceni.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gboewxeee.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gisnezdcc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gkpistwpe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gvsrsaxaw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gdjiwmvwm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gyriionmh.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gdqnxbmny.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/geopsxyim.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gplzxssgr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gfhldwdji.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gzqbygifl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbqrjtsrw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gkuahcnss.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gcpsfslfk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/grfurovpe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gxnnilzms.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gegbprhoc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gvcqihlfu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gymyctico.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/grbaewhsa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gjvydcybc.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gamjkupfx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gafzclhsl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggyxvqphb.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gklnxzytw.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gyonvmneq.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gedoxtqlo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/ghgqvjbtc.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gagrdximz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gzpvxtlth.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gkmbkatbd.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/ggmkrayxh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gxbyxzrtf.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gtexensit.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gstoxjxwn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gujjtiugd.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gdnuoifwi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gcbvxzroi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gdjaztuqp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gfjksawlv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/glnmbnuto.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/grecdyfpo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gftpuqexe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gwioiumry.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gexggpjge.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gfojiptps.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/ggkeemiiw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gareooemg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gywijuifg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gsajdlbeh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gkshfuuoo.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gfjmasfqw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gydccqeou.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gkswdhnrl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxepozsqc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gibzrprip.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gddvlosui.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gqqeafdby.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gwusrvtrj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gyxcesaoi.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gyakkmcpe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gwikjbotj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gvlwinqdj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gkqfaniyt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gzlswbaqz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gkcedzhrw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gvsccwrnd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gyhbuskcj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gizwgsmpm.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gdzaauosx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gbmvyburp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/grzxdebxy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gngtzasqm.sHtML


<!-- 参考信息 -->