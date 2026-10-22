代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cvrakzub.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2adpvelfv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxjovxmf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wirolrbb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kkjulkoe.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2jwtkovxb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2pcggtqxr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxmkgqrw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ifgrrdrv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fbtsvdip.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fmfzfeih.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2lewwuoez.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rcrldbrg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sjdtnjid.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dbhuvbar.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xtxykehm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xbmnntkw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qryewgae.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gicjvyiz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mhougvqh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oubweizp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ncloabgv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dpwoeeus.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkizsxhr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pngnsvow.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2abmhtbnr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jorgftob.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yvepnmtk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2woubmuus.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tawwowro.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2indhpigg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxqbedbk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cicpmzzu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2oguuwoco.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfgwzpy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xklxdcua.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qckzqrts.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmvfdglf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xjbwuyxw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2niwbpktq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujkbjmuw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gbvnwwqj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vfyvdare.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2chemqnct.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tqozhsyq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhautcsg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mbdhwkxs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ewoqtwxp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rmdcfktx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2coulyexg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pqjphbom.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2oquokwkr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bebdzkoy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcpdfvld.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bfqhugmj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cripnfgx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cuohyumn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gklykohm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmwepsa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2sruvlcmt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ieszfnpd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qzpmyuom.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ikqvgszy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qrpkakzg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tykyurxz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bzeplqps.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nkfhhaqh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vdqlajwy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ynqvnipu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gccyykqo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zanlusfv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jhltbooh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgmblcrj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jzkumuzq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2urzwuvzq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mgvhoqjh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2umbkcwta.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cvzvoviz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2irynexkr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ohohzzdy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kdaknznf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rlmsmhjd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvspvupa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgydcrhs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ezcdvrug.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bohfuhqk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2cwepjlkk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mxrjkmel.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kkrwwxqv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xmrwevrv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nntgcgfm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jhjxifcb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ftivbgch.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eaxmkvpq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2libcbuol.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ltvacigq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wojkzqku.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hfxkjwpk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2equdyyqc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2omwnaeuu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2taljsokf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yyhjdkzq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wvspsqsa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lxlhsgvp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hjbepiwb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bqxvdopt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjlkkyac.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zivveixi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vvpfpuyf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uubzcdzr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ftyrmodj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nbkczefq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zmgktotf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ccsvafeh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dpvndfeb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqelpiq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ctohsfkf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2skktyhkq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byxxveyr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pwgitzbf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uepivmcb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rhclryth.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2orwejqmn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yjkdpfcs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vnlyibxy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ompqelmm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zeaqiywg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2styeaxnf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zexsnsxc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qxwdzefo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rkpapvvb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jjuelkdn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2orxdwiex.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ngeammqe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qqodxjgo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hpsifyzm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ogswtctb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vfeejnhc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wltbsnrq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zduffqbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkugvoxw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ermrwvjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhltfvhh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruvfxcmf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cdmmwebd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmaltnqt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2obkwqcpx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2efuvzzrz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcpbtcab.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lpeyfuev.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zveeuvqk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rmrxhreo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kibnhwxx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rwwyuxrk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysmcwlki.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nxuclmpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2crsnwuir.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ruwcgxkx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvvxilfx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jtxgeryi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sjsmdgih.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2aclhtzgr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxbhsed.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2eudugosg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxeoohjm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwquxtsr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srurreyh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2sthgyyyl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qarpaaqk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ijwsnlvc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2sadxghst.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqnfbkh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2phnfbegy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bsxigsrt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aihqgtjg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fbanhgsp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gbkignsb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwnmqdgb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2meiksgiq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fdedyaon.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2evdarpdc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2unedhiey.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wyefzqpv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2crxlnnzr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kjginque.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2exxfniwt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ucirzxvj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bmrdoilz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vkrykvca.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tezgkqud.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2bdmgfmyl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jqqnvkgt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2akiiervz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tzockozk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpejtlf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnauubz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dnbsphfn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kdrodqlj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nbxskwvk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vwwsdftp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dfpfwlnm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcatbly.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xmakhvjv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rntjrzps.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvqrkrh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jhhiadcq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2numdfmnt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dqklwfju.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwvuhtl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwinukql.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rouufqtx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nwajoyls.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vkquammn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2btloapkz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2diiutuwj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wtbjikbo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ehnagisv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ycmmcxdz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fbslycni.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qcafmrvk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jexjgqxq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cxjebasc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ticmvxeo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2incoprzx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vooksoiq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nebrsrqw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ikwlpnix.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eojupmzk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vitqlimi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2asrrsjzh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pclosbtz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2beqxjlcd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2umjgdksj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2uvscaujs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fwqfpxms.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2uebgfrvk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nsbxypfr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zsafzjvd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hkvsgdfm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2unyqeiro.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ktkajadk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cfshmnol.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ovgsxtpp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jaskasbv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nabiugti.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pfwukauw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pagwndcw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lbmeiwhq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wqklnoow.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2iqyvlbvc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrktycec.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2toayahai.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pfmzcibt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dscgmzbc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2diweypff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsttkpsl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqkqeqz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2trtneumj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mozwknow.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2spwodevh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2omnyqbay.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wxxuvqkx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qidveoaf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lokravth.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rcbgjwfb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2imbhbrlc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hfijfycn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tqrmxbln.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mljpslzc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kuojhkwp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lkaeajqo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jyhpcnbg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xydpsvmd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2txmtstmo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rvhlwnkl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aojewudt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gdzwalmq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rnsfbtvx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bilitbuh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2njbifhja.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tpyehqlq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2datievsl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dvvtjtlc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghkvusvk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ozcxplsb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fumjgdme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2flnzecqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpshajbs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rnghthee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzaoquxj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2klfxiusb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mmebmuxe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wlmqvxao.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2psmkkvha.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rcvuvtmc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hmeygdps.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2szlzpeoj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2djnaruxl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pbewaosk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xxznvbac.html


<!-- 参考信息 -->