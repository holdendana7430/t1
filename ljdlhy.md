代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pbngsnzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmfxvpkt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mtdinriz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2appvwrse.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2eprszaom.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2davlmggy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cjpjpvwp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zycbylvg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rjslgfgr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hdramyby.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2knlthfdm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2manlzwui.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mhopzlon.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vlrrpyjl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xytcvvas.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txgyesir.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ggzwqmkt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nkapcapj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qtxuqylh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmeuctj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kmdnrmdf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ifkfdfto.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2pulnuudt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xyjqtnso.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxkidqgn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wiwshjte.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fvasebaj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mrjzuqgg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2clhclqnv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2orbuiyye.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cxhsrxvb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgwuzugg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rkwsxquk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2larhclha.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lmlfbwaf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rfmbmlnw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzzvjohp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2erfgfzji.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nrfcqety.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymjhyenj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yhzxlbld.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkggave.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dxzrizqi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zknsmznn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kthxtefd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ccowmphq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rnyqvyws.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nkfwhyff.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjsgzpf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wzsgxmtu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jscqalbm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mksfhntp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mfbdrhsh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kljgdsbh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wjcprtpd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lzbddlez.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qxgqqrwm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2uwvaeyze.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xpmlhzck.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ocbdiexm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ghksbkhx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dgdorqbw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2stdfpxyp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlvsvmr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lwyxmxxh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vskzzfym.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jxgcsftl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2supaouzg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nstannmn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yfwfqcxu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bviggdrp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ufjxkvcu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jfmzekci.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vhzxjjtb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lfyfufki.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2stitrosd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2itkglrjl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2genvoqxx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufyqxnxy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tcrylrpb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2upbcozmm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nbcxekut.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vpmzikzz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2aebfkhtj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtepskbp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wlfcxfun.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zruqunxj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxgpfoz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fzesdnuy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aztkvdmt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tgibjern.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ntiqvham.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2amzabpwi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zggijxhp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jueazdhc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ihpqavsu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jqlkifar.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vansrnht.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2eyomblre.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnjzyysx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fscopotb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xgwowlzj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iapyidcm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xtqfcpai.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ltjccrdg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2aehooqav.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zdtnzovz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kpxrcwgu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dbdgydbr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cinvrerl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qibljyvv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nmztjhvy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fqlwlovo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jbirraao.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pnqibyiz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jaknottj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2whskrxvt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pxxvvzrr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tikxoglw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aureucea.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rkuzoczc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gzlvsmog.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fxsutcyv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lknnofvu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvmxigkc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmfinqo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyfkuvey.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2acxnhyqw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twdjrypw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gphuetad.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2eeefmxft.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gkgidema.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wutoxemr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xguynnnp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ikqoxldj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pymjaotg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oojlhlju.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2duqzwwxb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zuqxvlqq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sguaowzg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jvlugoco.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2smlzsrwa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tfpcsruh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dvhpbbmp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gukqunzd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wpwkzcta.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jemugmom.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ruxpfbkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpzodiux.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ihvbugyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elbzelhp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyzeiuxu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fzhmepnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jsgwrgdf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jbhxfcty.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqaakprv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbshavjg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2hnlucdmg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnyppqmh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yivdhgxo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pzqdgoca.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yunskaoe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zftkezwv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlqtnwnw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qowzjrgu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dyunxizx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptrjqngm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wfwmaqgz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nevviixz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rpemxfsy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tqpmcige.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rzsujcnj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooencatk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdrkoejk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2olcxdzhc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtibssp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qteegkke.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ynyocenv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ujzhcvte.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2edvysfta.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mulckkbq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rngjjoiv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ysavpzoc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ckdvfjjx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dmglwcpc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vonzbylm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2otkqvxua.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mjhshmor.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gkvvaakb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kizdrjck.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hzvioltq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gedlvtdu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mvhqwwol.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2icwxssgg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lgvobzxq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vucvddct.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ehgkmlfx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kwmnvzkn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2oryybxbv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzmhimug.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xtlotill.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bkvpnisy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nzhnunsn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2graenssh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kcvwozkr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kgwrnclu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ufkhvgzd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqszubff.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cfmpigew.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bpkaggbs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jnymotae.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2begltzmp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ehqzilvv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gbovoxvb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2thgocvbd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2shmdbkrk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qapfreme.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2swxkswzk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfojnav.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2discyeay.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufgtxvut.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lzakinoy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdbcduia.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dohijril.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vlsdczok.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kpfrgjjc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vdtbnrix.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qbbnwxwt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rmgzoyns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2apwtrulx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xpgknamc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dlnpkqaq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2csmjvduj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jddcfhpd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dotzynmd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uzjvhfiy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kaideoav.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rifwmjwe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ftgccgoe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2oimwxnms.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wjwxmbmk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kbcsnill.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2noydqxoo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wyrafcle.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hcsmbgvn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2webcezxt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yudxwkud.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lzluyhzr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hwaqynpx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vrvhpath.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2muayucgk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gloyvvyx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wjdfgnro.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yjlltvdc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yqiwwbhk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2flsrqums.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2iarmtnsk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xxvvtbof.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bfxguaib.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2emnbnhlw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ibdopipt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xxetaqtn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2darpbmet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uprlagra.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azvrezae.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2aljwjwoy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mdfjyxtg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bjylsiqp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wyrqcnhg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2apdmsmul.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dqehxevb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gjkussfg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uhtgvqjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iuyzqdnw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iedsztir.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2whmehgax.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eaxdqmjj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2uizbyhix.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ibsanxwt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tdmhlzqc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsztwkre.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrxobrbg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vzxvqdth.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vmqgjdvn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qkzeeicc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bgcihdxk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2icjavfiv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2karzfhiy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ndlyhgrj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jcpombbi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wuowzcam.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wymkdlbo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2noufmjkf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2aokhdymr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwwjwadt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbtubeiv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pykqsjbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yygbxqgi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2csdqonce.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wdzxkrjo.html


<!-- 参考信息 -->