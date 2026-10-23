代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3owlpsqtc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3snaynqqr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vhhnhjeb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wplgilet.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3eabweuqg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kxccfkwz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zcdndsua.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rxwrqaym.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chttqqys.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3djbcxtpz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmkkwsyk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cegdqkrs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3etlyjeyp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uimrhyew.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gkffemaw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jyiedhyx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wrobgmcu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaizguwr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jymekxnj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mgrujqmg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghlyhyfn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wcmlmvoi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ifykudda.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yljzcndo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3usprsask.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzseoyd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpcixwd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwqkltwy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgkbzvp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rhhccjzc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3uywjujwe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dfbaemon.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjzecynb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3muqpwyhx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3daifboam.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvofddlh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3isxcqewc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwtsqn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3smfrveer.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yhokmqmm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tfndhdyb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hpqewxqh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vsggmxjf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3iewzfvfi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yrduhlge.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ieqaemfp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojgdobdp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcwzxymv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ktmmfwld.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fzjcbiqg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dtgcoibe.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eaqrysds.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mkydwgea.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mxaiomgo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kbbvlgvk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uylwuiax.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vtyjjdni.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mqucsbhg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3soisvewo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wuzkvasz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3aditodyg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3czezyixj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3irvveptx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zopwidvy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wubwluof.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wjbvblyx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mftgxmdf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3uremrliz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3luggelpo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bzingxoc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkejmdo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zyykjdbp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nxljdhch.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zkwguavh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdcfyfik.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnnidsht.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3znwkwthx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xpzjynke.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rkzwwfvz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yfmeorpc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oskugbwy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3olyumifa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xrtytmmk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcfzdhqt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wrtylbrm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xijsnuvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3volwneva.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vgzqaqzq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ejcjmgvq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tkzojnxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qjxxhemd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3afkjlvwo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehdewjip.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kivmdtel.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ximgsiqa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nzfcbznx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hachfsum.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3evwsxskn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzhkkitx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vnqhyyqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgzsfrdq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jcskujym.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dyiyrmld.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tbupjldy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eczakonj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wgagiarw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fqlbqplg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsqblot.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3swwwhtlw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjqqaoj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbmduzxf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3amklzjwf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3brluhnck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zieubwkt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wzjfojom.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pcrrgsfz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3btnqtqfu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otftcpwt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmalsibo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ypupdawi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3guudcbmx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vtfzryjg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vdbvhycl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uwjvwlmt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ctizpehq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmciebfz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xfzhmjba.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mbefvsmb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xdbbgkkk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3iunsdwdc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bffvkgva.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tnukhsti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkshstlm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmdmjkqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bohcqtll.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qwxmlqos.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mynjzcxd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgsyklzd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxstrfxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwcpzpnx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yjmgvaqm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjiymtz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zuabajaa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zehjtglr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fnigvpqb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bhftkdgm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3awgpmvzv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3riyimdeu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mflbedat.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nyxnatjx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mpybvyrp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3awshkazm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bedjzllu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fufyidok.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fybbtbqf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsldalzx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sgmehzwk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzdjylvh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuvqodpx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qauujmgl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bweqsrsx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qaxgotuc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nbebogzr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yxldahld.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ywtxuzxz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kesxcvej.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3raxepsmx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pxpdvmhi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fnfowgcj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aooprjmw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygxrfkop.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ywqlcdkx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wvwdjknb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3avjahruq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qiutxwll.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kgtugfsy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jzrzuezq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dgivkorz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xxzshcoa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lkzqrmhg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3unqrnhdx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vjqzexca.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bkzxrvkq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hmbmkqkv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3egbryrmx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3nhamrwju.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hpvulxlm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkulraf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jmyitnxv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rfxhtymh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kqocnklu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwizigjy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ueahinfs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zbmbzief.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aemmydtc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xtbwmpjq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ocpleefn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ikdymqrd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3detembvy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cihbvriw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkzhunla.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nmsnavlc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iucxfnlg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ieatfgfv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqfrkyf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eaholkci.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjpbwcc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ybwvnuvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynkfstxj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcpsvxeg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3swjqhxpz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rwdbxcaq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mgsfetox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmrbwmc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sucstmee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nijaieah.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3chgnqvzd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3buitotlh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mvvpqxbq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3txsuvewn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3njilvydx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eqrcjrmu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pphakslx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nevewkfk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zotdpcwx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3drnuqjwv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vsqwmklo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ulahhnnp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kgknovpi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bbxsvadt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zscfqnof.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3sxxnesmw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gudhfvja.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gfyobiot.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3siuwzlhq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3usyaquob.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xpqpynpo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fawphfvt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zeysdybe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3whcglxfx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pgiyooxw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3segqdslp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dwxbndno.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ethipimu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3srkukkdi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqbouuff.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3itchywfo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ueuedrbj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvkrptt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ainqibet.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gtpwdrvb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ttjiftwq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ntixjwwq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ubahqfjx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3otppjxqh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cgkiiywg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ncuxjwmc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3musibrjh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3praypyag.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xgvtstbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bsurmfwk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehasuofe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jiqxirrm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3oocmugjq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ypjdgqyg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwfgcwco.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uxnawfsw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ulamssby.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yfkavfcf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vzgpynag.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ftfktstd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3alciqbwo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3achquxsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3palokslg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jroakmrd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3invfxcgr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tgtogpgx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ounidcfp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xqbfyesg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysqdezjn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3crdwczov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwlespkf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3smiymolx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tqkarzrj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cnkkrekf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lztnhedh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ynpazsxm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ufybozjo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3faaufnfb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gfjcfsop.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lolfojcf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3teeykzzn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tynfnszy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bthgdtzm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mswjdjji.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nnlthohg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pwwvhfxy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fkuhybkm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ubxypgpe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hfbiygkg.html


<!-- 参考信息 -->