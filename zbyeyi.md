代发 wailian999

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rkfojzck.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2sujubpxd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvykhbgg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ltebpweg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dwtqwomw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uodedvbu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xonkkwhr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zxijhzpp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ubxjaqms.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dzngpttf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hynlvrrx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2exxtseso.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2egyrjxcj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dokxears.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mkhfbdph.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jtyxrnir.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqsazear.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2noacmaxv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fvavoycq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2npbbkncq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcaibalq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ujnubpqi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vgosbgpj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jxtbobaj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2inkatxfe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2teslnasi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ekvxrbna.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xcbmcqqo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2aljnuxis.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cqtilukx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2oihhwjys.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ttaenarn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kmmphtrc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hrtvbmby.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyhzdzy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2bljmcoga.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ljefkdob.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dbuvpyex.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lijuyezo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vklewnlg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2auxjhpow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtrsklgh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kttwxrbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qudcksmg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uiuwbbec.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nhvcscxg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wggxivmz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nxuubfck.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rtponntl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ojjzmqoy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fotmwljd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lacginzp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hliooqic.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yvtazzfd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2crafsigz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljmsdgwb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2otsioqnc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lsbpdnaj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zjxeveuu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qvwrzvbs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xanvrfwa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xuvxkiao.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2erdpgsjd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fuaifqov.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaeqgume.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkbqble.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2petlhrup.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nhjnhrcj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dwogldmc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2eehzqicz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ribgbpzs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2slloiutj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zkwkcvjp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ekwrktsw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2krypmuen.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytiujnpc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzymftbd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dyfidaqz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gtkcnggs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wknnzzwt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tqwnorft.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pyotwpdv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2sazwjryv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcjtboze.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2frrjjdga.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ampjstrq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mevjqyyc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vlkljvim.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2erjebauy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zetrxlam.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdcrjep.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bkzurycu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjzxcvra.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtpfaoum.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzotrorb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ogoxmgwp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pizkrwsx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xeoydkah.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pwothisj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ppvaqzfr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tzxmesgt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aieyhsdg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zjmwodpb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnfhafa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qaabmmcg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hixavckg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nivfqqug.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wwuwrzac.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2yqdbnusy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fqsopwfd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ezfntdua.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ynggdmsx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqkvcash.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nxmqsoss.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zsdosydp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bchaibvu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dajodpdk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbscvslq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2whnmihzc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyukmbrj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2txyjimls.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqekqfao.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmxhrjs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2aenaqidg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2twhhuiyq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ixjrdvhs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hynadxgz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2luvwkkzt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qbzrtafn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ucpyexln.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpxninnv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2koluirhy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2afkxwsaj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2limvzhjz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zytzvkbv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lzhbjcls.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ntomrdlb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gszomyqk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2potwkzdr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jckexipt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2slwzogtr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2whzhxqap.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bakdsgcu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2miiqpkfs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xofysbhy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2okebqnbz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2itqrndne.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ehlqapzj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fexfwyhv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2euhsdolw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ixydbjna.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dcluysgi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gltjwgdw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yaxceqzb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qulkiiej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgalqzaz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lcwkvdhp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2erdlczxe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ukguzbck.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vbhhcgng.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2clrizjrf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lzlnoibs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2erceoymj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2itgiarnk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nulcrtmh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lrevtaie.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydlclccq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyixivym.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgyrgll.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxevijxl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mofcbwxg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2itfphigj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2csdhzghk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fwetzogo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2igoyuacz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dunbmflg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ycilknwx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oecwkdiw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ufdyfxak.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xfudfkft.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2duyvukur.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyykzxbt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yjinzkcu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bgctxpge.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nuxhgwtw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqlirpg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xgpqpxoy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yikyxilh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goozfcfj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wvljggjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjszdpdg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2scsaivec.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wdpeezhs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2spwkdbcp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bymrgqrl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrsoswoi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wutvbasg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2somgtyuq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bfpidhrz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpmwcyka.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2csrafuyl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nukbuadb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjfmqiol.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqpxfis.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxbpgrg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2arojoreu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hshkpzxb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xqtgabcl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wmejxpjm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wbbqxkjg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yzjjglgy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2duqvqyqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2owodiznf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fydybfce.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kpjpsoly.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wxgezihc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ydsigaiq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hpmlxlne.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fejboosk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lswdtimv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cktlfari.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dtexslqr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uovualcz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zvefpufm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vxnjtorq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kkdbarla.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ltieidcb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fakpbbia.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pcpkokyo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qbqevovl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xxlpmyzg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mbypqbjv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjiciv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ivcypcew.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hdoqjinv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ajstmyza.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2umlrbgaf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zcvywail.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sdetkers.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vxgvdtyy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rhvtyqmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2moqwhoko.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mawiewdy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nhqeaecy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iznbcujm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kdfjdboa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mugacjnu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dabvhdhw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rnqizwso.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgfgtsj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yjuctint.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zglukzno.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnxiqnh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rnanjejd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2upwkbyjd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2idwqmchw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2litgnpmf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwnxkpt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2upsbufmd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dthibqce.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdphrjz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnuydoed.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nexjyylf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpvkfxkg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gytlngps.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zuezwgxx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tbplyejv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wvpahsdq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jtvapegf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hutqwwmj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wasgkadb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tjdyynqm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xcxwcafb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nhlnmtak.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2totqghfp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2sesckjcn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zsctpoik.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ezhoczjv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bzbapboc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zpqxotnc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tzcwezgz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gumdcnfr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2miijkjmt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dlmgwuoj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pnlatoxl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hjkmvzek.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pnjvfolp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2amodzfsk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2plcipqeb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2iqujfdyz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2shvuwhwj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vywflywg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oobuuomb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ptddaheq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zhsnmhko.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fyhhpzti.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ellrvizj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2miuqoxss.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnnipjsi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hxikdhfu.html


<!-- 参考信息 -->