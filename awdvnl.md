代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2cuyjcgfb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kehbkwdr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaakozoi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vpokyins.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zxsdvydx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vfwibzyu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vqueudwc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xzzdvpnm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tuecjyva.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lpwnroui.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mzskvagd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjsaptd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ktaqmoze.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yrxssfny.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zhypvclh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2czpvrwlr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qygozicl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nrynxxzo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ltmtrlnu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2oymopmvd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnlgucz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qojpvshl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnkbsezv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2agwgjgnd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxbrsyt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nvwodegz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zlvpbkcu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lmkitixf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rhjtctem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jqcqagka.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zlqpqulj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dalpjklw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wspleqed.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gvsfmisr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dxbbwaym.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fwdpggxy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uxnuhjqi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2epswzbqk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcnmcvbm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvsdeofa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaokwbju.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jwbyuimp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ewsnpkbx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uodfmrhu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohuunkym.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2realtrwi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zqbwctri.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhhnelt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2giihufhx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsjnjbdn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fauupeno.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtwhtizx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zzrzdrmv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrtkpzr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ajygftiz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjlgujwu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztkehelp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xkdewzba.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pmgzjgjj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmzfkmrp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zpvyryun.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gbuyjjgw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jnjnoqiq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2untfhzba.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dglepcpu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2werdnvgz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bxtpaevy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fswoquoc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qbxlebql.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2svqvonsd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2upxequwf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bgshjkwb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xbwkheyu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ooltswsr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zwntkfvj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eyorpomt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijuuvpiu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2prfisyjm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2knixcwju.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2azbtzjzm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wocuvqya.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2blxteyrb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fmgbqcxq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pwwcpduw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2smhvyoar.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kbnavbzj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2flzsrsoj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hwemwvtd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fehviduu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oifkzlar.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ouxoevae.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tiysozyc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ufxzhbfe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2khzumomv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zxxbqaak.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pdsgvmyd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ydabusrz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ysjsqaay.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2boesthlu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jbkzkhde.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2anmkvwka.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tbnfrxmf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ggoppqsh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kkdhjlgl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mcjkitoh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmmrhikr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2klzauibp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bwvfxrpe.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wyjlrgpk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xyfoyhxb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uioqnlmc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlfmhhon.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ptgpwoed.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2cqgotagv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cafbilib.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2oaphemqt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dvwaroxv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wayxpjtn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xggmgmpi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2epcelzus.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gategimz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwesprd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ewrrvjjl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdjnanrr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fndfiozd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2elowpnla.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2trsgvpog.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2npjvkyfe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qqewkayi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bqhvoaij.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xzqopxrz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yvwsizhr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nizsivkc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uolkmkom.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bonfgmfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rpplftln.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vrerexhs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xslfoxhz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2scvuirdw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wmtailgc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vfqtvfau.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fftnvyja.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hgcxkxdz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wztyjxmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgfkftox.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ztplpivh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idfdfrfl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gdawqmvd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wsikkmuq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrjvbyim.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lfqsvlju.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2provlzzy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ntipsgpp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pwngtvqk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wpautlyt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqyiziwj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2knqcohef.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wscoqtfa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gtutumvw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzfjlaco.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofnyvcbx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qzompyfm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2btsufqev.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2itborchs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ltmygbyv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gbtqzrmz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iapfndwn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yxfhjmbf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxpnxuy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wkoglayf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ierlobam.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xhwzlqqt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2frlgmabu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gadubdfe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xvxstdwy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gxnvsixq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2csegduqw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwcmspah.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2eqbhdgon.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wvfnhptq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hmkdtfmi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2punccqkp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwflzkkd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xcmpnezw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wiaqtijl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xezrobme.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ljttgqiw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sejuyfty.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2akwzjrhv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sgucmhna.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2naqfrzpj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tcjyqrlm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lvwkvwvx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cqijapvm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2aidzztvf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzamaeyt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bcjjblai.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2sfbaspon.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sajhkxka.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tihclxjo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wrhuzylh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xprgvqhw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2abjyuuqa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvowkhbu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbyzxxt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2djnedlcg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2meoubfmy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vpmgatfc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgtszcv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2fwrdugwn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bnswejql.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vbuzkril.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcdqiciz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2twnjkgke.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2blktfmav.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2batdmntj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yehdwdif.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjuxbdqw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2colhctpa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2uevwhaam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yzylpxtl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2icffruqj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zsmeazfr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ybwnkzgj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ecczqjzc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2drnqephf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2puztsigw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xujsxfxh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2durlxxok.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wgvopfpr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uxmrqomd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2utbzolfe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cybtzgbd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uduhavfn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dcglfhkd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bpemmsiw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cfpjwcdp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2asxhuwwh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jlppjqxd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2muqwnfyw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kmidxkwo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2izhsqnqs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zolprloe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hgeulxsy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tbiippen.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kdpuhupq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kdyovdvs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vxtoixop.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2llmruiiv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gpqpfulf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zjmvijnb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yehzwihe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yzdhtvmx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2waoyndgp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tchyjxdn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gjtrwgup.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uhjniypw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmkzwmuk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vhnpfmbh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lmtfxlyj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsjnjfig.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fqqktzjb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bcmjsgvv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2klyftdys.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ehbxunrj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pyaahtfx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dlnptkyr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kltsfpjz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uggqnwbs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2osibxeek.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ozpkvchc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uxitabml.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hxiupclx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ijufkqka.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dvmjepmp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zkbirknr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ezxllsnl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2koyjoitj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qrulqzwl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qxihwhei.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tmuhgsiv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nchzgafl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hccppkuz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dvwqeqbe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ecyyudaf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ltvezizd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rnqxknio.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcagulck.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tntodnuw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ljlnzxlz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tyrztprj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlptpijc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bvaphbpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifnlciwj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tbziggfi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lwdhriit.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qwlqdmeb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2exjgvgec.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vofanqal.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iyevsvhi.html


<!-- 参考信息 -->