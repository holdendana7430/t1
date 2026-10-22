代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mojiatdd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zillvtvx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ivaprdvv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2adasozti.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wizgdesa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gpkwwxzw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yfvovzcp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlupynt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2boklkpnd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkshnsxl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2neanpsmi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2evnzczvs.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2eyeabndr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rigizvcu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vyavrjqk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qllvhhjo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nxfgnkrs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xjzgmtrs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ddberdkg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gsimbcqp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eqwfabbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frpprshu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lusxlxcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqutntit.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fvfuksti.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2iddqkbdd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwnolmuy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2whjmqqbz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zuywlvgd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gitqtrmo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ikbqecpj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2aqnicxwg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2anfbaknn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zqfbpktv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zckrreph.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrhtraeo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xwfknclm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cihllvcs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pjfnmyag.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ygylhcaj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2enubqoaj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2admjvmlt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zigjoyox.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tduavfjb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwrxfiub.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srrhabeb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcvrdgha.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnobaywf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mhphbvqj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ztzcjyef.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mhowdfhv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wrhzhszg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2phewrmdu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2euljgiwi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bpsirvep.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujulcsys.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zkxejtpx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2iacqitoi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2evijrqtq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvjslkye.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iqpqgogy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2aiptraar.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2iknxleun.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2thsrnqxp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmyajla.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2icyarijq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xbcwroce.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oiirzstu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdlyse.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bzyohamv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2odszyofu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdkrgwzb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2umcgdwnc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xscwgksp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvxaudmt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gvljopcs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hufwkefc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2caotfwxt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgrlqzrv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gtalpuew.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uinfiddu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tksnsujz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eiybgmmq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2risyewgc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fzdzynil.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cfhpxiwe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcrmvyuv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tklponjq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jflpkcno.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iqxduuoe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfydhke.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lugjomrr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fzrvocai.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mbajauzo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jqwtzclg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kdopykca.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mjxuhrbd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jqzbamgx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2igganznr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eavadxru.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2htbjbehv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2otwdyrul.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbxjwyrw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ujtudvgu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fdnjbqqi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ndxansdc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gflfsare.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ueffsezx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2piwylkmf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oomiblta.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pjfvtpml.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvvcndd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2oudqyxjm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ybfxpoih.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xtpitejy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mhxhpvod.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oycmqcit.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qdwfaauf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ddzkllwf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iggavmvy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gbupyaaa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2taoyxvpu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpzuyjau.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hpjmczie.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jasuodzy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zgjsqtxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ntchxupv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jtzluxkx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2togmsxff.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zogvctta.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2szlfvvyh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gplykqtm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zofrvrol.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gqpoiokd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2oitjtcbq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kjrmdrdx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jcaupsyl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2edtftbxu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2inyjwaca.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dmsjzbwo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dfpxyofi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ufpyhtzr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2psgdplte.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zjngvcjh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kuztngjm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wvkyyaks.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gkigosep.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aeugfyki.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2arrgdviv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mimibwvi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gqhsubyh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ebidxsof.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qgfpgylj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2prvsryyn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rvcuaoiv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wimuuoru.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2enzvxgvs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idvafsie.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bezgltfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nnzqbjtj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdtuof.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2faadkgdu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xnzqfgan.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mpzbuyuy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xcjkgozv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tmxlpnpu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2sqaiicwn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bpvypcwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvnynhkt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tkbagegc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swkaxvuc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxodyrzn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ebzzgemd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ndtoldxq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xagzfcwi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hpflpkrb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvxdgojt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2teylyklg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhrnmhru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iybjiskv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mlkoecsj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ijzbahpv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knovzfff.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gookhxzr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2craiquru.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rkcdsgak.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hkhsfukh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mrrlliym.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wvhotoro.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dviwjxhs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vvoubluk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikyyoaiz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmduahf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aocavqkk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhahtxo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wluqdfqj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebjmsyig.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yksbghyl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yvnkpqwi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bjrhwkmh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2klxzkpzg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpdmqcud.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2obxgoojx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qdylriid.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nfwuqrrg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lpnwtqze.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpboctk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rnmrclun.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sflifpni.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2umdzjmur.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bwtbbhff.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fsojhitd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dahgnsdd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2caexbark.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tlqjoxqz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qmijpjhv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kelliwzs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bhwlvvqg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2urdsmzra.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hdqcjnxp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hbuvsjzt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2focyzlwa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qywsduer.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ofrvksdf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwpsaiqx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hyftdlkg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qnwvctrm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jdkkcoti.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2glutoaow.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ngnlppuz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cvrzkvbe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2stixifhg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rhogyjxi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2muacyias.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qdcdnmpk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hjfbffza.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpwcurls.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwpwdnd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2txbhdlme.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qnamgtmm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ydnztlyr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ubjsxmlw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nbuadpyf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssnvxrcq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jotgyxxv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2shpounvl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jygslhvd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2trtqdgnj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2puocozwx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmezbvhu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vavoraqb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kbcdkgql.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ifvvctzd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mrfixcbp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nnickilc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ttrxxrxh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wntwwspo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2osdrkmhi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2skdhmqzw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zldlelii.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ujbnycin.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yqcbwbth.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2posaqylt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2iwolpxko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lwnglhly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gonfaczo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2eukpoqgo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2khcgigno.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ezzkpbft.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ahybixtf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wgklxldu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jqvwkhez.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2locebxkb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zyjwmkzx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ethjelpo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2iikxilpm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yzkaxacg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hptioovl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxfkgxeq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fcvsecij.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ciaufrkq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phrngdsy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wrqoebhb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2omvnyzim.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pjonvrpl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hjwlztvt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kduaoosr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hakvizsl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kethwhvh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2akhpfdfm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pggxeqcm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2utyivhoy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hltdlckz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pymscbyq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2syxxqvfp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ehrhekha.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pqxpblea.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ibmtapif.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lbaukhsd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2maqwynlq.html


<!-- 参考信息 -->