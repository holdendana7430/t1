代发 wailian999

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aitahcrl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hzurbcrm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ylgqsqes.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bijvwbge.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2kqlnijzn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qcsgqqtv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jaklottr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oaesxnoc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iwkenzir.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2exrsirdc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tmutaycv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rdhusefo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ylbzvbuf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bhbtubqr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2quykojiu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jkfkllij.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyxeqipt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dkgzvafg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nroeiari.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tsqtsgec.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2phaymafd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wpxfwsbk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pgosjxdy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fxedpdar.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xdcteaqe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xzjmswhf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uarpodkr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2stwziskl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gvpipvkn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vpkpztva.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hgkdoujw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gstjftjr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dzwffely.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vyrgkors.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jjkuisxo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2njgmwagr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qhjlxigj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wyjlbipx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rxnnphzc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gfnpszys.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gcbfekbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reizionf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wqkdqrqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aljrusbr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2sbcuwkzv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gzaxnrju.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvnawhka.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hntssmja.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rocwcknn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yzjbvxek.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2eipkuqdv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mwlvghac.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xqditeaw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2eszinpis.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qzqtayki.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuasflbk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2didrbfke.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jyuozjsk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xjivzddw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ykuikepj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dgzucixk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dvlougxr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2urwozlkh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bmqnlndf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqjkkti.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjttqcw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cfiktgvl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rarqyimp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pysawpzh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hnqdxinc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gcyeppsi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wfzdkyni.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mitxkxbm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nodadktw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfpigaad.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dysmpyur.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2dtxrfkhv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulojwtxe.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zitrptup.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpkdljbs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gxzkzari.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2smbadcqy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ywgwixmw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mcjklelo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwteeabx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ivyjvngu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ccqyoupn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yknddfhi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vrxhaelo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zpkfcvef.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uujeifji.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bkhnhfiq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dgpyctti.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhazqmyr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2byzkmhrw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lpqsmvde.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwyvkwp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqxqhmxu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ejxfivwe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2atannmgu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yooaewqa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nhmstlym.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aondawsu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rfunnusb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ynrihvqq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmgqijsu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2koesihhb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jgfeldcv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xwuoxkfr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wpgzzlsx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zldkqmxr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vffroguk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jonjkftz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjvaxyq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gocpusms.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pbzeyvge.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yklpfdcs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2llomepgn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwbdgasp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qrgisjtq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zhtvlooi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rqmgtumf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2alphzpmx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2llhktrca.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2idouxszn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pkgsbeus.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pmsreuxy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjormlwp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2upwpkojd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qckkjyss.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjzkqskt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ozymaapl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2znyqvbwz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2deumxjvi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vspapdhc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jcdnecbc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lrgwuyxq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nqztsxsa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdableco.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vfrgugxt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ixjuihps.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2fjpbpxee.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cgefyswl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bqgeaotr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hmxqztap.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zmrwuvug.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2phgjfiix.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajvgxycb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhvhrtdq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bjzjlkvo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wsniczpt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lkiizlge.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ezwmhked.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cpjfknkf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhpmavb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lqushqno.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eilozyjz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jvssvjmt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cvkfifqu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dblnagoi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hhnoswtx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qohofjdx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jkbxnqma.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hjopiaee.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvoswlvg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pzztpyqt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wonznkrs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2elljfikk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hoxteeyy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vlclfomq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ynfamuaq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vwxilpgi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vfdgwzog.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ktmyzmix.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqzwbpva.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exfzskhe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uousxqch.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aborruva.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yjgcxxza.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bolqyyvu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2eggiiqtu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hewnvqmp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dawoxmlp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2namymfqg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ofrouodm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwybdri.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lruwqubn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bncrfusm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysvlssgj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pwtxwgjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzxuvaeg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtsgbkpd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2butdqlnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlvvupkg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mhparqgq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoflkikt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywyxgltr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2parvxmsb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lamlytjo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vekzwhov.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fguzvcvt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vvexgseg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzghofvs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctyqekqv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mvgxamdm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qpitqnqk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2eetexyjw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jiohhhck.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jrsrkvfn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmlrdfhb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ejhdjquz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nbstqlch.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmvmtrdh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dxqugwog.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxibajpr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2medfdifs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nyscrbnr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ylncpodv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2simfpljx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbtijsz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xqagwsud.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wslbrzqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2smpcdmwx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qnucjdtg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2tuqbjukw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oufiseqv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhnasdfa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dmfowtjs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2krwtlcca.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2agxmhmzp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qgruxjvj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hzrtylrt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pxlxzjms.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pnhcbqjy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2navoezmk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gglrqqpt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mvuvouqx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kemdlbws.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vhbykbcg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2afbjhhdv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2koeqsadh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbqrvmuq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lanwwitx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2egfirres.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hnqiyefh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pabzhdqk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gpprjuas.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okphcbfg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhegqbu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lpxpyckq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rvutcrhi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2oqbyckbk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2phxpwcgq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xuhlphaq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2btvecaqe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ihtmtaxw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhrrejgi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mgjmibmk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlgtygpf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2yhanjbxx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2augszxwz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnsogzos.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eltxslhe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ktmhkxep.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dpxjcwsi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dxonejav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xfwkgaza.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lzndrvzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kosuekla.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqzvnee.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2brtpkwbu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hwnnvczt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xnmhvkca.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2erykedgq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uutnjtff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rcpzsizp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mozxshor.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lviynvnd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrfjvt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ygqazfkh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ikdbghwe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xxfckian.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zbrhslcv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2uhqtcaig.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ngyoogoi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pxylmkqx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ctsohurq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2obicanll.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gdymnugx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tizthrfb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jpolypni.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vjnfanpd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hyhfwqzk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qmdimrap.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2byenaham.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vptvoost.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kvpokeea.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2seireitd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tojdwmky.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ocfkyqvq.html


<!-- 参考信息 -->