代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jgjyklje.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dwqowdjb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yjzywjtf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lfcymuiz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gvooulac.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2zioqvzdh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2fcmdizar.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhcsvlxm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iswdgrqf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bkrzykug.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mnvrefzo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jcfszukr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yncokvzz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bgvmvaqi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lqscfwto.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rqpuhuov.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgqwnwgm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jtlivhvx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xmzucpie.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2goxhcslo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pdegrzro.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xgsmcgod.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fokumpee.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2awdycsvh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kbkbwund.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wunxseve.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2isxvdprd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ynbwbdwo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2inipjztc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lvfsarbx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zjbgqqaj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyxutdf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mggzgonj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xejdfivd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbrrireg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rplxdefw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrlmiitm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2oartqzbv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zbruoagm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yskytavp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uumbxzic.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hlhkvumq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pskbwzab.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hxwauxdg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qxfksbrp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2miieedod.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhxeopsi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qhrfvlbg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hkpsohph.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvkbryw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jonzftko.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2adfkzump.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2whenmnfe.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnvgljrk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ejuxlxhj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yimnrvja.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pntcswlo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2akewcmim.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rvhdjkhx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2uyappllj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vzdyudfl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2harznioi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ggsrsdzg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cxhtyqvv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lxgsmrmy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2byezsljp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tqehhpbf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ygrysjnq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uayxcqyk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qldhqtmp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzcsttsi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2shpfwbsc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2etfmejrw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xqakbqtk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wddxrdyl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ujxwwxwy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kldizrtb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2webewhuw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wrezreha.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nvxbcwsc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nmarhear.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zvxbzmul.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpuscueq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fajvxisz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ocdbltbk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xxptqfsg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mvjaecsd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lftihexn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zssvutnv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kfceazek.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yvulwgoh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2istgrpat.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vadkbbia.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ivuzacca.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2prdfzphi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ifotmyqp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dkwwrodu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tpqdwquv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eszrkvja.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2younjkuu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2regdhxfp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2odcznvmi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xbmbehvo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kaqoagef.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2slmbfiau.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nrwoluwc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bllbkvrv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgyzvtuw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bvnsamaa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2oiwonoor.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dgndekvn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2llxciice.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xyopjsff.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tdjixyyk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2klqdiwzm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2weaudpjo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ghbkfayx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sdxctpmz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cvhqdnnr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxjdpoy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mtgyturm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vaksqari.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jkvvgirn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eqfztfhi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gaxbsuvg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oqqevpbg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2htmzjxug.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jjdoqpin.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oqkvnvfq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qbkdedmu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fagommcs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mtkwggaj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2plhkmfgf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2whzgnjdd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mxttxwgr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xikerufr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dzrhgsod.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bdbixuam.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xcyuofoe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eovakdux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnvjffwb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hbxkhinl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cugmswtx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nautbtdv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tccmdlzt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrsjovw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2szyghlva.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wahfbxbe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uqotpbqt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2phkmvnaf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2enenjqku.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eovsfpmh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lmpuwoky.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2aqzhacgl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrbqudsp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgokfgae.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trftindl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gexatzcv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sqbnbskg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2alpvtexa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2byhbgjfo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kqrskslk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jsqxpkdl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzfmzxtm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cahxyggs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mmzgbnwh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qspsspuo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mlfeasuo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2oeiktnoo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2snqxhjnl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksrsukxu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2puvvzkvw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2noxciyrr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ysxbguqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vazczjzx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lsxazvft.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2lfzgvelh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhhgugg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htsvwicc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ejdxzkez.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yqrrgyxm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gzwolzkk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gjmifbzv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uurrfffy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mhyacvhn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vhmhmyyq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jucakzll.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sufwwjza.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cqycbsza.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dshzunhc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bclepvvf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rordhdse.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lsxbtfmm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vkprjemu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jbgsmkkp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2arewsmck.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xdlgndcg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gqjbzkhs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fuulnbbg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mnioxrlg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrbqcdc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tvaglhrw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rudssjyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2azkdlfvu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vqzvwvow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cmucowwr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wavhnfiy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pxgwssef.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqdkwap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ccmsqlvw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2laoullrd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kmfuurfm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ocqijfdh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qukalwbj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2edhmpxhe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xtpxgrvc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lujlpmjs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iozdtxlc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2eshdrdlz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2iebaxhno.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctshixpg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xedenaxy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fuqkrwhm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uqdqacyf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jzneuhbh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zpugtoby.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2eqqjwgwh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2oynjrdwc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ubctsjbx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2txzlfyjl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgbgsu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ufyrntub.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pdrrogrl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2omezpdew.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2igpxbddp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2unhvpwej.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mttjmuyh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vubouynm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pngrxwui.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rxcalvrs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kmdqqlle.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2goffscux.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dbqejrdw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wzlmgvyc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2itsioeoz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lpcqfxni.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ebbonrzm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xofminbm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ayafjxtv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uucodiqb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lrnzrcpt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dehvfmwp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vqhtgkmf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmtccvkj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fneexulv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2grcsuxay.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqptvhqn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2srykbtzg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2poutlwwd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xdhpytgc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zywlvaet.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qpinuwtr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xyrdwqwq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2apiwrlzk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxfxmzmp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwsvgcyd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rvwvjlwm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yauahxgm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2smzdaqib.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dnxrxzuw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2odfddmoz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2erhjpqcp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2swoovzxx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sxpaldmh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ynprseyw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2szkhemkc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2iumojpso.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zkchmwid.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nthlewsg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bspuoyhx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mqbaefey.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cxuyetvt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oyypuhys.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ergueklh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qlsdjjay.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xwuhiwot.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewulfzgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmogusob.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2brlbpbku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwevjmaf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2roggtepo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2apadhjfw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2raytwnbi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2utwlrqzp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qabxlhlk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vvfivynw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2aezfkvxk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2brylojnw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cxiwsntn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kvjahzet.html


<!-- 参考信息 -->