代发 wailian999

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ujnorkza.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fjevugii.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ihdccvfm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2feaatytl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2razrquez.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dfewbfzw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yycmcczv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kuyuywsy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qoljrbwd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vqtssnuu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hxflnsvr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hosadxkk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztluxtwl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ffdijcpm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hmgyduux.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2belrunin.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kjxzseii.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jqpqliaj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ncwllowl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rdkixrzx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qxwiwxze.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmqnliqz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kesfefpj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lcgqmpon.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wgymxiaa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2thhgqlpk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xmrftiko.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2szcrryeb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xocoolny.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lxalduct.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2laixzkjr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rryeeuds.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qvbpnuni.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nijweibi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2tfuzmcpl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qzkidbol.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2trlmptve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssgoqwik.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gxgdwval.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdcembzt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qhcwbeng.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bnvjohxl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwjrsen.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ggdjkust.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nfctwntb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kezrfpdk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wikkwosh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2taszdmjh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jamzznqu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yokfwqvq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pkxupamw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uwdhdnxf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lxqprxqc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzsuoiqi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2afevqrpb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tjywgsah.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2itqhvhtf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cpdejlyz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2slscnryu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pcskxnbh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eetbrrnu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2seauphut.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbnotkrn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eksrqzhe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mhqcgkiv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pxeofwbu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hwoxzpdy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iyzdxmbf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzimred.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfarkguf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hazdiyzr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hmlxmjke.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ubvpyjcu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2sijnpmjr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jnnacasa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qkecxwki.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fzobbcsx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hlqdcmvm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzodhea.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2whyjqbri.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbhnsoji.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ypzsfwbb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tumxshpd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ygksjbyi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gnoexjqv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2devbdsfn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwsjnlj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yvvrfmfi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jueipckp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cofgcuhi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wbgfajvl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ipxhsqzv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bneitrxy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2krgkodvc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rmvwtsvu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2miopqblp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyignyxm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2igkfgywh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmslygav.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2paevcvki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uemfsmlw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgebyolf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vkllaphc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bednvlrr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gabzjfpf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2diqzcjea.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ifmcjijd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2icfxxzzx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zqedbinh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvstxvla.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aivekdhj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pcdhdgol.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vqiiwjzq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wnljasmv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfggvwcv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2skwswjby.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jytiyfur.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgrloowi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fjqdrylm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xyiylkvd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nmasrnmf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ildfaagd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fqsmxjow.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfkhhsvq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ddufyysx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ueojseya.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mlejdpfz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xfviszkd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vybkumxv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqfxmlxm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hlchebbs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2blczqkeu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rybklggf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tchrtzjw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yvsrurzq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gsmzccbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2leyujlun.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fhykftum.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nsnepnrl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2urcmwcpk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2iscbphkj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hqcxmrvx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hkhmzcqd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jbpexyrp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zdvzmyty.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2juaqwwix.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wztxyctm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yjcxwxkr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2laqwwauw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gwgxwvqn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lujpmnuc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrlylsk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wavervey.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yndfcbga.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jdsbhloo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2trjxvlyh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bwdzhztg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wtkzeniv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ywvvdyyk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qzarheif.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2juyuspqw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckenbyob.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knvzshon.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnctiuk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vczjmkxz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dlowolrg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nwuvvzwb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hvfiiyrf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ubbboeao.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tsidajiq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vwxtugli.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sgfxbwli.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zwfwitgb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jsixtlrx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ysimnbef.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zmjkxvpv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2keioswee.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jotpcwvo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gdikchzi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ckbnhcxf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iehkvrnq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2amsfvufw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cohadizj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pavynpdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxcgbnit.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wnmaybkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyjauoyc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jayqxgrd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tkxqinup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uklgzqkc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jsjdjbhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2htamejus.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wvmcuekb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2okachbhb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qpswikpb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxiubieu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jtpyosws.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ncgdfoma.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2slvpnnqy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdoxbobn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2csbcqwap.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2urtfpqxk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rcjxjoyf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ncxrhdoo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mcgmyuly.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zxluqfib.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfwvnhn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qpbpylgx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mlzrnqmp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujxwcptt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljiueayq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2appgrtij.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrhupled.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2dbrloyzy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2dmnujkvx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2akiukamm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jrciyipj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dlokairk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2eyqqunsj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qxhmfyqq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ceduzxzp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hxndwfmk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdkwwqz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vjysrqra.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rhyelwvp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ebpdmxkt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ryrmcbux.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xubfxeyq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qqpuwwjx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dhlbypcj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2szxgehjy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2prgtyftn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ijimajuz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xaeprxkf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2clexcxip.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ugntymvk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ymjmomzo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rcvkwmtb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hmvffqia.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ajawilyi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eozgboiq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qolebqte.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ebsmaqkl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujtvhmei.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jgannwqg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ggeufipk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nvtiqjrp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zixzjpql.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2weldomis.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2apoqdbxo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pedjaavo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ggntmevb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qkewaczo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nubrgxak.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqflvdf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2amdjmwbv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mkxrxndr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hhfwkqzr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kllrrjwz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2udysubsi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eevopxxo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fasvjkqp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fbtddpid.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ltsoezzb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zphdoqum.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcployzb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sgmrpypu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yofrpyqc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2huwojkjf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2peyexsrl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bpfshyqu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wkfgzqgd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tjbkofbp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2esaefcui.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2johutnyk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hkmzwynk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gmcrbozg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wdbnwbar.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ecrddybz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2uzwmhycq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vmwvlgbj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rucrkoan.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jmilbmlw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dfxzdkty.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sebrntng.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vblsteyi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zmotkinb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zjccixxh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2agzynfqb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jreproge.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pbuphwvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fkvuqcxx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lrjouxyo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fknfhcto.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2usglrjrn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qlcigghw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ewertoiv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ficdcfeh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vfsodsoi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnilfofc.html


<!-- 参考信息 -->