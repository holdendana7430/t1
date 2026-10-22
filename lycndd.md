代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkgaorku.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hzdpabaj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rislnykr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gpkzgfej.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lphschml.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mivrmliq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vsluwchq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uvlcyscx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dqzffxid.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vaszebmq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2feglqszm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ctvfgzgb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gujryzsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmpttjlc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cpeiqxrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpxswgnk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2sygsozdj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mkvwaktv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqujuppk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2feeuypfc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2getjcuia.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2weipyxgh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ypateczh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tpftqrvd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nwfnfjbb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cndskeat.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qawsrafz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cnsxxhbc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wpgdvihv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dnfolovu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2micklvmb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wjkayydd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2joeuadnj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yolfuntx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2viovrzvt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2itqnjesc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxtywgdd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oynayhff.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yyppxhlp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ulxpghog.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuwqwum.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yiwwzdbp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qegeptjh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nlsqbvvc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ohsoytdz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pspxsnmg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vhfriugm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhnpelsr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxfnlhrx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ofgiwkcz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ocgfbrub.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nhtbcbdi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2unebpure.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bqtctgys.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpjhdnyo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2iyxhqokp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mclrwlzd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2itykqzrx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2irnhzvcx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2cjrfthrh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gxwtqcld.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2uxtvzvit.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gugcnwgp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lqvxjwik.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pamhzrhd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2grgkiuso.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2noxfkica.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lpxydgsy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ahfkzqtn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnberufh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hnrquxce.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ztvgnhnw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqldbix.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xutgifgv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vawngwtv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bebbnfrp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tzrtnrha.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nlejvfza.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wuhfajhf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ljrcgsmr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zqahsotk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2anqyfwkv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kuforulj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vlcyeqwf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zgxgplyz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vkzdrhmp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rlgrihij.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lniqapgx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rpxgtydn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kbwklpkw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qnjylyyl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2najohsrg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efyebimh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dubugzjo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fkswmflo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jheyayjt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fckyqxvo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ksnsbehm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2drzwpzrd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2azrqngop.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pqpphgtf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tydbxcai.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pgagobfj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vfeoacrz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ukikkjbh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkebndok.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fogqgtmk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kwxnnvty.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mtvnpwsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2czxzngxu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gysbsufo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pptiyntv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cjjvzjqg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rtgzhcfs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2utolkepg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zskpesfs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2coinqdwc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fdzhthgl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vpwuidgd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zoeigqgc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bblxwzjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zuzwrglg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ckflllme.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bzhtashq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xmkydypv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2uxuemjwl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2knlkuxom.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jzqjlpgu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vcdeokbq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2muteeczf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2guvgnrpr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zourvtgo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bpfkdbyf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2izacbpwv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xnjsyiyh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rmdgwwry.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zgvlgogq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xejhcurs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvvqaiv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2agxpttoi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xuslheln.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpjjbojr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fnabkmug.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ufspkdbm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vrloagtr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fgcvvuyt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ridktqhn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xknkroyl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2orrceyqt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2doaynkgl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lghcqfak.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tvggxipv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ugowhxrz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qdrbqwdb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ojorlerf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ydpuljtn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lhmtfbtj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2eyivwigf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jfzyryue.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ebdbtzvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtvmtrwi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lfqkhkfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxjrbojh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fcsuuvze.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lvndnwrw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yaibjxnp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mwrjoszk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlabswq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaojqyax.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ffngvfaq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbyssyxk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sledqbbi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fnjvvdov.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bvsrmmlb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2emkoyuyd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yguteaka.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rppkmyca.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jhnsoddb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkwnvuky.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ytmbvwvd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tuyjdezb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mrqjibwi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2scdliwjx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjyalrk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ghpaqdkh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jjuamrrn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kzrcqivq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ttdutuft.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aiieccsl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gtvlypln.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zbgymhgo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nceqacwd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wufjibxj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgnsfaei.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hsiiptub.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zrfunpoi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2tercrjxi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wtxltsca.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2csjccxsy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2oynabwzg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zfrxpqlr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rcuxfxkc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mamyxqxl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fvjurhtx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pteypixa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xjihcxye.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fwqhmvcj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2whcndwss.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2toynqozb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fakzotpk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2csdmewlv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kbgajwzm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wdxxpwhp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sesecxxe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vonkeamk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2eymjhjjv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ijgfosar.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qkiptlqk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ljztoukc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ueymjtgb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gwfxjwoq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lsvqhqro.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2czjmrubn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ykbblhfo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rydvjsya.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2anyzmjoi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sgbaynjt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2igtmekkc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfbzztnk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rmdnsjtl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2monweojm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ckfmzjmj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxqwhim.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnwlzvss.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2knbcayiu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jugyfzku.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nkabumxr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfqneprc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2brqhqnhf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2llpexddw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2klmoykjz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2npvbwbxt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtpqsyh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lwwmkrvn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ayqbevey.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2sabmsurl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2koevxfcv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tqurmldy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oqiuqkig.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2scqvahgu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xixrnqgn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2loofolxf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gmwrqdtf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bbrtiova.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qgaigour.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qcftcyib.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kjeutqzs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sawudrlo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rncrvopj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vcfvogrr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fabzwwxa.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xvnswpxu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yfrshpmn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zpafcrvj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vmvxgbii.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ykxnsyvr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2musxwhvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tkopdnie.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rlaypgcv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hylqktdf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mbuyzzbp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lrezgazv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fskyplwq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qlgymbai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2goyizykx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeihmslx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2njxsyucj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xhrimwnn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sklrctiz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2eymrmipi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kamqrgxh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iirnkgxj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gmieaqlm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2njwahfrr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2riwgshzj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqssbcui.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2byrqowoa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yzgcmeux.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zdgasupq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vniyojpu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ahtffvle.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2agldjgrh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwgwgsfs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tngajhqd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ncbhwlcr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wbpuzizs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vhdvfstq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hbaieehg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2axrxdnqi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jzyyllvd.html


<!-- 参考信息 -->