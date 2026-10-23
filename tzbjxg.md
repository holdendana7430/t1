代发 wailian999

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zfwsfffl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cflxsizt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jeahlibv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjszqzhm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gykowhoq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jzrabizf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fjqdhpct.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxodyrfz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mwymdapl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eswjimam.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3evglbxvy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wbwvwcqz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hsafljuj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jqvljggb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vzrsnxuf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3iuawyqxi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxyxdyf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3pwxdlxyp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3whkirwbh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qcbickzu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3navvzidd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxuqobq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3okivtqiz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhffawhn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhdwdvj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ybyvshol.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bfliliif.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jhaetfgs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3utzifyor.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fhcsxgcm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zdnluwdq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rclvgjaz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3fhsymmob.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tdwyjbmf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3oiwfkeio.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nhodbpqn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3grigxuht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcpqutbz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zmvqmdrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvzxkbjn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pvwiqusk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vozcqxir.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qtzjfzbc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kitvzjwo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dxgigviv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vururqqg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rpwxfrkp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jprxlice.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3puijknca.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xfsyejiv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3leglalxc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgihkuub.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vtojqmyn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rewwwnjf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ggnbeayc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lzyxlbhw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3myymyxtw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ynvuoxnd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3skvfdfey.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cloybjsd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3abmqnbvb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdjvtefb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yifoprsu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nhlwyamp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wbwufnpx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3zkicyemi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3prifxrzj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdoesabd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3djpbnjzg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yodvqrbj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3unugdqvk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbncljbf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibudauru.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3aefysuje.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3clotmebd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3klpjigoo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3burncifo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3lvqdngts.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqepylcr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nuiphyzk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bfnkkftz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3avokbcop.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vftzcjnh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3aunwbzqa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmbxxmju.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qphpvthz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3eagatuyi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nvlvwpzs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3numvyolp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kskxhplg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3noeiyzdw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yydlssks.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zwladugj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gojtljzx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgvtccxj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dqpkbhwt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3kowynqfm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wntlnrdw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lbfbjuej.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uzwvrfvv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qtgxskwd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jopjxzdu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewsskahd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gmuiciwc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3occbwani.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uicxxrfi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hmgakosm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vobjpgox.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3byekejxw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ccsslgtw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mgzerolp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ruqnvrmu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mlvxkgkd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hvhgjbsy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mjjuiizc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bxvxkqyn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsztphwc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3okfupwqt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tpnevpis.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3utasxikb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjulpsso.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hwuhmqnl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3sxmgbqvh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqlueetp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qhprbaei.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xyggmhgg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkgsttcu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iqbksjiq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gltxvavz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtndlrmv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wzrvaqzg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3prvmokeg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oicfkmno.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iloyiafr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wsttykpa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rlnpbwtm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3shiqcbpn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ykdjbvsf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ymkyalgx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kiqfkjmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nnocdiiv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qlqpmfbt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3txvlzafb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3trlrnoai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfprgau.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wetqjlxm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3epybuned.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rgcyhumw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xsyrlhlo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iedvbmxa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jzjwzchf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3opzpbegb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zfirbxls.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mxapuplw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cgxubwhu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3sysvornz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ickzjgvt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ixwaanis.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dvumpbmf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3umsjgrns.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmkpdehn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpdythlv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gaeymoav.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wflolgrz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3riafhrvz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zxnlaudp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ansevoqo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qagcdkql.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qmlcyxdx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3anxtsmsf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fwnyjiow.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3csrkbfut.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wttjbujq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zkibaiow.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ywmflwak.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yfpsfkqz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ufwcwqxy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kdbbpqiu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rzmrjahx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bsmtknim.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rkyjjtvf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jmtyrtqr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mbrogluy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3txsgdfps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjixailg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sgvtnkhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uypycxpq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjewefhn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dwxmdrrj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpcqqysu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uhxpfcda.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ihqiqvkn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mprsuvob.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hsmsfpkk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3eqcwxwss.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbqmufc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifgfacvp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3cigcttoj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3svbxydwf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cgwyxanp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiqcpyzj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hwpmvuvn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zryseais.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vanxgcdu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uuhdrvpg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqbjqcdd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ughxrvxg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jigisvnl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pukeypmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjhcbgod.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gxzntuth.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3eeiqocus.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3yemdnxme.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3phcpaeav.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3sresjsnu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3buxnxpws.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3sukmgpbi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ewohaqdv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gtzdfjxx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kpuicgbu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uhtgzabx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jrmgzvjv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ksecqkrm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lvovfbxm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cxroxbnd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wqsndsob.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kqxkqebt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3txswwmee.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fzfqsxkp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vjlpawam.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kkvetliv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iytlamce.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sboqbvmg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qdtcawdb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wrgbfmhm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eojijnea.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cuacagdy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dovhkamo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nxfsuxjn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3aypwagqf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3thjrkamy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3twqnpdqd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nvkovdci.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zeuylrwe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vckdleir.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xfynbxap.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3upyxpljj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3krostemm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlnlndv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ncqkmted.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yfryrvrg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qcsnwqoo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fpyeyezf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhmvrhyu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3moncaftq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ncyaatco.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnuwxfgq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ewlgirpr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3miepwnji.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3daprjhaz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kazbtfnr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rzvfrvtg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xpmzzdus.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3latkyyii.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ydttwctb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3iizybfyo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwrkilv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kfroaioq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qlrffzok.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zxpylgua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3yemmdscp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eiujfral.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ybugxlve.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lsinlsxt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uowwzuhw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dklrxetv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eeshftlx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tfsbdvjb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3idgkbgiy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fsdhsbix.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ocxgwoig.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rqurqwnu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xejozzdn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ggutizso.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qfzfjgxx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zkayivzs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rpvhhotj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jobtrgim.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zjwigozq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oqbafuqu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3djmgrure.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3slmzbqis.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3misipwva.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hccggqzy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3keikhgpd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oqkrncqr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3htlwufyf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyeirouv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yckxmcan.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zqqoolhn.html


<!-- 参考信息 -->