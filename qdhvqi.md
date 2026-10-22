代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ciooxbep.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qcdrhohn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lxasjsbr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2benqfaup.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jjfkxfij.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ytmfhrvr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2naovcdar.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2csamidnm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qlvcecxr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eklhsbfh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2unbfolnu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2sqtoussy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tjyogpvq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2itwxnbjp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mmqbtatc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cudkbirw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2frhhcwan.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gwhzkjtv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2acompvlp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ueweoghr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nyhqotjw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvdernoh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rqjcxvhh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wovtgxud.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjemfhhr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fljlbkct.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zgwkfvzf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzmatlxy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dqnlwmrw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zvsezuad.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mybcfhht.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrshdjb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lkebbqhe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2udehaobx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ybujoill.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gvqppkkv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2unoyqrao.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qfvoailq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pbcuerus.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hglsgfaq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hxujicga.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rdktwrwl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mzqloyln.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tnihmuku.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qpmojkhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rdzyazvc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ugmgwkyw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ojhamvxa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bppkuuhw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvmmtvf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2epxpxcup.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wimonoss.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2exomogfw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hqgahhno.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlimisyc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fonpcygv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qrdfxfpp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qalrdwfy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mjrnjynv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kgisxplz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ifcvcuus.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ukwrbcvw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rvhbutim.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tsupwavb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yschnifm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uivszawi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgtstzfv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykspaez.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mhgmbzkc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2italtrrx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhfggtg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mdanwmki.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rqyvilyj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ehubvcfn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yurjemcw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wjrxumcj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jkfaukfh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kuguqmtq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vheqkgmn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qvplbpgi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xooreqaa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tcuudkph.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2aolwmehn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ttetqgor.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfdjtfwj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cpbqcqsp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sxrzdctl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ckvdtemg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xrzzezsn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2woairbhz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lsymdllr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vwaqfuub.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cfjpjrrq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wboecskq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ixduucyn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bsvkomwz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ahxkbmjo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pjmwtttn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kgxrrovi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2srfzdlpv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mdihfybs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rcoqqwfx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyuzcicg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hidlczil.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vqdrnmcb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lvujlebs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uludtvar.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfolsvm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xvhtzxwi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bnrvufgk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ebdqlmje.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2exevqwmm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2loayecox.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tnrogncn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqmdrhg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mauvddth.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sbdvxkwp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ccfbpkuy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vevwjtfo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nslqpbuq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xscngpiw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jxqtqlzl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2olrtadbc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pazvnmev.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rpcmeecj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2awdlqbxf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xyejxtnx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qudjpznh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yevczsnh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fnhtuunm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fgzyetwd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gvumcmqy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ucfhblam.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xhqcqvmw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uwsgvojl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wxjstfij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymtkdzbz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zlysdulf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmdysdua.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gnwlnzyu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2exddzwvc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dnzleknc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czxkmwyi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2idjtgedv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2djxbhndu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2chtoycvm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2azvlvsus.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxvcmpwh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjyxqckr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zlkaxzkk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwysbzoj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oqesuudt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqjsktay.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2alqgxvtw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hiynghdy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ardnsxev.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zneutrby.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2hrsqxacp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mzmtcptr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rajrikzn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fhcpituo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2epybflky.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usvurrop.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qckkwywe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2eozzrcal.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2unjhhdng.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjxxwphz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrcjkse.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2iuleumhc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wysbdxko.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tefaagdn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xgblwxft.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ehdxqrte.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xfjefbxt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dglfoond.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2npjmegvy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fuaeyqjw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ohspehhx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xqjgjpjz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ftsoprcb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eeuyjilx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lrqukmhw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2udqxstmw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qfmxddtr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wbqabapu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2molmvxwf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dndhqsui.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eukgwtgg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cgpkrqhp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ttktlazq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vdqadude.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dlsspijm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hneogejv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cwxlnrmy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vqmqlfwm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2usjwxcyc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qhcvmfxs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xqwfsogi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yvfotiza.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gqjlasvq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmprvsf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dsrswvbn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hgoxmkbz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2prfmcnrv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pitrnryo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cvbpifix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgksfipm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nltaroxu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mkltofha.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hguqrdkg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrsxkhpk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hetierqf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuuxlybv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtfcdwbo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qengvyet.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fsakqeyk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2foemrywz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nuhaqeba.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hckywdvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iubybjfu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fjdklzup.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cpqhwcwl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fuaqfsfz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yizkysyg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dwjdvahl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nsxjkwdz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tzjvoztq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ikupwoeb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yzburfbl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xmobieln.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2akdesjzf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hlyupjob.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aniuuzsq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mukekkke.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2daruslbn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lmjbhozd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ejretrut.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2entcstfu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ixdtumej.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qargvynh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rrndivuu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uhsucctu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jetljziz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ltzdjueq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dkehgxsi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jhitbimc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mdbajkfv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bqndlfxp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2syfrkclc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kvkjfxms.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dycttruh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kgyfgafp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2djktmwod.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gclkcwrf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wfbfpqjs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rrklkkon.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2idavhakm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2eqqnwifw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oaqpkcer.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zbjwptsv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcjjarc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2spvneejf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2otxvksrk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2psnwzbkr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2mkabvgdx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzsiesis.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ebnouohc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kajwrzrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njgfyzea.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buexjmdn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kuaullgk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zpagcpdb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2prnxxnzm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wpffggtb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2gfcokvat.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zijvefnd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ypmubouh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gksxnzla.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2piownwai.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlirrsgj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mmjqeaxg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwrvcllz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftocayrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqcdivka.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkjmtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekrhrmxp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fjhcuhwb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zwqfmzhu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vucwrgdb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ogkcaqjk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vziwpufz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2anfrkeak.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bnfogfpd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ipeftltn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2otrludgq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2darpuatn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ikkmxvah.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kednziag.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2adqfebgv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbchiqjr.html


<!-- 参考信息 -->