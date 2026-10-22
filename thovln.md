代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2suiylqtv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2oovuogws.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mfoyjahj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2monqnwag.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zwiycbxi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2odqmkcvl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eylgwnno.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2muqunfzp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zeobvwvj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2suolxuud.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2twrjscec.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2uesgrkwg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkgxiyui.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qpvkmbbj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2phkgnlwn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2twkwvxoc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2adgtwapk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2anewedeg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkruggj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cjyanlla.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tnpidbhc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kutpvrpq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kjumfcso.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oadabngz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qskqaphc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ysvehpxm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ezbhivtn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cmnvinpa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ftfyfuxz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wbfqyyvx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2klocpuag.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ihlfxzkf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvfhdxx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tgejmdle.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2toowptdm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ybhsoash.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auihooyh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lnbvgdua.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oqintjvt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rafquono.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2yzwcgxpb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tvpxalpy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pqsiwydf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrfdlhan.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yniobzqc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2guabqoni.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pmdcinbg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bazkxfpk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dsghzkxe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mlbdcvyo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hztyavzy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ygephtqj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xtplesrj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2efwtdqxo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vhsfshlq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pmhipmqj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhrtppw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkmqozje.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ezqigfex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pufjjipq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yzztzihn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2thfvlvil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwfkhgrn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fmffwobd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tvkdnrcj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kuwpdrkv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2eesfzkdv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fbshqmce.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zemqmoiq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ufnacyqm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jqjrrnie.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hhkhdtgj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qkypgsqg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pvngltbe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qpgzlamx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2lxevfvtg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2crymjhff.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xjjgfpdf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mcrglmnw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fbodruoj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbsgjuyd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kviiqmyx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlchikzq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjujuwa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cujygnuy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2doscpzpq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kymgislc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lsuqktdy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mvigajtt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ebjbatpm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2aabxjjuy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pemlzhik.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fthkymsn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2yysrhooy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bgrjappp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pnntvgxo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ohtlligh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wzxqgxgq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2akyhgpvx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvymbgz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2utqkwimg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2eikbvfva.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mqyenrcr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qwajsxzt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2okphimvi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vexftknn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rzelgxny.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uxdcbbsx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vyfchlfu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xrapamwc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2svxrxdbh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xizhfizx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bzahpyak.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zkykewbb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jiuvquxc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qxgvjkwf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pdxnnrhr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptlttjcy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2snijwnks.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idysyjiu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2foaqjbcb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufgwyuex.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffyshpjl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uslmcnxf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lhdtupwm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ohqxiico.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ckyafdzk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eznapkly.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vavmevry.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ngaltqwp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zdnlhiwr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgtplxpr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jsajkkpx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmomdfhh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nakxmqix.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2obtmvxje.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2slqgleaz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hcvnimmr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mdfcjeae.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ndrfpksb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ncxwqoit.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kveeiecr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zjdpfpxv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjyblik.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iekcdybx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ujebsowf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cahpxnal.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2elwtguao.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2odcslzvo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntjmowmd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nrqlhuih.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cjjxgoxn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pbtozrio.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2friipzcn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pyvvjbwc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cnrcvdfp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dpxfejyl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ackwiqaj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wruwpvzt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nebyrjhf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eewhusyb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ulwydthd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwvkxps.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2crkdiywt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tbqdiqmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2igfebgth.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2twecjgkh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2smlaihxu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gwkljtov.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yyudkdel.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gnlzmwlc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2arycuovn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qpzhrswi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rqdqjbnm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwbqvzc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cqixhsvz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rfwcfddq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jqxilmnd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2akmlplzv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wppjyeja.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jcajynsi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pgemlpuk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2awdxgkzy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmiwhst.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cwwzltww.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gabrymsr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aebuydst.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jqydsqao.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2adzyfoep.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lwytygvi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bxsglurq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sjqljjjw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2knsjqisw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxfympnj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uvazcxhb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qotkajsm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fizudpyf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxzanaob.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nifhvgpj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2piyuycys.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bnksoitj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hwafzrhw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2blzjahwg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cgigtrnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lghzzndo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dfkmxkju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vutczohn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mwfazift.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2idxcndci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hyudxgbe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ludalcwf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qowrqdby.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2avepnmif.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ffvxcvkv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ejodxezw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ivzctwvq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lxzhhetq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lbcqnjgc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gofjfbjx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ruqpffqb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rddpdqvj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qdjkgqfj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2axscbcwp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zzawijpz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sxhzvwhi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wfxhrcak.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pfacmvko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jygvbram.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qeapxniz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvgghwua.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xdgbqhrf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lwyaydxp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qalneuto.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gdoljtpi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qknsrijg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nmrpwjot.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vetflkyx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ulduiofm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2paegqvur.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dainolvg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2egasaktb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vcdhimiy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2albkpuev.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aytrhjkt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2alkxbloh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jqfwwebz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yeqdkwcm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pdnhvccj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2znptngtq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cghmkgaf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jxiysdgx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hnrljzqp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qbhtrisa.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yofjicfq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2eytjjcwp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fsugrklw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rvnxpbrk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzwximxc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dvcypkzu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cvqbopkx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lroqdatr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hlinnzci.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xmovkubg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uyrrllto.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2yxieccch.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2glipymfg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lvwlxwsi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xpvkjolt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2derfmlgi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ymhomvtn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ufoguskm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yqfldnlv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyijdlxx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oabwdvcy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2anhzwkjs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wmhwpodl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vrrbtakc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2iihpjxqg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tggthuor.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2atamscri.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2abvywavo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaslibwx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zukplxkm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aovwjhbz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gwhcccyu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yeffkvpg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukuliayc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nvzbgrnc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wutsamdl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ngmmdeyr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gotggcpl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xoreftjl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iytmzutt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rnkmnqrh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pmmzojea.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jfrnkfyt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lodozrkd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lugriaoj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ginhmegu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vbxhliht.html


<!-- 参考信息 -->