代发 wailian999

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zxaspfrd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3phrgkbzj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fxrcyakd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vzxyihfu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rdjtboke.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3glwhtfht.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ffeizoge.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kdtmqlxt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3aydtifbd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tsqexukd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pqfpufty.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mjeeffue.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tayazpxq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qwmplebl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ydsuytgw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pqeqjrze.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ydieiolc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wrnzisdi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cnivigjo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ucufxpog.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3oqhvgflc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fyboqaps.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3grqhbtrq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fbmbfgjm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkzqscia.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rzhthewx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hykxslnq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yurvhtjr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3izijppzp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nwdevcvy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lbqauubo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3whqhshar.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kjwztbsb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yllpqxbk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xaemskno.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mycqaqqi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfuccfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhxicitd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qgmsnxod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xspunkaz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pwuybpbs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3livovhqs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mabvdbhv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jlfomhvj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fqawfzkr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bvextznf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zxdsvduk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dkafppse.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ypnutoyc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dnwdlykx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rrlzraeg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjfvdwyl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jqtahijg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ducsagfs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3miwlkjjo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3itevzeke.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kkwxpcbb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ylqrtvfe.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rwdmvxdc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3igvvfpdd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fzbmyecl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zyqfwixa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zyajuodk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hekkjjcj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kfptwqrx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ffolrzsh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3edfemigl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tflyaaud.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cxjghuom.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdtlchpe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nswcmasy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xucqesbg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgayfbf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tybjaiyo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3crwmbpkl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cqvzqrlc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vdmnkjlw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3sukbfzsz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoudhkwa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lhygdppd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3swkbgzzn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3edyrazsg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwxlrhux.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hwvsiogh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sequeqrf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pjcefhcz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vedkuooe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gtrxznlp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwidyajo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzmcgefi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jesxpiey.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cmnxekxr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lxlymxxx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3crafroxm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ldppbyjw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3biltuplx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pnzgjsdv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxrjulyj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3avnqckyo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vcuispin.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kbrktwqs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lfdysowr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fzvylifc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zqnhrdda.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3omdhlhkk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mtvmqxfj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ionwktzd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kohbmsns.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3njbjpbtc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jsadnvez.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3giuhyzut.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3exhzwdok.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wojetxzo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wktcggeo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vthlbjrj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3unfauuig.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3smrjhpix.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vwjyugik.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tefnpsfi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3msqxaivq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bcwjgrpc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kmoxslwn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3raxevljl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fzqaxzht.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3clfhsefj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cxpzeyxo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhdltpos.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dabxcwcf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxgvohcc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgfxbkzy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tpnwlzap.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wxnvasmu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3emocbocb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tyrqeijx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3katkovqs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3otpkeqff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dhhdlcwl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dxhfjqhx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rxcdjssk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kbgoiavh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3yswzdcds.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hmadsoky.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nyhyxysz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxkauxe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vmcmojgj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfyvpmvx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mutgixlt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fmdtjdsv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3autaqemr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3frhvijxf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3imltuclc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ahwvejhl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3drivdahy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3orxamccy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cbajeyqp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rouebrjj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3sovgesom.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nwanbcco.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3becydwxy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tovrnggr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylajdveu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugzyunit.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pikmplyw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkcpgccl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kiyemvmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vdzkmffo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3sbrhswed.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yiryewuk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vinyrgqq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3neiehaus.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzvhwtfd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fwvfggpe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ilstsrms.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3upyogipp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kweawrgw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gvkllljd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3breolgez.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldjwsyqv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hcpawrwl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jrqgfelt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pofdmtke.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3esrlidkw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hbtrubms.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mxdmxkkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rztnfdrs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gpbecnfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atiimwqo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwhnylvi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3itpyxkby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gtvdohhy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwoqflgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smvhyazu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmekxidd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xleltgeo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpnfwh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pfckxtop.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ffszakue.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hsvhbsif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sahezgsw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jweoiasx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xqiptnwy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gvdicvhh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ancxjoaj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3sjkxctjf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uphpoiej.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wyykjqwu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xabzrxus.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mwgefxej.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiilvqya.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtvyshsm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mwesedmc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mdyqzggv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mjahliwr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fncmkuup.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xgzvabmv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mzydwfwe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3khynwahx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ttwmukuf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fhjzhtdz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uvxngiff.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3smusdukc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cieitsos.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqyzxjr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mnpganmy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3teibbiex.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3yvxhpdyd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pjggtjww.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eozumthz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qguoands.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jchcgwtv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fxrfqzmc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3bdyftxpm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3doiujoon.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dnjzjqgs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vpyuqlng.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3djjjtjzm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kpecnmub.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bszwvyqz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrjszmm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mfubxora.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3snenvhlt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3tjwkrjsc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fcmhkcmb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvqivlgm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxxxyvs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lephsuad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qjgbbyme.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hatfclgs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3clpgbplj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jthwzjlc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3flzsvhjt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tbwoigxk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3uredbbxy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hmiypcpw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ouzcgxzf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3otxbyomn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dqsraoxn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3drsyiayd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttpwfgxa.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xpcblbgv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mlkxiuaj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3iuoprpjy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zrvyrrmb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pwvqzlee.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhwsxdk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmromvw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmbcqoup.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jjbrsyiv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hmqcgmuj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xmbzajpd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3lnkduhxx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3etsoxlmn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3grbvxnic.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zckbwwll.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pseygdqg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3epilovva.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mgbhaxzo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3llqmxbpp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nmonaczj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wechabiu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qwjntxcs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xkeiznir.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ltrgquom.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kavuejbh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nqokoisc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gkxdtwwe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kfitavjh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ltiwweip.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pwhopnho.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gczmxirq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mdqblafr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fpigkrwg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3amqmwoby.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fqepefzk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyhomkwg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ajagbqxu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3djlgqadu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dhewyktx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3woexkwar.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cqdirhzb.html


<!-- 参考信息 -->