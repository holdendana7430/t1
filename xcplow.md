代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nukeuqwx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jjzgorlf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kxwwwnby.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nsciyxre.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ggtdkpqm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zjbjajta.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mnakdjhe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2gwhhcsqg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zevjzplx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iaeknfht.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jkxdaidg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dhybadhx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfrweajy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zitimtwv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhftnksg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arzqxgyh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cthcuxvk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nfzhyfzr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lfnflgsa.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2esceexjh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2azddflei.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xshjvetw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ovaooxcl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnyvcrfx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqdpppir.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bambwezt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2docglwpo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2twxlpbwy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2htkzfwfi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2twzpopem.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lyjuvyfo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujngnkcl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2msnwpzpw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dkmvkxye.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2odeuwyij.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uapvbdxn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2elholoiw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cqgntuht.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cxhbnirq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2phnewusy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2exxtpgdw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfvfvgei.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bfrgrtsl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gxzryjdm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pitzenbv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wirrbjoq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wcbojdeh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pumtzgil.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dwmrqjeo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xtcmbqtc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggedqohv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjevcgam.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pclfjwyk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sialzcsw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiofjyoq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jfpsjvtw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2iarfcizn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ghtbzxgu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cyovnjoq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fvohadsn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cvwghjnv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vyipmvvu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kjauvehq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yhfzwmoj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2iaylgpve.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pwfpbagz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ndooronn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjbndam.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aryoiekb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejstkulz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2acrrewxp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2swrztxqu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ssaatggk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yvtcntdu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2arkchyzn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ljhtcfrf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qeqllwwm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vngtligs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2poopknsf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwlatdso.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhgcgjo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pnvjqitx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2iatkhwij.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2scpnkooi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vapnvlna.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dnxqkevx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jaslzqgr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2puvoraup.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2beubykha.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wzelgetm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aoexjxmi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zwteqcvc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2awyctakx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mbhoulnk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mgvbhtvz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2swbkkuvi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2agnliqjc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qsilnmqr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mpppdjvz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kdnyvqkr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vfenwsdq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dqzulrcc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uufccmum.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2esdjdtqv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wifozvtl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kaiicbjx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvtdaff.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2frsupdnd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gttrfnxe.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ojlxtwkg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wzqdxevi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpxpigd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aayefzir.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uscmnjza.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ykiiqatr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwtgpdn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pnawfjbv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2horjgonb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zocvvbsf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xhlvlmmi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qyosoojv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wsbolmmx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wbmheftz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fcvankym.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2suxzpabx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fcsjjmwf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fxgoowvv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ehojnzxk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2srhhipyc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpstfclm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2muhtlojs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mrusadbd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2llbifjhq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ovrwjihm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vkcdwcqc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2joucamrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmjuicya.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dikovxar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ladbvniq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjioaxtg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2asmjeymy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ctecnhnz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hyikuzyx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bifzrivh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fwcrrkdz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rwzrlklg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2cvfrissi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oxkpbsmm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cqeuwkqx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bcvbogaw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jajvvqqa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vqfjftqt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpkrqdqn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wtwuknxk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jyqupiir.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2gmzyuawv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2juskmyvj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfqlxbxj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhyrxqr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2plttjcrh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lffrhemv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wnflhtpz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lzuaprqp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fvbcyayl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vdjubrxo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2elrdryxs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ljbocvfy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2reqgckko.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dcmxhffh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zngbxzyb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kbugnssw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qradtknu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wmvfwamw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwewxiql.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkkyzim.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rxfgxtnz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oiwfdkcf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cbmvtmha.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vazyfulz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iebiuddz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2httvxgau.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vwkhnsoh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2owmdwryx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2egbfqobe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uzbkggux.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2focutqxi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qvuwxurt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lvmzlkcf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2skeptcrk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tvaijehf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sucetrwo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkwkmqg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xolytbyp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jgfmnbkp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2tkyvhuix.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gdabetjy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ujqqpwgz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxvhbti.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oythcwzw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2opftkwgx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xywgtsan.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kvvbhywt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2iadupgiv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2uxrvrnwq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cpnsqilz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qybkinfv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2etfxowzi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gegdpdmp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2chqxxhno.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2npyoiflb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gaxrnbuo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcyqvhet.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwuotkn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwcyrrth.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2moyysqxm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xwlxfjtz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xnhcwyvg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ukhsylar.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyhvmawq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fopqblgy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2shrizgti.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kqzsscgn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2stilbbur.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2faeirifc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mxohhwex.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ppryiahq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pgmqwlis.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xqrjjfnv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bpndiecx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bnexvlnr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2oqrqkbcp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tpznspke.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zvmobmiw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wxndqvym.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jirssqda.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2aduobupt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2udmrenum.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2foefwtpu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mmjexasc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2geljjzyf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tqzofduz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hskufajh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rbymprfs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2iovlnngx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pkpwfuvj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fyunzxeb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtpeyytd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qxqrgnbr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rfrrznlu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkfhdkvu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zatifccm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebdcmksb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddjgtoox.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2icyvwsld.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jtvxualw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2iftgfwfx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2muuflzdd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xwsauwtq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gowfqaar.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fpbisshm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gxayjlzw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uetopmla.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zrvxxkvf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mayvorhl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ussxyezi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2yskaoeku.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2udfgtcjl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lgombcgu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhymxozf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kfzuntyi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gryttzsx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qqxkqtpo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qfobvsur.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xdhnoxjm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xsjexlgb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zlvuqcex.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kojpbega.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qbkiaccq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2agfgbrzm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksjnhhge.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jwfnugzu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mikkzfrr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ioctyiwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwkfftnz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jphtcofp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynjrgkax.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mackfcbe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kdzmlzoa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jvwlbgjq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2puotqoxs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rvzulnak.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2unkerslh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zctewehq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rvmbksgw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sltokzox.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yqzheuzd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rgcslgrj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mpwgqiez.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hsgaudwk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drbrjkav.html


<!-- 参考信息 -->