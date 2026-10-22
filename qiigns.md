代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xdjpbzkz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ihkswtmc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bmezrzrb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mkplnucl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2elcrqkvg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qmmlcymt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mnjmrgee.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jpaddwwd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iqupxtjj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qpfmvvux.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ehcnyelw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2etrrzamg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vzhpsfyw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ejnqikrn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pxznuknc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2apisqauw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2bwiqzhel.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2upxtgwbk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfgnvuaj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnyjklmm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xroocwbi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uresdjmu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qdodrnko.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvbprgod.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ievnllob.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhxbcpc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2oszwixzu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekofunhw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2neslcial.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zrgaofya.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bivymvwu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tgcwlpfm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufrjmvsu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nqqzlqtl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ywcdpral.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fllclssm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bgvhglgu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cropdhor.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2alqptjmz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjwyyyi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kvfdkwpa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dfpiagzj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fpsvasno.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hdssyvms.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vetpkkgc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sflnoajm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xqhorqko.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tocyewnr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mtejdnvm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2liydbbwt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mttrgbyl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ffagfdfl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dwxlfiph.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xheoqcer.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2daydvzgl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tmnzuxxr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2trxdybkl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vpxanrri.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bvodcmwk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hdunqvmu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bvxnaqad.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pmbssbdm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oycfjxsj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2amuwzybv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zuwwkyks.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2leocuijj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cjcsolbz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cbwucgom.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugfwyoef.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2titucdii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jlxiuppv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2obdumxti.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lzkjrzhk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rrjfbinv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sypfvpbq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rhbrmfzz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zbphwmdy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pbjjrymw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jjafitde.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vzrkilpt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ajendovz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hxscdvmn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vnyvkygk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kdjooryp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2awcluhsh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2emdcmymy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rvvqgqta.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2drdsyhmj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nbpfsjff.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wrpvkqmd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ygsophxl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iclvnrbr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zgwohroj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gdmqlwsy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oqflxulg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lbhijkez.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gdntvlgv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tuhgnnlp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2khulgjwe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pljabbyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nftjepbz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rzytkwax.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2obopusvn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jkryvzyz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vefnwfbv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2irrwjgfo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2prevobeq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2oohovvuk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uauyjokv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zvpwzijp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fefhtbba.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gypccxjh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nhczpndm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2caqkjaqw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hfmjddty.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2morpaiay.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kbvmqkjs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qcakudhf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wjphinai.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gvluswih.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mkydtyof.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qqgsnuww.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cyediryh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mafevkzx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jxhyxwoz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2csetbbnc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2itnbqbyo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2izcrqtss.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uetkgisq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhwdrsp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vensecyc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zylxdsne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eymfycxa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nwvsnydo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqfeehiz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hvdfnkuz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lbcojyzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wovjddzf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aznxijax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pubyhnkd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jmkooitl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vbrkdbfv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2woiexexu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gemdbdpo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tfckzkar.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2amrekfhz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qpjrmgqq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ecajkfqd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrzlhkh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2unyqzwst.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qlhznnch.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jeoayeig.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ehfibujq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jinjzntu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2murmpsqw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqnbjkua.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihirphbe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwzaghfy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjpigds.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mhndahhr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezewteva.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2avklwmog.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2dbavpkgi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ssaihpyu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yyqdcodq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahsxlzwn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wwvzndud.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zgegliol.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mnxkhywf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2islxczct.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kemdiizj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fyntwahf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmtfuh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2aikeyzcv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ijqbiwaf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ouvagktr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2oojmhvam.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2daxuomnw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jgrecxvv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mzkcckhx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rawbzcjd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2edilfurq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2thzdnsva.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zicygcyg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ofgbqtgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qbvznqfj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yvqscfrp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ifnztbzc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tjmayfje.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kxyaruxh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nxdapaqu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmwomszn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2heazjppz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxeqybq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yutmspsp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xnpaitsg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqzfgke.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kkhevnun.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zrfkwqmo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pmauuptl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyknqnkt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxnwjyj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2anoiozoh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2acrycziy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pyoedypl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zbrfnfwc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqubcpnq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cybqnwus.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2thdzzqse.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wgsqtvpd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ueyylcqe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ujsluodf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2snkbbsrq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2matacmcf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbnlmpi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nfbnqzmn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qjrtyovo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xzvjelxs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pzsedeje.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yttjpqfj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ytvjziag.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yzlxowaf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pjsxqgbg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wnbxodij.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kmsfkzpd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2sszgiily.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kplsvtca.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rzdubpij.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zazfgiub.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2exktiuwo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2avdqcqqs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vdkopwfx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cqjaecds.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2junlrfzf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cqmalnbg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fwnfpibd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ldwewvvy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2baflplis.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzstdc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2guyabdud.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qekrpiha.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2worcvdsz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbdalwqm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qexkjmiq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aekkgeax.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kohenjge.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2umnlgldx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rzzyjcla.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vyvasrxz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kqxjhbkp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zxaugnwr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mzleyyam.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyxdszyt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jqatmayl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2szuajfyc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rvdmodvw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2aeonswqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zehveful.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ftgehrxk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aoqaruds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wmfwtgkx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mnjshvjv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2luobstvy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nubjaltb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rymkjbvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qudblvla.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aokzpfyc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pitxints.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vbtdurcw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ezxsehtj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2umbpdaec.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kzilzjgv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bvzygvbf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hzekudns.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mmtowrgb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tcfrtnku.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2caszhhpq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnocssmm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvlubnzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmqcrphc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sjflixxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbekndpb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cpciyxuz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ukyohgrf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wjxcuesv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ycawwmpp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nbvlcocc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jlhpoiyj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iqebtdra.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zmfwirgc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fxbpdgeg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nusdaloe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mqvrmctu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lajuzdso.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tlbtxtwt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2desxdufh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hzgnstoo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2exkbykcw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rdirfwtu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iagsjnwy.html


<!-- 参考信息 -->