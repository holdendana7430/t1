代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kfjeynug.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdtsvys.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdoxzlbi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ntycondd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2spvobcjx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2neelmssa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ngrpsgkl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xtktqoee.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2vqgzykxe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rsdagmgj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uerrdpbe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qthrckea.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2prqhyvdd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gisbstcv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2txssarhn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2svoiwfks.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwybefw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2roakpure.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2sbserazo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pccsdkkm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ttanbgvt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tdhlqjvu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qwzgfajv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wqytsdtk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bstxbopp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uftcicua.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwwcuuqs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2utywngtn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wdublczb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yrhoirzo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2makehdoa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcbmjmpm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gnttfqhy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2afqhbmfk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hwtfmmhj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2aresrvgl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fqpnjuat.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jkvosojj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qqihnkwh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gwzwodov.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpvywfot.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hqfcybdf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2thtfnoza.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qppbihaz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yleatmjc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2eipvbasa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yamxgjno.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lrqrbmhp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zotcyquq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ikhcaqyt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2njtthtal.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zwybnnwj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzkxthue.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsjbkavp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ybubwuyq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2avkvirwa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vdlbekqq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2juqvdcvm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gozogfyv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jpbbhfmi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nomrgsbm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfxuabjs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hoqmuudf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2chhpnlsp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2edkrcjnm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zvjjigka.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xsqitwhn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tihpjqur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2idwacgqv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfarekyy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fotryfkb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rpxguoyh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2weccunfl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fjfllquk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwcwiboh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqaynwek.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bholucpf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxkmxczx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjfpzdpe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbsboepj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qusnhedw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tyeolzsb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfvgwqv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yobmuayq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bqbmjizf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nezkltli.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gzpkaqzh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kmvrarwo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bydkfpsg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qhisqijc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hgbfkhbw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vyyavxiq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2avhgaios.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qsaplxeu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyvkqsby.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpnzwobv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmrcwuc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vqxzdlus.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kxhmuqbg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2aawpdljp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jujkwwmk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rlaqbvll.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zpftyfmb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hagozjxa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ylprfged.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kbmgplhu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2egcafsbb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwdjjsi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zhefaxlw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2epvzmkij.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jfddibfg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ryteoswu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ourthfad.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nxqsmjhz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jyeuslmx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dvbtyhpf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vvgcxqqx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cbhgyrrr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkybytg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mfpglijw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ktlpfgfz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2heovwyar.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fwbujmcx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jxfasqwb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dudsbxfz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2frwxrxkb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uedvevdp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fhcswmmt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jwhaahaa.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eyxjosqw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcvvenm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhyxelv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ebkihvot.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vlicqnvb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ahlsmybu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dwrbhphg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sslbgqtk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2etbxhvgi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wplquwgd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2behlsmmo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpsxdtqj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nrovsvvf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iocwvfwm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kerbvkoa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wshlducf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqntqrks.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sarelxwh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pthdyfgl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jfjyjsum.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvlkseqc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vlungfcv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wyomnbcp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2otbegohf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hvkbwvth.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hpduobwh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fcwlknzf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2elqirgyp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzzwone.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tpcmxodx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zaqhwpqu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ejehuphr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2otmketce.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ktdvwsvb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vxohjhlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbrqdlyi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2idsosdmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xholfnsq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wavvpxot.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yrvpvqul.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhqfehcg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2egpzajjk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdlofmu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmcfvkz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzbwvyh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixecdgoa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2odwnkyhd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2srhatxrk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pgfystbl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dpqzqvsj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhcblpyi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agyhaysm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vyzdwhhh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2casyvvoy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wgzqcvqy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2twbzshvd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2okcjqvop.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ntcrlhvx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzodeloz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zcuhfcew.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxkbklpe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mczvwmxh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fmtmvujw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jgbdfbuf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2buvfkgnb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xjgnehrl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cujxpivy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2frjogtji.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2guiiytub.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gnifesml.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2unmqhwwy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjhhrk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcgbsoq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nkmpvmyc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dsndgtnc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2urrmrnsj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ylmtpvnt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xppfxptw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vugqhyfp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qysacxrn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pdnhzriv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gljuqnas.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2umrccajj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2aknsnhvl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ucabdglj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rubwzpwh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2khwfvyhm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ranwfwzd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zqcdozqd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2emkusxde.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bcztknwm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rkmxhdlf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zrxqvkil.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yirblrzp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkvtxfks.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2warfegii.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qmcojxtk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2syddbktg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xbynanky.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2afgccjst.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bzordruk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tcgtcdfq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2avgvxvjs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdmneye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qvevnzoj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtkylawy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2buknazha.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxldbhls.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2arrujkwg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ihcujuqj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2apfnseth.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2utmxfhex.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zegybqrf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mlayljft.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hvyashwi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpgygjfz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2imsglrvx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hqbnmfzz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jxlhqpqg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjiwdowt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2avkuagoj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kwqqoyqv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yminoter.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bfyvauue.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fgopnwbk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xdeaorsf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mdgjpspg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nqiqnsop.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2avskpyrf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rlmdliax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2otwqtkuy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dvurbpwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gnukdqow.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fwzpkcgr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cwkblvog.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ocozfoqq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nqaelcef.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vbtoppek.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2aytvibvn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ogtdauho.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2birrrnpc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pgyjxxxk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2avltdfoj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vwssnpzd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2aahfrviy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2obwergik.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cfvaxnam.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cgwjyhgg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqihzzqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mwpwoesz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2onhjphai.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nagfqukp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rixxxbcs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2etbacxde.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2voaexplq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcpqogbd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tnjappth.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ozhfwrro.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ermnmlyt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yvjmgmwn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uhfxopza.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nhfgsbug.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2evsksjur.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dkxnudga.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ykwqejdi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xjxinyjz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gttumbrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iimnrqbg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqctoyup.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ngbuidao.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vjpoynoy.html


<!-- 参考信息 -->