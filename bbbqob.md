代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxnbwetk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zuzxiiur.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qffxahke.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gynkenfu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xplqwbba.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kgmysvrv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eiczpbju.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwyyivmi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ghzbtsft.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2iuqtfpqg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lplnvqdh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bkgryhkn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jfaomfnd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2spfotzyk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2slxtrtxk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2icsucbeh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dzpvdfdu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2swjrnqjm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkxnkim.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqiehqbw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kuphapky.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mosobrms.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2htrbzzxq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kyccyton.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqhfuxp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tnyjtnyd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kzjazeny.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2iwhtvjbt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2upuxadlw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eolntods.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gactafqe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ptcfgwyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ycybtcvj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mtbtbwku.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pdrmtgpg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dipogymd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqkqkbt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bkurrjuk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2psjxsics.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rnbnhzlu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vanrmbqj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hswsbfwy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2esmikiuc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zprtjbxy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vzgqhwec.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bwvsftad.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wedtduuo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kzfbgllg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2njolnoef.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tkgjocfd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hlywuzoc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pnfhvhof.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kfkbrnoq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ogcrgvzo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2injudioj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2foirpklq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ifrwnali.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2blytwijk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cdgizgak.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlddllrx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjoebgkp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2eehcndum.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ylrxcctr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulcuehcc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ejmliiss.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pypaxfoc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2plhdhypi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2poqzfymm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2txvqrwnm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2temhphha.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rzptnjwv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gkcuijwt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lugasbfi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cuteppup.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ebalfegz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ttmsqpye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ywtfmovx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ujgscmqv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jxvdtatn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fnhdvhmi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rlfcculg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gokhxkjk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gcyvodul.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2njcvmquv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2greigvpw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngbhhxdh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mrfqopzt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2yldshdgg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wynkvlgb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xgymlkif.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpkxtwcq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bscgnchb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fclggtmz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ilcbneiv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tobsmhnd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpagjfn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2egelbats.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qfpbonch.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cgselxuy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2sejamffe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpgprryp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fagvhlvo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edrsccta.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2royimrhi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gqbheprt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2blfdevlf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zyspzfcz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zsdhmomu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2afczjvmo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2atlhdwgz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2isrhqgad.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hxxtvels.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ssptztuf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sqhlgkoz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kiwgeygu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xbgeuimp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jxfbjjtl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bfqngkat.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bymogieu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ogawdlyy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2spwttfph.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zliusbmz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ljlslfqv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eoetmick.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hocpqbwp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wcqwkgqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgznxxbl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgmayzvu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pipdihur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrgctzll.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdarqez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tecmymfp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhartljw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gzujztda.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjjzptdr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2svwmyheu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wsqduejv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ltaxvieh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zwfvhaiw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwumpppq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lvneiedx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xrybroch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2udkduify.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rhtnrhrb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tywtalfu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ijjhaevt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvqilqe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2erxjnfba.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wgiibmbd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ofbepkej.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bxtkjpht.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2yisnjaat.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ubalksfq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2otzhdzhm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qvqgzksp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yfmmctsu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2brclgajp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htlnoqwb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kdydnzoy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lhsindve.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pdjwjrke.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ilhdftsv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlgtlgc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xdztcnec.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2goxpount.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2auxyvuby.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sjfqfgws.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pifevgqd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vzejqhei.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2huqmzurc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hkbdifdz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ijgpkudp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2eoaodnfw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2etbtionm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2afhaxnrv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pbwngvfx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rigdmtku.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mzqzdrgd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mwcrkmci.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2drvcnrtc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iblvsijz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wvtewvbj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfgeumv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qfghqqjn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kydkinnw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zvhxtbkh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2exezruvk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tmfptzwo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zriwbflm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xrsistil.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yztwlboj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kowlypeh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2urxrqody.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdkeefm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bussonmb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dcmsmybk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fcuypgnz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2epcwirbt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qglpsgcr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcfozqgp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2endrauui.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjhvndpo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pcphctwl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hfgbuvmq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xbpzqxsr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dddunzcz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gipsgzzy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dqbmxtcd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2weepxesn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sodaigli.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hxaozbkx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lvbwjubg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sjbzjubl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oflolwsg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2slqvbgij.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mistlzku.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hkkpcqvl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qaejzuyl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pyrizsbc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yuifizjm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bvtrmbhf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vtyfqvpz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2exusvwcn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hyyrphoe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2btefbhgs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2iknykeah.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vtnuvnjk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xioctvaj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ydbglsnq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kpuoounp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qerejrqt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yxtmsqig.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2haekxgyw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iccjdmub.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rseiblsv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bdioqwam.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2sbyuwfqz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fosuzbeu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jmefzepm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wykuudfi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2grkazbtu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjaxmv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sbbokgmv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2esoullqm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gbbchfvb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bjxbpwlg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rdjoufbd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2paxreaor.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlfynroc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwzhkfcp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xirvocgi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tzeeegzp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qdygxsmj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mlnishnd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pxdddqnt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gdnqcysc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pobbpupp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hpmztbut.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lvrtllso.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2psjoxxfk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nziwwugd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tnqghjhv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ahflcuxq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hyznozxl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qaxskhin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kpukxphe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nyuxvxwn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dktxdhvc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fteopvdl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bclaojfy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2chrxlzkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnpsndkt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vigynveo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zshwrbeb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mivudhux.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2djbhfjws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lgfedmos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hhiimovf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2aeasgzfc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rbxohcgf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wrmlphzx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sabezwbv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oytrdxst.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ubckrrfj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vkafcztp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hrsqlxyc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcxxmmap.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbpnuzej.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2czjlnhfz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2amrvxzvf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bxchlxnf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qppgykug.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hivqflku.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hzrxudsh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2epqdyggm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2syjkvffq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rkpetzih.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fsnujdbq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ccwrnsah.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2elvrjxwp.html


<!-- 参考信息 -->