代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vgamyned.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qqgznaoo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uobzfonv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dezvnshn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2aioxosgi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gqbzbkdz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ediurfnq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zchudexv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rdzripis.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twwqscmn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2caxxgbgw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hibojdjt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2duazazzz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2paxlfbtr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nljibjjy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ufzymdmj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vehzswuw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vafwfqwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbmoucfk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vendurjk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2exlzjlmj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wzmjhrrv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gskioepv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2oumhefgp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nrqymlfb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdcsrox.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kqcmyttf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltvwtnxb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2inquwliu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2iosgxtdz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zhhjgoiz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pfgjypqs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vogcvrfn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wdwzleup.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kcnqkeso.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hehwlool.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2roosixey.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcajwutd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcgknemx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lqgzjgyg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2polklghu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kqvojrxf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojksgprd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cntjgxon.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2erwdcmka.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgnpzhqd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rxpopfni.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hccgutni.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2brajcesd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpmcubyq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hrysqacf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jweepmxv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dodbypoz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rlbcyziy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fkkbgzbt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xlxiwpcw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uxdjaybk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xdteesum.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2icaaatav.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kdpiyegp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2sxmcavfw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jzgcknyn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2egxddbmd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2juixfesw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2umautabo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrdkadj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wvzdfiwz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrscnuqs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2srekxlzm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nkjkpafe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2htcdyuwg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdkwpptz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qgxztisf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qadjqmxr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bgnzgjym.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bddgxxsc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2epbrclwt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmwbrdzu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mzsenfor.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kmtnoknm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2atpeubcy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yibiagod.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nxbzlpoa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gujrewqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2fkrgtmbi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2znfjmmpb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wiyisnqd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2csdtzcif.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ydsfcmfg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mfdtbstw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nznbjntq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mwkkyxis.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wqkzzmey.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukwsivaa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ajglituo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gitakrkj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hnsnnxev.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bplnkogb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bevklems.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2azpbodhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dmwiskpl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sqeutbfy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lrcapzwp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjepxwe.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ngnklhot.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fpsitfpu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2knlocjud.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrmtreh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vykiutix.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2winmsfdi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qntofwmd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcuzqiky.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozvrljwf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xjfusulj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pdwjbgyi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2juexaewg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iwcxomki.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lpwmzmfe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wqmpiijl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tymeqnxs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aaxwsgtc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vbtlkdfx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mhpzsuqt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hbxkhtcv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kcxdohgr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lslfirfe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kjhyehyw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zbfxkwbp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jzsnuzuw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nqggeqxs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vnobxzwp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2knbynqsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvszhqqp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2btpxrxxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foiwwcjy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pfxaehrr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sprlquox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pongptns.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqihhkzt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lzqzlvwl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jonevcer.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vqqauwql.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ovlbmrkn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ndmbfwpe.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nqacgajn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zooklafb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2igshrrdn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcujecnl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxtsrcng.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jbeulxbp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fhiuhpfe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vblcnkrl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vupexbkp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fnekkhnk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bznbxmfk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2geuopgtu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxyhmwtm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vwixkdag.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mudvvtmg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dfkgeifq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rrpzqquj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nuxftuls.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bksmutnw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2msemqzhj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2iaizzqlm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2goqutzij.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xhlqmstl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wksufhxx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xmmngqbt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kxmtwqjw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akxjbegu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kebhiawt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sptwbwqz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2grufgnpc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yckbdbuw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hnzpowwa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kunaxhls.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ecbstmne.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mwrzbevg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bfofgyuw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uwhstxol.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qwygimjq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pkxlrufv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2utblnchm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hwwcxvff.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vpcxgeoj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bqwkatrl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qzjzsusd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2auxwgmyy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2euywbvgp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2obzpeode.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rkuhuupc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2exlytvhq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2nhxlbvwo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2itxjkgeh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xmdttvps.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2glukppwg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xqrirtng.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2iotcntcy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pvqmfvhk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ullhsvqp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2chnwxuqr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvjsvuv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zrsjpogb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2blzlnslu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2glpvsngm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wmdcxksc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qggyvgxl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vleuhqye.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2agbmvofz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zegldnti.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2glugxhvr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2niiesgnz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtvzxap.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xzntkspb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lyifysuk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aazikswl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ilhirrkj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2muzqngbu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ancubrxi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yaeksmop.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2akpzluge.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2frprktot.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gzgycafz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rtikhsnx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2imkfxzds.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mtlkvtch.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tjouvffr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2scjzxfci.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpgkud.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rzumbjja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yjnwhiig.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qcwigfqr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pskfovah.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hjrtwirj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jlftrtmh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ejpldgxl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mylrhoxg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mfafqzrx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mkptlbqt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wrourudo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jlkudqhr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvaiyxbl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lckaqdwt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zxmmzsab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhtpkkv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xsdaijto.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lgeizisw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgibndaj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2acpapkdl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ipjpmmbz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hmucrzou.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xorahjak.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kdughcrp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lkpzgciv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yeqxfjdw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ssjbirtm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2izqkzgxe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jwpormyw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hcuywpmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hehyvcsk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wkakblbu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zaywbdax.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kemwvofz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mduegxkh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2clrjpvvh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2widswpjs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vexmvsdv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ubhpqdax.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iuslopfg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xhxbkeos.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jxlgpowa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ryfblolo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2edqlrjps.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2chyxqvhg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ylcoiani.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2fekmpied.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2myqjtmhy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqgletpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guvbtzvo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2usrupokv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bajogbxu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qomnmexm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tjitxccd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2roywrpmq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eufsjcbn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zjrysffm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xwjyrkwg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gfdqyiyf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qneyslbk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ijwwalwy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mkexghsx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ckgdtune.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2apibakao.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hqchnemh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zlnfditi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2katoefpg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dizjrdes.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tvekbwou.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aottschz.html


<!-- 参考信息 -->