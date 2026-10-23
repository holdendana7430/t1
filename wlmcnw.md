代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ueambtfa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uspzmmlp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3msxafikk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zujwsokk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tmktdsne.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hjzljwud.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yiwuupxz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ypdvcmli.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jzfeuxzk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3buuopafm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdoeofzw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3sbtksevg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3djobpdbd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qolwzkwr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ytayjuhs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zcetxscs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3trtwvggf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3upzkozqd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nqxmkhag.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ksworzlh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3anfpszya.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gorfaqzn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3urgwlooz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3mquhmzhu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zexfspjo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sjdjxvre.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rvsqcoom.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vfkogzse.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3vuwjhxzi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cukucnsp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iteiroru.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xpngtjiu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3nwezqyjy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bktdbhgf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jcslgoqh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zprhpaon.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwblmomd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vjmfmysd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wckhztec.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iqnjvrfb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ahsxtwfa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3kfpxvegr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yqmnpqfw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cxmykswp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lvdvjdxj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3savzwgge.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yxzgyglf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vpkhfnjr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrfxtyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmprmoch.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pejbxigr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glaekwaj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kstfxejf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wbbfyljs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mvjntadw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nesnjdkh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qoqdljju.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uhwejzgr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsxvrnmn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hnlamzmm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fjjenoqu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dxhqgvmy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ktrmyvox.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3dgpghckx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ofelyftj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uwxozxxz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mjizbtsf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgbmxhcq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xqnhayaj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ggfsqjzd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qnolkhzv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3csgbqguu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zascmdhi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wkyevqgt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3siaievks.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3htecizvl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jdxdtfvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nsuorpuo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3alkxikyc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pkegnrwo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ggmcwqlm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hyxkskfu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uyekzxfn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3asuyvmmx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tgumxins.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xudvvizv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3sxvkvfll.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3erzjcspv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zenslpiv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pejtpvfh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcehzqzc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dzriafsi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rssqhjjn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3paojvvgx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jotyiete.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ztezqixr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vlvlghpf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3sszathdk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtautdn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yivjvlpa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uonljghb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rweofnrk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkaiiwor.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3easraxib.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkagbwf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ukumnbjf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ilgthach.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gggcfsen.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aejtlcye.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlzdpvbg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxxwgvuw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoasyaap.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ijuhibqf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wvrzexxa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3icmecgri.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qxsapadx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gbdbeuau.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vjkboglj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ufcyvvtr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nhrdxpom.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yxldajmr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xojtmnnu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ttonvzqo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3copemkqa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mczbccyo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lejtkdqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zgzfdupw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rlggyvfr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwiikbyi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbmnkaui.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ahwtydfu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3iqxthqtw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3odxrbhiz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3adzchzne.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wwxgnvtd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3sqeuutbs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zsvbgjpo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gwktvrhd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dvymuvgy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3roiwwegy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3atpkwcap.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lgvdznym.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xnzobsdv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ibrtcsfi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tfiuolob.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujbvcugc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3borzwowp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3atohthjo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xusbsdiw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xuzorhsr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kgjfeaal.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3skambzgz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jpfnmrpz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3doxacnzi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wukdjqqe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hvghcgpl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3enfuqoev.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ddyzjaoc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vatvbagw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3iusdtvec.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ftqqjjpb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3umzlnawc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktqhdmsg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvcieuw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pmpjxtvo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3egmawsln.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kezbbdjy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bciepoip.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rdwnyqic.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wesnfgxs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rupcdetm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gampgrei.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sfgfihbn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gkhvdxwe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3foedmbkb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aspgeorr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nafxffue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqqtwdoj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3unhamrdr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ybhyozrx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jqfogigp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mjddkyyz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ncuiicpv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3erxafsnp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nlelrpwv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dygjgdmt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qoliidce.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fiqrsohk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kaigkcqf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rjlnxiie.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cmfyqqbx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hgyodxtn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vnuzfxrf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3trzhtdnm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rbvuelwf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ekwpugig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgypnboa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mmclrzhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svlcrjrs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfsamtor.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fdlebtrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jstzoyof.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggkjnvzl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3liesuzte.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mfftbtko.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgcnzpq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wxykeiym.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qvphqqfu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kemspnfd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jjqyzfbu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxohxmwo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hewqecei.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nmcobszg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qopqstuy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilrnnjme.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rkewoixy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3puurjsqw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3immytqpj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qsqnapvw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3valghqtn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sihevihl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfkaumey.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exukeeqh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3datpolbh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3eomlgvjh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xgulfsim.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rctqcdhq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vklaznwv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bpvytkgg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zctzzldd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dhhnnqvt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wknyckis.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hpegybkp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xlurgejb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdjdcce.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cbojehka.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gycuplfg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bynoeajd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jbbookew.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tdmbznpu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3aytikzoo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tjwcjmxk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3folaypge.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bnxsglwj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uevwltwb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vkrvmebo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jwixhnms.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lweogeyu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xtsfmpac.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qmscvips.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mddfqmpa.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gtmkwdfn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eimfmruc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gifuyojq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wixyirtb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wctrnafr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dtytjmtx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bpigtixh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3livewygt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lxwfyewm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qfidgfli.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3izcwoxmb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dkjjrvvu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tsixkmhq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3anopzptt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nromwtzx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ngaiknfa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cpgdebqr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ifopudvc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3aoulhyyb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eaibvrgw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jepwidin.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfmrbbq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bahajtqp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oxsabezq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ndolqrvx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3eittryvd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hwtcdxga.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3edenkhdf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qkgvirzt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iryvubvu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wknvhafd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qwreufgl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3asxmshah.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ddmvtybu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klgdmxlj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3larbcvml.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cmzqqquv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pxnxjubm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pswjmxrd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hkhtbrte.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rrevtwov.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gqsbskmp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rynzpnub.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ducirrit.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jefoebvl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uskmprsz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ftgjbkiz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kkstpwta.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mkydsxut.html


<!-- 参考信息 -->