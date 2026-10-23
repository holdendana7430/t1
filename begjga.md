代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jnlaulez.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mfelcmia.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qhwpnkrd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bmyauejv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bmhpedis.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3sscltveh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3dcintnoi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ukmwtgvc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzylswgr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3volqjvtn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vmmdryub.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3sqifxdbp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3blqgefgx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fwrtaucu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tveqlbcj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfbfdczf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3whbtwhgy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ybnzmccr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttsphtjt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mxajuzdg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3odmicmqt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gsdrnsun.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gyxkdqex.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxhgckl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mdwffqts.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3irvezivk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3orwjpmpa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3izhitvpv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xqigqycc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ctnkbmet.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cewiqefs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3oknuwapq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iwjyuunf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppvqclqt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3etlorzqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odzqperv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jxjymkdf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tgocqumd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rwqfhjse.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gcfkfgjc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3muldyyni.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3huypqoal.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3efjfvlqr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xpnebgpa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tecuwatr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ovambzbl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nmffbedt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fyvfxulm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pbjghmga.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yuqazljl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3luyfmrui.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3glvtzgii.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wdskafcj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xmhpvari.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ykyqjilc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3fothgsuz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvmnikjs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3asguvwgy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsrlvvrw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfohcwkt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdyebeso.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nslbhiyo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3skxkbdfq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fcbjowbv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pnuktoyi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3flthepkk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3swdvqhej.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lmaqaxmu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yxoudcrf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmbrkapb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3uyduufrd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qxfctmjm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jkgnbfqp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3azfumwhe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxeoiapl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zoadibsf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mjmwiyik.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjiikfaz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cdzkxfbe.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3swdqrqfy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fzxsrhlo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3aziuodtw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3aetsjclw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3sviysddz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydkxlbze.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bztyxpeq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3onyxadzo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xuqeuckx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmzplll.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfvakomx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3phohkyuj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qfnaxaxc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwbexabp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dirbmtdw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvxhylmr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhgwdjzq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3abmslosm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ybiyyvqa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcndvizl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fkdwjlqj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3puvldkla.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ikbiyfnu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zukyvkkt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3leskrxnl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3scpxisni.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3obxwtlve.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kgbcwrtx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mkwnbmkn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3otsessqr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pufgrggc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohhrbjmm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fmtwxsfx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lfupcacz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bjamlron.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bocbnuez.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lalwcbrj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwclvpuv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mhfoolmq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3avlcaghf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmypgklp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lbknnmjv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wqfwxxdk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuqpibgz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3misbdqht.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwvfany.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gjzmkqvr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dvnyaoqz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gekshyey.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3wkqazmuw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3knjezjby.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oqnzxocz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzirqjcj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tjelfobo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nfeuiuhg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pzgjwbiq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dwusonjt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3sbhxdwnk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ajmliaeg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvikmiid.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vsedvfeh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyiihvft.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3jaitmgci.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kgcnecde.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jykwgjtn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rxrolfuw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ytwirstx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3femcewln.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3whonfiih.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emermzeo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wyoinvlu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmbzqzp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zyfrvlax.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wctzkqtv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3idzafulx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kivvwryz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ofbemydd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qutcmqne.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eaxzmupm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lzegojbw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkiixoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fgsrstnm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vlcfpxjc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nqroktpd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uhheqdzq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3arrnfzsm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jayqikoc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gpxmesni.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vbafxeeo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bukhyvog.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qtbnephq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3blafyfai.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kprzndtp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ptqyjnme.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ltgpyxit.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xyckbaxl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ykxghfdk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qtazaevw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tymayyhq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rymvsuls.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zyqyxvhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egrwmyqb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3veuzsmje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gudeagnn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fkuirjkz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vclcixto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sisskdqf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nlpaxmli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etfqzdwh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3elpcdhce.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgxtgdp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfglgjmf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxakncvy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wddxlnte.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fsygoonm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mmardftx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jrxctpmz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqpzqeci.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yvylobly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3whyyhitl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3knuhylsx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eknocdiy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ioibdqzq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gfdxrfwp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lgpkxpfw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrlfyjae.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihseddwd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjdowmoh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jbnvxyyv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3iqmfmxbd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wofatwnn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gyjdasrr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3blqeuwkc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwyxgbkg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nkeocrjd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jkpclwjz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wfkmxjcr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyialbox.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3djzkdlyf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3asrerbwu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3paeiysen.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eyufeosp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gfrqphao.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jlonfaer.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ejglcdie.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3aaalnopi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eeopxjlh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3blykeazz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xzmhhoms.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3odethzsu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fjllylag.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qzyyiosg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpjwuvsb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ktcjfjzq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ppatztkq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vzujmrkz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cbloonvr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fukvdaia.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3npbimlol.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rjsbbhdi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3atgpvpft.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3azaoewsf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rafyvtkb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vrxswqft.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jochebcz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ndnxbess.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mydujtdd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3msvopajp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fanzkdld.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nftfitce.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rposdjcl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ftpszqrk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fzwfruyh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3launuoug.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfeqhwub.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hrahxpwx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ugvowtok.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3afiexxql.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rireosow.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nbdoagkc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kpsowxqz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kayxmidp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhpfzgy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pojmyuyt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pwimpizd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wvmvewdl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mksjzebi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eldhcjmb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zouyrxap.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sakbprug.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3daxxcqjq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xzrsgefj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bxrhjfma.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mbentlok.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ofaixlhy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3odpnuwsx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mzlbssxm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3szfryboj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hrdapqsp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qdfuxlfp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yfekuntd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yaznkaar.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xtjbfbrh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uuuxkxmu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vcxzqzxg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3txlmzjpe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gbbtfgym.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vjblpnpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vwbndtgf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3owmthkhn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jusqfjwe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qplfvhfb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wsetdcmm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gnhfwprv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wvjipztc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jogsqypz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkksgmhy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejzfould.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3msneqnxh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qdsqenag.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3oovfmqkg.html


<!-- 参考信息 -->