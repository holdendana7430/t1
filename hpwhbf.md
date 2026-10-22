代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nrztyoos.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vgjqxbik.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kmhnkysb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yipglghz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2htqigimr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wnaclwtd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gtcqidfc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tezsjyne.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2auazwnuv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fxmposlv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mlrcfaoz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nououqjd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzwojk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2khtzdqan.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hsxpbzlh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fkkdgbpq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ennbntei.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wvxonrvj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zkuohjsn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2joacjbhk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nvrqehnx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2neikmhjs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lkjqujha.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejlxuwbp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2yvsydjpf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2odajupjr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2roixruci.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kavqngis.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ghfbkkya.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wdqbtjaa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2faxlawba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2goqfrlzs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqzjuikp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezolbbwn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2akzvbtcs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwaiiti.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gmveivyd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sigxsqbh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mwmtgrbd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ennjappi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2srwazbzz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrcuhhxq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2sveyfqxr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2oggcpniw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xfspabkm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jcgsqtay.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kqtuegcf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ezxbkslz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfqeyovi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ycoeieff.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bjpcumdo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxjvtnnp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tysdvvcn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2cvzfcnur.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2omvzxzwm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mrcovjxo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fevpfsho.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pojnwehg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sdmkxrxr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dkkgpfoa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2purfknox.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dakmvfct.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lkiuzkzb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hcucteyi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ffdnsavb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2olszjbtw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsavnbf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2htrwyeth.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cayzbenn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xllqboag.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdmeggdf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbkwqhhj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lywteycm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bidbnjtg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rhnjebpq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2frnbzgwc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lpxaqdzw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2etoiappz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zarzvlov.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cmsbwfnl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xwibukcj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cijimlrb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hremmwkk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vrcoieqy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tuzzwwcl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sgcbrwyc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zacqtgwh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rrokfgcx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zuquulfi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zxsnpuxz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2khwzckeg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nbcecysx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qhefwmyq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nwduzmjo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpcbrmah.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqdypzso.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tkcthgjt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mdygpcif.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fgczjhyb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ofyqvxat.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zqracmaa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lebyiuhq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2dlyfqzit.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zemzwsph.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwkrzca.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zznysqnp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2whyldlii.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2acukbbjl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mjvgjaxv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vfvrssfc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qvixqhan.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2opiyemri.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bcblonki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yajajmnp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2imlhxmjo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlsmmbyo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kxgscomj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hckfftob.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aixfotdp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cwldrpuc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gscdhsxp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iysgbshc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eshfkpvb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mvgircwo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ttgzqmkf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bcwhhswl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oclrpgvo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fhwltdwk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wwbiwcki.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2faixuyqv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2njcjgycw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zucazhhe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bmzdsefc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2djgqmtzn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vyafxnow.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cqbexqfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfuycbxd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ibmgpwuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzisnddh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2myvnztbu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qireuovt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xpymmzzq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjhsvxwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgealgvs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfyotfee.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jmrkcldr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqkwvfaw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bjldsirv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dqpntmqu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2iaryeujr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifhnvagw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bfivlnwk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2smztkbhe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ekbuktmt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qytwqxyb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2agylblte.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rqqdavna.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wmyxjwks.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbqyzec.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gshxxurk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ijotdvzm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2shgheqes.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msxzfmhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2iligobjv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2angbmxou.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gsgsisnk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tubkovus.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mmykmkxq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jiewnucw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfquvgrm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wzgmpfxk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2crnqzkpd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2prwknaab.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jlulapbc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cionlazq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pippgskz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xihgfcoz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vksnxjak.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jddobdrr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bxwlryxm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tjacbrmx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rlhrhnrr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2llnxdnpf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2blibfuyc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ivfzhddb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2enuikklu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uhuaoegw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bjkozjab.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lneyzkjv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zovcgztp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjomqoh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ozjptjkp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dyrdezqv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2idxhoaea.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rfstwaok.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cpnpssqi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rqnqzhnm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2awxosxbd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2llvwbvpc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hgvmvkvu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kyuhyeon.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2orucomti.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wxreyqes.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pxldskes.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpauelyw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kwkiepnv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rqpcuplo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2anqdnakk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dswccebr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jrnmgygk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kliosfse.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2klopqahe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gbqxfjlb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2swofcrti.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vhwwtotq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mnzhkpiv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecdlbwwy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yeeznfys.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwzbvqwi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2svbeherf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mbassyfk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fbqssnos.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2iklnkhvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uvmzqrrp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jgvgufqx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uqdhwdxw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vbudzgqw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yxkylasw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cmjdrghk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2njklweja.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nneoopij.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kpiumwto.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gbmjmrea.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2odeesonz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vhqmvuwp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2iqhjenxf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2timcdihh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mpqtjknx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fkdtlphx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ftqnwouc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yhvdhcry.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2btnrxser.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qbjpiyga.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2clqupkiw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2drirmeno.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tfeapzdj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkozfcwn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hcerkfpn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nsdzgwsn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2afbvmgwd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tunxcxlb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2acyfpduu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zkjtmwyg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sjthnqwt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lkfrkvpk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rmlephjz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bdhpwgav.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zoaiwdat.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vabjlmmh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2drsdkiio.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vamanhoo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcewqlkr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iohajwsn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yssvclqd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nbbaacla.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvvzvylc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ofrdukqy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lnxskcxp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xlbwoqwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wmjduprd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ofcjffre.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zsrcvxpi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2codpjyic.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gzdawmus.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ijxbptar.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xmcugtdr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wudnzamb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nspdiijl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cnsudoum.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dxtjkryt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zuxrezoy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jncbdjvd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uspxlrja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayzeylsv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2neszwzvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etuwnyhm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ysoqkmjj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2oynycqpv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ecurjmsb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wbrntnhu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gcoxdjhu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kqcdeyzl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bksckwvl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yoqjtqby.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jtiyhnrb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bmtnxltg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fhnyivkq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjwolkse.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fdigwolb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pxbfoabr.html


<!-- 参考信息 -->