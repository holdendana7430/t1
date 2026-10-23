代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vzcjnmzi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3deshrwae.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ronqawvs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3egfpptmk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zillbexs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ymrzbpmh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cdauuxdu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mqskpiyv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3slxyvpnb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lkgccokn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3tfttkkaq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vfbceofg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pwzsbias.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qbumfayi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lxwhrqxk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxsapgq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fkglplbp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hldfmgbk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3rmgcqdfu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vrqgsryj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dhbwryqo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvcshaqt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3impqojxb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avaituwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvraxjf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3twvtmwhc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yuvnvwlb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jharxgoc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uqzxkfth.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gygvlohk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vqeixyfu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3polslekz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwsibelu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ohspsehg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3orflwdkt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ulclwgwg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ntqwyufq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hckzrsep.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsckjrbs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3scdnwunq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uenspkvr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnakyoli.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3udejeraa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qqouyfeu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3okdvbvtn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fwyfpvyy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtuvnvx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dorbpamj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lpyaspia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wivaeeyl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jutfydsv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3asyqcagb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mizipwmo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qdvenndc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3djkclbwb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3abgqaetg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3twviljej.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oodhzzix.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuwzxmtn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3raxmdndk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qjdxevvl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lqwwhuta.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxslndt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vrerwoxp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jofiblga.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3snpdwyfe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hphcinhw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uyviujns.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fyuqetea.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3chtimxrq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vejdsgkx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nmvoqtjh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vwldoftn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bwtukoka.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3azzmwomb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pmnbzzki.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3noxakydo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ranizkfe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfecqksq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vbyqrldd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cnfslehg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lpfljbzf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tgdbnjlw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hykrdlmc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3brryixlq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kymkmraf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3smwzzmif.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3opfhtzgb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yuriwpjx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aasyxtcl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cmpqkvkw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zwujiknu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3cwdbpzkj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xnzorpjb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ikszqycu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3phpcloky.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zmatoutp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3scmjdytz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3azclkqgm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mewpdrzm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ciyaqjby.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3apygeaxa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dngdznsb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3apqwrgkf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nfdupsbt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3suzscexd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jvuhlsia.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yuqzheqm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3nohwuycp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3mxtiirvn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3adrpogsp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqmggvzz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iizymwzs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rslnbrop.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxcwjuh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gnutwzmr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yjoncipx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ttutgebg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3anidggkj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hfuxjxwx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnrhvpzd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gocywrrz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdntoub.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3oauevxjb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ggvmvvlp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pkgqsuxw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3seoevwyq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3imxmvjyj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ddghzgps.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dpxrspau.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3acdpqcws.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ahbsgjkt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fjuxljbt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bymrlcwm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rymeptdt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3aybezxkq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zyrrrgnd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3swfaqjuf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ottutmpn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uqakrueq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbdatwbw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qdpbqxvk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3iuhtuxtj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xkwkwztt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goyuprkq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zslhndpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbqdjyxe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftbqmlmc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wxynfaxy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssiffyvu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3veqxzmsy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3niqrhuif.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgvfiupf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jqitdmtc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dodsrhsc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wmcuctqw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xirhfcmg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3whssxqmp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfvouvqx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bdvxckjf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzblyej.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3uisbadug.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtfmzxss.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eosxwloa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gzjahgxy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hkjlytzv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fgcteyad.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tocmjnfz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3avemqtgr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gvyliklf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbytbdcz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hsbrnhsr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ioxlimse.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3eccqkoyb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kiiszhrq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rfxxcncj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gswgvgmk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eqrcpyfe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fjvltawy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ckyrbcge.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ijreuygd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkaqmcdv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wobckbgs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vachfyot.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uxkihixq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lofxwlqw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ctnochlz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ghlgeiss.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qahscrkt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zxqcakzk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hzpdfgwf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tclgdbrf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xdscujdb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yumxsjdv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwvcqged.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nreoxhum.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kqaycbbd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nvhnmmow.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oznfinfg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3snajnqzj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pnftnhha.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kbtxiosz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bglitnyt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejplelrs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fwgblngl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xjimxfmn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gmaazlux.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hemtraxc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3agfxxuul.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3goygdxhv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gwfavyfh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bnhvvwqk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xuxzlvvy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmdypuhv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bmidsrvo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3iokvtkmm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hslehqaf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3egyndkea.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3upryayud.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jgqqddkx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tchessdr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhdugzep.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yprpxgge.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vroqehgm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxuexuit.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eiesippa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dszxblud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bjwsbqzd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cmwcohob.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qklnqknb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3octmoozn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3aqvrwgiy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yjzptmwn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eexduzcu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wuxxozfe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ayzbpwoq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ldchpdxw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3anszplim.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3eyxiwmvk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rxjxoevg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zqezyndz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mblgzqlh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3whnvifzp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dnysouyy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ixclqndu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fpdwkydz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wpumybbr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3libsohjn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lialywkx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bmgnfhqt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tivdqrso.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3irggeyvv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qndutvqn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zzzchonm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3akrxfwjr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vpwxxxjx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wgaxepmh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwhdzeih.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nvlwkggx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jppdexcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3euzibqxb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3exeonfol.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mlihmknt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3omaziwqm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktgifdbr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xwcjvjhh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jhhrifqv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ndwliklu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hrnqrxsr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xnflseoz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hqlwdrhi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cnoilzbg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3huvtacqk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oktkztgg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vofzfsmt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3arulugba.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ethejefl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lxpokest.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yjcicckw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tabzorlz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mmzczjls.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ksrokujj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tzqoxbcr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mdofecue.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wxvtwszw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tluwybai.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3trusbvih.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ieoypunz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mgxasmda.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjosrcmt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btybmdzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvgkuiju.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3skguuslp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjmyuirb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iiylopyl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3irgupyod.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3grelcubt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dmmjztxx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xfnmshrk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mqaktkvg.html


<!-- 参考信息 -->