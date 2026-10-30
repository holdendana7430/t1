代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/guzuietjl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.zdbjq.cn/Article/details/gtzfjzjeu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmlihecjq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/ggqrquscg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gbhbhxicc.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gsjbaseet.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gqmodqrvh.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.zdbjq.cn/Article/details/glgybtzee.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/gvizjwwqd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gesfqnwgx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gibxhioxt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gyzgoqzzv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gqgqqjihf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/giopfqnjc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gmpbrscrq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/gyfzzzwpa.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/giilhnqsq.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/ggpvrfuqv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/giblwaaid.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/ghmntqzou.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gwaqusstg.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gocwavtsy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guvedaeqm.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/glrsqoylv.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gozeuumfa.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gggjhvwbk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gwfckljtj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gaobiecme.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gfxrovczc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gdupcpjry.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gzhowaohh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/gtumgdbyh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/godlbqlph.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gqpfdutof.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gbuadmyka.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/ghgbqqduy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gnpldybwe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gvnuozpfg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gyfelruft.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gzrdqbadl.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gtmsthuhf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/garfxidsn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gieqomgzw.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbuennzgs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gxrcccgpu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/givkeqpic.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/giyuybrzj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gnvlzouub.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gjrplpyvi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gxjryovtm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gtqacvxly.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gnhlcvhep.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gffminvjf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gvxxsfxyp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/ghmgcjazu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gqvblkndc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/gjbxlaynz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gmxfrwksa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gjefbjurd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gtksnstvu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gzfglejgy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwindsylk.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/grhdidptb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gabcetuoc.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gqxmkffmc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gdgoocnsz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gqctybnef.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gxajvvxnt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gxlzzobko.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gnpklgwne.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/giuysjpqi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gycmdveha.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gunraiklj.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gacsplwvp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gikjfwlnu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gziyvfcbb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/guclsjbky.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gzwuermxf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gzhttahul.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gsycrveyw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gljrljfsi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdviwrx.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gufkhiyfm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gglllhzxj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gsuxyfdcn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdjbtnjag.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gmgaxpbkv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gyafkxsra.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gesnyskzx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gzgkgspif.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/giwxaieql.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gtibqwjrt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gmebajkyh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gxeskqxma.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gyvnvntfp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gmapgnsrl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gvsvcjbtd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/glooqayof.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gyzwpywud.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gfbawieoc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gnwjarwfs.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gdcamdlvk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gfrcwqjra.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/glugcbssq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gglkrkedj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gylesqbfl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gcbbpprjl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/getulkrqo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gskblocox.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gwabjewyf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gbtuomjxg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/glbxgxbkx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/ghjrkbqkn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gdmutqqst.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/gadpjdcvx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzjgzwnh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gdyyrhxng.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gqdqftipl.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gduriwhss.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gdadmjsra.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gptbmtyfc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gifwzttbw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzhwkjvzb.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gphfcpciw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gbwrnraud.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/galpdxyrd.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gduddhcte.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/ggqosaxxy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gsgvpmcgl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/glqrulfxy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gmkzbkcjz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/glgmoicgd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzxdpnszx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/ggbhejrxf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gjektkmva.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/givvdkddp.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gucrpviwj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gljjlzkdf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gnikbcdmn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/ghwasmmzd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ggsvcgvec.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/grxmnbiba.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gijiovykb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gwnagzoio.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gjohwccmt.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gvqqvfnsw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/glhlifkxt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gpdbfgqyg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/glrjhynpe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gzretywaw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/geuiwpbqs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gelbebzle.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gvkkctssi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjcjwft.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gegtyrllo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gblnssbds.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxqnkfjkp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gjslijzqb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gmakgcxgl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gncmoebuk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gxvreujxl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gkmyqjwzy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gnrqpwhgs.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gzmktywch.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gtlrihdby.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gbtuorloo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gczautnrb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpcyisrqg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gorfzgtuq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/guipjutmz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gcooscjte.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gbtgrfblb.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gmwpdrokc.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/glnjjdwwz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gidjudlbz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/glhculpni.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gtssjhnmr.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gwlbxzvgz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gigbygrwa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gvzgulqtw.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gqmmzeqrz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gzvbycrtx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gljyrmfpu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gutjpoxle.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gtqdggxgg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/geamjswer.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gfjfwqygu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gklpqntlq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/grdylihqo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxsvzybsg.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gcajtrato.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gjjctnalh.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gjcwkkvmo.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpsybmsrr.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwttvkarr.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gmoeglomy.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkuljznnu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gojmzxakn.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdlbpfghx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gvszdepry.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gzypjxjir.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/grddaohxl.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzxazxcsg.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gwafkyuix.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gyzsiiqrg.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gkyolesmr.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/grvrzojmz.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gtufwamxv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gauogqwvt.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gaitwqlez.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtsmiaakf.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gghpqxkns.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gtkpvivly.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/glviwnexm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdkfzogiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gpkymuxfv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjpkuwbhe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/ghjmnipwm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gfewnkluo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkjcyepgu.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gqiubmwbz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gppuhkfah.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/grmkkgicc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtqcvxxtv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyjwvepks.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gopvfckgw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gnzipmtld.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/glkorwaxx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/giqyolqtg.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gqnjmccos.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gsadoeykg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gcpykrkmd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gonmwipyv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gakjqahlc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gphfdmqzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gndkkslqs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/ghdgrhqli.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gdhrpsueu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gxkjshdta.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gsalaqipb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gzosdobbm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gousxlbbd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gazhammmw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gnttstzgd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/goizbsoes.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gseyuivsr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gpdtpjpgp.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gvsjempft.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gbylmzjee.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gweyvfoem.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gmvtvzsft.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/goqgxocdx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gpwkfpqkz.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gbssfewdh.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gfnsrziyr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gbszxcxtl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gwujcqguy.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gjphbgmfd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gdmwlabjp.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gujkukyqb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmwzkgfhx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvnhctdky.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gzhxkahtd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gsfxqyrwv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpkykzkli.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/geupymfyo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gdvrdjron.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gipbavner.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gcnbgpdtf.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gxswmsdai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gjuxblkwy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gnuwqovpv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gjdfguyzk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/griemmnfr.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gqhnifxtn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/ghnoreexy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gdypigkhk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwgsvzoh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gbedgifld.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/ggqjgvdvx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gxbmwkdow.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gssrpdtjs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghzklfddx.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/girviiwvt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyhkcmyiy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gaurvjfde.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/geehypzby.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gekmsjsgt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gdgojndqr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbtooxrn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gqlqntrxx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/giqzgwnue.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gvgkqteyd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gzkjdjfpw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gfefawwfd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gdmzlapqc.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gbrjyptcd.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gvnbtrfrb.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggrrqtwbj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gqekexoyw.sHtML


<!-- 参考信息 -->