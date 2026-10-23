代发 wailian999

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvcsjzvk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pquppesd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtxvvcs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ongaxjxj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3uaiyjnig.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kkecsdml.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ystqxhce.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtagqygx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ehxnhqjz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fgzjqxwj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wdtixuiu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yrbfkqki.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3htduoxcm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3favybceg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3flcrntxz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mectlski.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3kxjggrdt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wdbwunov.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ehkazgfl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fdgdkgcw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plgtpubu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xzyqxptw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aildlcet.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vnlebgue.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gmdzxgpv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3kawsixav.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yvzknone.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jxwszitq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qufmcxcu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vqnxahrk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cjscchle.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwamtvnn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zgomthnj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jplzymil.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yjftgtgp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tudgsbrc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ghcaixdq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3noqrtztn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3thquytom.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ftoucuuo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ynaqxpqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsslslbv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nosleeof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3limhjakt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3zvanmbvj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bownmhzn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrafsyv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uorcocvo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xibwokdq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iihxipxc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lsiunsib.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wkieebyt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mswcxqcx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pvgrgpvm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sxskjorz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rgnmtkap.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yzmcatbw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mtvrjoxz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fepdrhok.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxklnrm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3elhsjnix.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vedjnatz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gzpzvfpr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hqllaumr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqsesjzu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oemgtlum.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ykwkajav.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuynpfta.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kffnbnje.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tosijzgj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gyjgwwjp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wnclefuo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mlrdnfll.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tilkyned.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqnyvyei.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlglfqsb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xwzkfosj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ccytrigg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fpwueuhp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbnqwnx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bomoxyrp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3enfjrcfb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fypcycrp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3boqnydmt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oxlekltp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3esxdwnax.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qucdvivf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qliozwgk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqjyjnmq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zsdrpysl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kjlezxmt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxhwrowh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mwqgsmkj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3msoqgfcl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tytddglw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fmuqwqco.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ydaupgqj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xalzjbiu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nmbwnzre.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bgzxarnm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3kpacvvsm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3datuvymx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fwrvksij.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pacuvsnv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rhghmbvw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wizacwwt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3igikiwcl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gghrafup.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ynrdyqjy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3imfyroel.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vpubtqlx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tsokejcn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ipchikpb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gzzpnqio.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nhtitktb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hfwrbxjr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fegafhyu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3flizgbst.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gngxwbtz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uqaukhxm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wmexklrn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ywlmckgi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xvlzcebh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3blovamzk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3stkbdipr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3icibwvdh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbzxtgn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuslvmlf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ehhkbfmv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3argdolyg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lratmsjw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3avqunymu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rkxezvnh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3utcjgzlr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ybzmpkcu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bjivztgb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3oshowicl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3blfjmcfg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tktkaeib.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ycqnopvt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zqqjnxoa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tbuaaveh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcfsnuc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3eeivshlb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3onlklzcy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3imvkhsvz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gbwscvgo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3faimpylf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qepvxkse.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wgihceis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jomrrljs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3emetpkgb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3srumtilv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3czgbipju.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3uzbfhqbz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iihkbcri.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtykjcuj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vgwvltqk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gcyqgenc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3txkkafsq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xekmttzd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lrvxsvwp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rzpzvciv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rreryulf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxifseu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgelwuym.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3egnfavjn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kfgnrfxm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xaasagjc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bzrwphvf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wjffugfb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3acddqexe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wpwlgvup.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywiufdpl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ojkdwwnb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hdkgmuuz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gjmwtkfy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vdqhfwfp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swcfsdon.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qqwkhgiu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3eajhovde.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjppwxvy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3frtzidrg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zyjthpzt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nvimgvnn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gnlhznik.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tlpezzmn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iyjyrkwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llxoplaj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3drvhcnkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcvcosfe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3eheskqkh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zxlbterf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctvqqxun.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sazsuwqk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqutnht.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drxliaik.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsfpuxo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jclgkqfa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rellepyo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvtpqeeb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mzbabxlv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjtruavp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bztwjlwr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fywxmuhp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3whgyruhk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mveqflgl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nurkliie.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hdisgboc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cwvxbooe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hzvpahpt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xafvrwob.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zhiliifs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3voevixfh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3woqiotnp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3saxrakgi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpcnvicx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bcuwjxix.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dkscvkgz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rcuvkcex.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vuylzmmi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwoovuos.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zwqhrbfu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3itcbrkrj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hpqohcuc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lnkwhbcc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yojiazmd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hnfybctq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bmyyuigd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3efgnaapu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3euwxgzfn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3igbwelqp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3czsmbxlm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lvqsyjgp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jvzqczdu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kgxhophu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vbbukxha.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ypxlcyfj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ifnltbxh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3atmecgdq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jbrlyriq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iuxukxnn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ehfewtnt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qzxvsedg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pvqpkytk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pqkoakvy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hxtnjzzd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdirunef.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vfardmfs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcpvjip.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xnuqfgrp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ymssjlmo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3srsfbath.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kgklmoek.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jrlqawvy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nfpbfndv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlpaqcor.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3siifpgvm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3efioberq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tbfycmpt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rtjkyxjl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvhfrtmk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3muafgdid.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxntaexs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qetocdpv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gjxapgxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fvnqdoyf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hivrpjet.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pjckpsnh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mjrydnbv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hibwkhft.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xnagwpfv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3glbnppuv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3sqeebons.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qdxiqcnt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3okdulnmv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bxckyzxr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3plrwulkx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uebspylz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3prnettnh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3egtxvjfl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uhfaljao.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xlryfewl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bvmilcop.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hdfnnsgc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3krknxrxy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jipkbruz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3murqhmus.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zbhmgkoy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ywiqmify.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vwhzhysq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3uqmbyzxg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zzyldngd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jworskff.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3isjlpzxj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vkmsabqm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ucwuojuf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hghbldof.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3liktzfch.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kkihxovf.html


<!-- 参考信息 -->