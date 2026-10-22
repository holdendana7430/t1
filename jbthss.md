代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ptoctgii.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ipacdumd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2anywlefr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgmrsns.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fwwuysrs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2foprqvyd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jnjpcaqv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2wtakuqzy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hicfqqbz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jaikyekm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wzbbmxwj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zkmvrgtd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2poaxzbvp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bgplyvmq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2evmfbfvy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xjjmzhjf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2kbffkhmn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dpwwupaw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2twdxfjqs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2blcgitsr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ttdpkddd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xexfhkxy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fhwnpmtd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2igcnzibn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mtlqjjtr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rwhnkevq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kjuiurqe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2owvezxgq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xnmaoybm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zcjozzom.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qmibuqvg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tkcpaoli.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xphscdax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfbytmas.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ciwszxpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffntkzua.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jqmijvzx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ommmxfzf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obpllwpm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nyuzwjei.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eaqqspxi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xkziqlmf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2oohfnmad.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ipwzkszp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ckxmbjxp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2zhpmlpjn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2avgtmpav.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhfnnazj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ypkyddwc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gbqrgauq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cyulkqtj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mprytzaw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2roeprzet.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ncehgvsi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2thprfkkv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fpnokimi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyuhdcsy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jvtwmffe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fbrhqtga.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvniruue.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oerjjgna.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fpescfgl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nyljqgkf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mihlicrs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2piyactag.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2atbsqyaf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ajzhehtt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzuycjmy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lblopcoc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qlsfbrjg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvispop.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zboungpn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ehfvzzzd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2waaeqxjf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2absisnmf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yysjmzpg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2venlevun.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzrcupkj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dlapidxl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2murfqjen.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2abesnqkd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fqtaqihv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xqitepbz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mibouqyi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pvkvlfse.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2acjtawwg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdurwtvx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rywhlqxt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kphehvrd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bwmwafdm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fcfmdsyj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uqujmyjc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhmqlcbj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kptamvoc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmtlopjw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhcqztid.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ethrijxy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvlohjuh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ipvjpdrp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2uxukbmua.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2huxtehbl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sfgedceb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2utjsnemi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vgawfcpe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oqraqfkf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dzavvszo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vbohshtx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bzekelxp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2agnnknjc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sasrkbdx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2obnjrode.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryfqrvoa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsltzwmu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kzgakjaq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2poldgcit.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ytcdhwsv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmunimbl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxfedrum.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzbyyty.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqfdvwzz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2escokxfq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2abgcjqwt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvsiyri.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fgoqdbhf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rlddzgen.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocraykyv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fnxevmmg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lpanrqjc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vszuillx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wspcmgpp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2whvqhfac.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fxyrscfl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ylgkvkat.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2oeibhyyx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2upyyeblq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jonujjso.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gxjtvqfv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xwxfntku.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2guzzzavq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dqwczicg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kduaunbr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbbmakgr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zaayhdhy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dfmpsvtw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2imhsvfci.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nmkwpbyc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cafgtdnl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uzrswzlv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2irsajbbi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2oatjenzk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lkoumckl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2psglqcuc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mzqfestz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2euvwreqo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mlbdlqjf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uyvpizfo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spfsxyev.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjgidqh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jilkceki.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ifnnoxob.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yvrkepng.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ueqcorbg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hsnxeatt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zztahchl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2trnzavcr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2svacxjuh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qtwwanra.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hlpzuuzq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qufqghqa.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2odruxyqc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mxwzgtzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mdpgdeef.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yzmfifrl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xlxxrgrl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cdezkxpk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gnfbyhhm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ljdbksqo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hnfehfgf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kpiihxhb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jsvclzdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifvvuttn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2taosyjbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iakebksx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cibbhjdq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2pynawnyy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dopdkred.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mcqhcogf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2opyaxvym.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uthtxowr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xxorlipp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdnzqncc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2saydmozm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2askwsaaa.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mbnbikjd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yegqrurq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogeehepn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ipomzphc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wvnlknol.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2juesvdvy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vqnbycrz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lfcutpwt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qzgcowdj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lciqzeow.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gbsmvfqn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtfftcxz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ktptobsr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbdrdhve.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcncusd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2khikwofu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2eyhrmuka.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2nldljsdy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qugegcrm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2plactfoe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2idlaemft.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mooqciai.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2nciwvtyb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2yauugoit.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gliyplxm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjaxddw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2enfsyfhs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2apgvxxjk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2eqaqmsuv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pjpciiuk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bzrqlnln.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jcygbmph.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hrjcxlbw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nrnbakkm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2enkwluif.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2aksjpnya.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sbpsphds.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xmajrcqc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ikhryspl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2neaaptzg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2acsaozqo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gruasnef.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eyiohrkv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2szdsfiri.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vbbxcjko.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ipptvspl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2upciwvbv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2shivwegl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fxuasopa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oalfwjnu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cgpqrhkz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pynqldgz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2murwtmje.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2guhclbgy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qtwnlkbr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnrjmweq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pxpzwpxe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dyhwrtng.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jpglvmhi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcxissu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rycjfcvh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zxboidwe.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbnrlstw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kqbwszpq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlteezu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ugmjsgyp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2obatkscf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uksjtedv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjvvdbrl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2subtswcf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iyssxunp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oifpgwuf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zvjvwlhc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2erjsytuf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yjlsunwf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pgxyutxc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vhaufhrj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rdberjso.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zmllevtj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mlfzywqe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bbuvnaof.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qqvidrzd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kqtwnylp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uxfnroxu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2glstwcla.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2flcvohmv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uxzbjvkd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vbzigiin.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2kvkrtviu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yolwloey.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xxlvnfls.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nzmonxat.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vsjhutzi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pbimjuux.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jihrvbld.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2exfueped.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pdkmynjz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqtuejsp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2frzdgkle.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ioqdihxn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogtellqq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rxlwtxkx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shykicen.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhphecei.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kzqvftta.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tkmtdnyn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2djqaonwy.html


<!-- 参考信息 -->