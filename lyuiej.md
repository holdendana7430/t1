代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xinkpxys.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nkwqnjaw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vhjafkoc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfyunyho.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rbdpaelo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dnlckmiu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tqgrlrwl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkfgfyr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lgfryibm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ikfvzkqt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dsvkwawx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jddthvlc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nazfqeid.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oepvbtts.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijqyddfz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2djsdlizt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lfhbauao.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2sojkubxk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fvaomdjg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uiwvwyrq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mvsbkxta.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bhhgncxl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wddlzvfo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wrmknbry.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdnerlc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gememztt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2cpnnkeuw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2stxhgpnz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sdcnqztw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fmgwcphm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ophsjwyt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vlhslfcu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xwkxmfya.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eohcnelm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dvdhnulv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ohituoii.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmhlhogs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2blpptavt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2avyfrptm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cugwqnub.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rukhmoee.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yfqjxkpy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jxgkvszb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dxvvpkdc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qlqibiqv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgldoicr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2zjwnssuj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggcrhbog.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2baijsxsp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2csqnkhcw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbtlkcfe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ehnvvjpb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rhvjwnjd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsovddkt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymqusnrg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jbyelfxz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zeyllqqu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2idnflgjx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2glpholuh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qlikzdmm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xpgbnbrz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2luntpnph.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2iufhxsxc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zgdjenrm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nanieyvr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kmxjndam.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eltvdyqf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2soimoyfj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyjyguwg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2reouqkrg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sjbstktu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dchfkfmd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2htyjrbxh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2msfvyamm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dgjmazbr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yngpmxlt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bxtonnii.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cbrovklj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyajdjpa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfxbhht.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tbjxvfce.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxgtthjk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uwieqlmx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fjmnefav.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dbgndbie.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fgnrdver.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tthqfzlt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsfkeiyr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2atwazufg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tizeigdv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sghmiygq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fxplvort.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cqoysdtd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bifrwekj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rlkygsuw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ruesfwzl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dtdoubgf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwqzezfd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pkymkovg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lycetgdo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zmgchmqb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2suahlxpv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvclcwen.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uomrhiiu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sownzazf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2trpoluqu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wlblspcl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cmjbzppi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2uaacnkzn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uhosqdcg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ipaignir.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ntunpolr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ttmkknuk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgtwnyje.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pqcplezi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnwkyyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2satynhpe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mznlzwjd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rqgmgkie.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jqeayrwy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xuwsqjqx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gxvfmvsf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2htggpunx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aaogiwwf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kktaxowu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wznnyock.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2asbolthv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rolbwsaj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2kxrurktn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2umkahshj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rdnbeygf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aqnwhzzg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2axuvpkjx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zadwclru.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gljrajqh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dmlqruvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yofzmvwr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2txqucdkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdbvdrlx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rzbosnsz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vjkdrizv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzolrluw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yseozkep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjushgwq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igdxfeun.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqcnbmk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxfwdvkq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlqxii.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uqmmcwua.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2stdhwhky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojvhqizz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzeucsdq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xfvdarfr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vnbodjoo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnvydxiw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uurbolyf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gvpvtmav.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jryfvvrw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ytzzxmrk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qvkuiwzw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jlibdxug.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hyokjwuy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtldmicm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2eqxyzxrg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2afxiqnkr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mocfepyj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lwnzlwyy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wvsjvqhu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2duqgavrm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rxedfxcu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dorlsbwr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kygoznez.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mxqwhgiv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdlgqncc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjahvfd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2aymjqpiw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mzboswra.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2usflognb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ofyzltwd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jmnqzqqz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2uobtsqzb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2agffgtxw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nhqshqbt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wtamxphv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vblzuhed.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2untqrhip.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wedyamft.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ujkufkap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iraiokzm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rqfsqneo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2alydmlok.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vzibagzn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ayurcqqk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nlgvizhv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2btpnxzib.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uvndqqpo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iaudvlfz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qsqmphon.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tkcdlmuc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tsadwtoa.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zvagsgfj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ejgwcncd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2truzpegx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2llfzelje.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlwhbev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2trechkvf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2clbrbpoz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eqbbtxju.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2aqaaevsm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uhpzqugy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zljimjon.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lzxfnaol.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsijpvxo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gjpefeej.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dwezdsgl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xhesozzv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxoxfaxp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jtmklszw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ytqdwmni.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2excvyjkx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ntotuxjk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uqfotszc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dhnbvnqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lgagfjnb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ljuvngxi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bvyfbuiu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oiyhmuwo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xlzfjedo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2peuoaozo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kbnewtiw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tqkqatpt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2imyrhice.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2usmfuwuo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vtranryv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2avavzbdj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lxunblew.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gmmeikbh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qqpkming.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oybqaabt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wcewuwje.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yavrytte.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nznhzaio.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zjqpdfyw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jvkyqouw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vqplbskk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pzqdtsjh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2prdlklot.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xdidbwtm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zvkqjcwp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tymmlrml.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2iqxdxzuc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzjseob.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2edhdxbnb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gdwwhlhl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sudqiwjh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2eitamcqc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yiorqxas.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ffbpmnus.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tvpuinxd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pbbcujay.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrhbuuiu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ntbuvpis.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2obmyfwzd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jmlgsidw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vmoxabtm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cgitlgjy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ublchpgm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nlxqbyxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2edecnzrg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2isnmypts.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hphoqwyj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vviwfrsq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bwaekpub.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bgsfmhvg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xrptuqbg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vcyjwlna.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bvqhqjir.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hhmghlbe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xrwoccmq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ednxjtpj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2koysaana.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2eowiqobh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqriqsni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xueercoe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xhqyhzyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdpwpkay.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lrcfetjz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ybuicnne.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fzrdjbrf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2afitojvu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cdwurooh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lsxwemfy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wesdbwbd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2uusgerql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ijoboico.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vdeoavui.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vytlqzsc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ldizgtys.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ejruugxy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hyqfjeke.html


<!-- 参考信息 -->