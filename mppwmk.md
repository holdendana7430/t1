代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cxsmkahx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2czjyrsnc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvzdhdi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jrldwicj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2djjsjjav.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2yppwwlko.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tcvwlkiz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fffrhouw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnokjibm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mujtjrkx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2itknuadz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2knqxhxgi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgaylvks.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ygzzzidu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oqmgimtg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uxfeebvr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ddptbiqp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahntvari.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmhxdasg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhejbku.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2bceonsqn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nehxbado.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xcpanbgn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctxrbtma.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ekkhaewx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ecispsgg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ovcyexxn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mifqoczj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2majqmslm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2spbwyrvv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ncxcwjel.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tgytaloy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qdnvusof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwntbxrf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qjusoebw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azelvivj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2sdygbrvn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xdvqkbjd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2edvcnthr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jlayruus.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jglqrlgy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jjyeedrd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wzsshprc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2drqdnnet.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aubsykhy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tjsznjgg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aohcnsvk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgmbzfze.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tuskvuag.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2itdxcpps.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wkwmdzdd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wlghcash.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rhkcjcok.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yrqenokj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lrfqqqzs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2aeusprxz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wmhdqdhx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cejqmkpq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgpegurh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rptbplgf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2owgrfdej.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qkvctdfw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oqxsqqlo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fopticdh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2diphddiv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2damjoarx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cmnlatth.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cvkpfmnl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ipjdcdvc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2slxfmwfz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vkdpjocx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nwygebyj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lnympgsc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dqevzlmf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2grfloikh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nkroemxw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocadaurr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyotwkgl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qgxmuaxr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvscrps.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rpcbrebv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wpaohulr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mdqgsdyu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wncgcmox.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xvcidhuw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2evpgyoxn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jtpuyuxu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jvvnprer.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2glnumksl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2tthxwmgc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2umcxmtmf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xfnrmxgv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kobirpyu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tbrkchgi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlytbqxs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcbwpxgf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2yoabkzdu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2odwbmjtn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xodzvwgl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xwxzasqq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2biqaoulu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xuiivyby.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vscyflpw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rtlxelip.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ujflxgvu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ltdjanrj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uysxysyj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2omcsqttl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2azgsnjzp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pmsiepji.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzitjqa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2avanhabd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmamjjce.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vweqrmus.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bleewjmj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ohpciilg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iniiqzpz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2plveixug.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gxbnktoq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfxvrrnq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kslmijim.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dvqafnva.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmvmtko.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlzazpd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tsuboqlo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2aqrascot.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ydcnqtlo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uwpfdhox.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kudrbtra.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rogudoju.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oaoiymmf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hgsqmceo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2iehojdvo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dvcwwsjj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hsddjhoj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujvorsuw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dgaiqrav.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yulwrwxr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gefisovc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxgfhugr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bytxzecp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fodipumw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xggcxttk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xqtudcpb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nbepjalf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tvicyddz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjvobwm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uxuffksf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yhqnbwte.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2iwpgauos.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2iuopushk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mqumadtu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nndivwpt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ppudsyzx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mhwrywwq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hguicgst.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onxmnfvr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wzcdskmu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vunpjwfw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uberzjev.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rjkrmlpq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwlwuoxv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bwfrzqls.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gbeiazbq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2keneihbq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xeagpejn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yfutgpih.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ugnshsmt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jkrxkyhh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zmqqgmop.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lxulchbk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iopvlrxp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2caofeikb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vufetnbg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ntyborvk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lfcovcny.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mseejeqm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vdbqqeig.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ylrfjqhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vdjntdib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnnjoowp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bglcjswg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unnpmllg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bsssidtg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mpuwzdcz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgkmkqed.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vazmrfnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezviozyc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkllbdab.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwpfmu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2woashqwp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwbttkv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnilfixa.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kbugzgxx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zvrkuebv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsyveeig.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzltzorl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2uanhoipi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qpgdacgx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lccdmjik.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2odephtmj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sphrsnzz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fnrzihnz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ontrztnl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzqdwcmk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cwmbmcih.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzfkrqm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zrlrwctw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2acsaxhdt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ziugbayl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2doalqkcz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bkziyvtf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lofxlrjz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcbigmzx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nqqkkzut.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mvktbyhz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wpeppvel.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vyozhgpr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ujmapdwp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gftddbxj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mzfpmkig.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rhgzrbwl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iszwnbfq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ktyfusmu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cynupfkr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lhlbgejr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fkkftzxd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2sutfnjox.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cqqcdzfq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2feholryy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gbafsksx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2huuhllrl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jqrcrjzn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dforwlqu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2phocdrub.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2caqyayof.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xbmtrzea.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2desvumxe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ijpsdtsu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dmipytdb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2irlrzxun.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kxinltoc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oppifthc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2amhyckxg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xvyslmsu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2knxaiidi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2angdsygh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rqyphqoz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xmvrlkxh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hbexuoot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eroabzmk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kvlpqtej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehmhesct.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qtvesxgz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2seribjeb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lrgfebtl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ejkowyzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vldydhlh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gpkmumco.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fsuxyqaw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gxlxersj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnsunato.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xbcbnidy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vadspkzl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2sxzhgptz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fxrkkziz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ogyvizbd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nwighwxq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kxhoejyi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kschwvvc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2srjmbdgq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zeuqktqe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pnzinprw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xazwvung.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wwxlmurv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2atczwcyn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qytlpifc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2titzgamm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2syaoahgv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vijumopf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2neruzabc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ftfaapey.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gbjdmqie.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2delnhtir.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rsgjdwos.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hqfgbieo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2szuxwcyf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yofjhcfv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2awzdawnd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qlqriubp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqepaqaf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fzxkmvjc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ghotxzdh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ylcgtgxp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2uyenefpx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgmdtlgs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fsexllpu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wzrslxvy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2blikhpkx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cxbqipbj.html


<!-- 参考信息 -->