代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mixsejvm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gqoevoxx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hwwrbzjq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3knprmsvl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vqiiggbw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pwwcmjvs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hsgswvyj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3edkxjcfl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqfdecfe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gczfnsmh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3biskcepz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lqhktfiu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csetaizc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dedbtfes.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ktsufina.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bddiwskq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rcitsuvk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yunpiasj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zrncexrg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pejzvion.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuphohk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bcgdywbt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3btjgrcei.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3aijdntwc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rapmyyvq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nnueqfpe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhhgiug.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nrgaathl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pwbxphko.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dldauhog.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3htturuic.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nronuytb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqbgqaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlgoijwk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yzhoozoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhjuimgp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cldtevpl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sceozaui.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bzdeagzb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ruahgwcj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bwcvqsxd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3umbhqrlt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ddsgvqaa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3uiktfcdz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eltmmfqy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mvgyprxc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lcgnxrua.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3extkhxpb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3srbyyapy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wpkvbnzf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xqjckykr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3yenwfiag.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dvlwqzgt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mjhrxocl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3friienhn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3scodrfjp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txnafkoc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptktvpnt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vtqxwrqf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwtzczz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lultrpfv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jcpqopwl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tirvmsiy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ivlsanrz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qcoxyjep.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpxyfnua.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgsoxxal.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmosgboz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytgpwood.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3agrtbojk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ncxcvfwk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixizokxz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pzmsuzli.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qzwvjrbw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffykfzya.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmksvnly.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3etjikxxq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qyhitmig.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iujhvtwl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zdnpkior.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3khqmanrp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ukmawuwl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ctusgvlj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaqeqnxg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ojoxcafz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxnhchq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ftaiawrq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mxjvtxpv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iyldqnhy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cmsrdlqg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbjepdug.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cisqkrab.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxjkudkb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjxazvqs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3atrkmotv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggmytyqt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rzvsuwfm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gbyyffdl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3txncpghm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yiwhfadj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3acqmkvpd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cxesabeg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vghlrgyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wsdqrldr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3blskoieu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vpgfajoy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fibwtlql.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwppxv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ehnsyaam.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3srghtbgv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jouvmncy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoqatgiz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qobrwpqh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3igoltvor.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wpkcirdu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkgmpeb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3chntjdaj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uyacqkwq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwfewzc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3imffrnmr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nxeitdpx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3oyzmfxjj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ywiejnsd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ccjzbdfj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oosbvdtn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cqsmhhgk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mbmdrpyp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zrkmgaqm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jxciquvi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fxqtyamr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3htvsqipp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rvucdcmj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wvqkivwr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pffbstlz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dfgwiufq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zlzlmoqv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3prhvfyfp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3prdoongf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mjxmqagb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hkfwkloe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrpxnlrs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtmebzql.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3irdtomrr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qymyjgxu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ntfvsvjk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lhifcidz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ugjdkyyl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3egqstezo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3olrypmzr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3labkykcm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3givcxnpl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3edptaghe.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rcdruffg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qiiynxjf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oadkoops.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpriqeh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuaksmgy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wmgxqeaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3peizettf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3efauitvp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nfezupmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpbsvfc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dceveolj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uigosvie.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gllfyrld.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lsuxxpto.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aztmzobo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xnigakou.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3esphnesd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vmrihupi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3reonugdy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jjsvdiaw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jpyljgwz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dumlshkh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xhcxmmnd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tzqwkzdy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sljbvhvg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ecccffcx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jtyuosbb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gwybrbvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqddnfxh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jsurfsnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwfawkmt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3koqarziy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3biytxzdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycsdgruo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bmghajqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ormxodez.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ommppzfi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cnpaooyr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wtptlowf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vylmtsdq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3enavxaxy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qdyidsmn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mnjykpwb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iukiifdl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3faqtgqxk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xchdisye.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iggazyqk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uslsxlsh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zrqlazut.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qdpqghna.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3brobsucl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwdhbmeq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ycpfavhj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uutsxume.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mshhcauh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dnzqytpj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3esrdtxld.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3recppdsm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kyhetofh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhqfjbxw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tkkegpsj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bamyceoa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jngmuzms.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ebpizfgi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lidkykcm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbylgrgk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkimpfx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3prdgjlbz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fjkqvgxw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3saywkvkj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3puwivbam.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fxrwmdiu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gongbehw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ephfpqpg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pqjpdnoo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ibhiaqby.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oiomojqq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vpyofcmb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jvacpvyl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gupqubcy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lvcjolua.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3agbjfumj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3auektjri.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3phseiqwv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mujxanhx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bemezmkz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ydfoejbm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtsjpasw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ulgpahxq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3kjqfzkwe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3elymhtub.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ssxluana.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ponscoqg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vxrgmmpk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dwvjhuia.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3usksnhws.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3twnkaukn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sowucggb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ibefjzeq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ocxrxfud.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzvqflct.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bjkjiery.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bjwqnimn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qxumemgv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuefbre.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mmhzxxbw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xkrvnmrk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3osruqmpe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xmmzwrzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xdgpjgvh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tnnzljxn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3surluqgt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klsqpiky.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zswupbbs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ikmvevwh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ggmleqex.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wmhzjfuh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3imbdxmvd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ymymdges.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ebrhdhmx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bavmofos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pygwhrhm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mhomwqed.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vxwxrnxy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fatgbqly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oyxvaiwz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jeliimzb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mqpxkjiw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uzrnmybw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nxknvyhz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ujtcdfra.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nzjobcqw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zxpxpsoe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vyhmzzsc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ednbiyiy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qrbfhbow.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gzsfrqvl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fcxoxvyp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iifgwvpb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3brkccudb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cwghocwe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsriydpi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3igcpznpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vinyojaq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iyurposu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bcjfgsws.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lmdefrat.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mtrnmbmm.html


<!-- 参考信息 -->