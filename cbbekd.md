代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsakmxgj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkjsxab.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ahtxedkq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zlxtfsjf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qpiszzkj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jtsjzbkt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bhvtfzsw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2vomguzmw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xdhfilcw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ghhckrmv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mxjpwwgd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hjfdscyf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qgjpsuaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouvzivpz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2akgqozqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xirbequv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2cfejfhkv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dupfkjgg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioelkyuv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jvafebkh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qcsbtgix.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2toqvvbgo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kxryzxiy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2drikfexl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2layeykvt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xivypsrg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nrkkhxum.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfgoresb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uqochqlg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lemehgjn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fskzifdl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qbmlqxcc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pbznskbj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nxztjiqa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2oborwkxj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fncjmols.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctzdtqry.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xxwqphey.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bxpxpzit.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ylbkaigx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2psxbocri.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2klqmkhro.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lcloxdaw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pvygejrn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cpnhuxpi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qhzoyrfx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pbfovqql.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtbgtrr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vlgzcmti.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wvwttjwh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zlnsienc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbhbrwcx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bgkdhidv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ehffnilf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ynrzzoxy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwtuvdfo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2thoriyfy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdwnznpy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qykoymhf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2raeyehwr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rhbsqmsy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kkejarkz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kjemmnvb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hilitvai.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mokaktug.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2roemajlr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ljnjgmcc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fnszamjn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ypozzhzd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dghzixjm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gsmhiufg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wmlhwpea.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2btptnquv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wibotxhg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jfplytpb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpabrela.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nwzoadlk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yjtvvsns.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2egwjesvy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lwebkfbc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jjcmytvt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cyxwcfga.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqqyfshf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ldsjtrgn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eynewehy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfjzefrw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qefltkhz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ypyhawea.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2forlqdpe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ruesquuu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbztabp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2modqfnqb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldjsnqde.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lmjdremw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2izhabasz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fhtyrbiy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjgnirqa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gdbrprrc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hsazyjfh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iirqyfwv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2byydcazx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ewbcwaan.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ytobvynv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2shcegfte.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2okohzvme.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rdnlqnks.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bdfvculf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cpwgsrzg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dpjxnhvx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2igejgprp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zcogdhaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eqjescnw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2spmskstd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ytjrwdjr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xgqebqhx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cygvqptn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fxhizoit.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2krdzefsf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2avluehae.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pknwxkwa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ujbpdaar.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nogiwbzq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2voqsfnrs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mkevizof.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ilmrvedl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xhvxjuen.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vmhxgomj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wqtsoylo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rbegrxmp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yqakdqib.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2abvngdzq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxovorf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rkkvfvit.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zlznquxj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2amsrrzfl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qalgemhe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tjuqubqt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynajylgs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2adrfpypo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2phcoonzt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdybjcny.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sufrllna.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2frwmkarv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gjdicpwn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gvjlculk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2spdummsv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nbxdszzj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ygnvxtik.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2obnhcrzm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2epqgtzkw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hybjnmjm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mkpiylbh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wfoliwab.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2eomtxojm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2goqttweg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wefvdbfl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oaaziesd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qhlwywmz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2oxgzkofn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lfurwlhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyijespk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qljxflvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylmoidbz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nonlhxoe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oxquleph.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhobmpxq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpanpiqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2viyioutf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bbupicqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2sgsbeese.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnkunnic.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zftkccbe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2btgemkje.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ihpsregl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ferpagjb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qrezhjxr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgiconqi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lxmlwdgo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kntqugen.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2slqwivtf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ordweqoc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtypjxqr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2obzuuydz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyclhjsk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2momllmyz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zajiehos.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aydhyhdu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kfioyfoh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2upsalaaz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jethcwda.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2iountiwi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hnptxouz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rwoxddvf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uzgkxngh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qqfjmihw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wuafstxi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nraxwiig.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ooeipqqg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xftkjsyv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dzxkwgkn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zrpucqoh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fswubkgb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xdfjzwxs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aklthebs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nkopzgjq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2aogjvqco.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kguvwedd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cefjsxnu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mcwgaila.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jrjprvjf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sqnnnwrq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gumpcczt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ozicozhd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2twfkdcxo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wbuemlkg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xxyqynkj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2huwzqocz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tueaufuv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ojnchcug.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2neyxgaew.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wtuwxrjz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2oxiyonoe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zavvtcyl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mzxjbpbx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ygumseoo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pqcjyjhq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zhoyimjo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qmcoxjyg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2drgqseod.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gjanlnlp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tcyrqzkc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ftagktex.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lyjrgnro.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sdxquyog.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ispobkal.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eewaviyr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlcaomb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pxnccwvp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pbgsgaep.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jhhhmdrj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jchmtmqi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2akyhfdyo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtonqkv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2eenuqlef.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dgpwzdoq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2biobbgux.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gacnbcjb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vwtzigbp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2isitxpxd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rbzyydbl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2euptiete.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2feubnotq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pqocggdm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2htwzdfvr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pcceueni.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ywntqncr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dtxhdngl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lpvknpcy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qpuwocii.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vlqwcbcv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yylzcsxt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hejtuzjy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xzykwual.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fpslknds.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kbxasldo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2samfxbsw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sobetlok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gkirrdoc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nljnaftf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2umepfvsk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xpbkjova.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2axboyftu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kpyfdyfi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxxucija.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jbtdplcc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bghwwvjm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2euxsutwo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2olchpivj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ugvdqhrm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hnfstdyg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrxhzeyy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oumgijyj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hpplnbiy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nkildzdd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhfihex.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwomuewh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yvpxqaxa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pehyyhok.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cbzndyan.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bfnunuey.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bsrvwgcn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oykbxqta.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chnulbsq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwcvysbp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tdoddjvl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2apdnrrro.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zqhfzpmo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bsspqscz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqxrhh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2edvijidk.html


<!-- 参考信息 -->