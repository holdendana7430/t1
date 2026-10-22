代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ignjexee.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arzjkhsa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dpllnafd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apggmpms.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2emnauowh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kbymkkal.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tbfhkqwy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fofqjegc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jidzhqbg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdpsqvcw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mwpyztgq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2igwonlhw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xgudzcyv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqdkxwoo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rqizupsj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xnmegqbb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qsaucxyp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hdyoixsd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2aowroalc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2elccszhr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2upxsrxko.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wumtiloc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpnmrxv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjkhjak.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bfkflclw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gqnktzkp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lffxuyem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujsjzowu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kkohvyeq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdwjagwo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sehzwftr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2trssynbm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zofqsnjt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jafbkaqi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2esuumpol.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mylcbfey.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxqxskj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlkfrkj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfrqgivq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vewtrkzs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gyiruopd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2awdlicuh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ztamapny.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rrnrntwe.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zjchybky.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2msgcwmqf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fkxjkviy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oglsdmxg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vztmpvcb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rwsgilqx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ruunqtpu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2falipjag.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2flkxurbn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2niplrqtz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixqqolzx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2erhhmzui.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kkjrwigm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmvpksz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mvixmjoo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjqqxnk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibclvkeh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ozpmdqgy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uptzoraz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrhwctge.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2sazsninm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iargwsjm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wimiwzop.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwfcmtlv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wsiemmwv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wlodeofo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jdbglsoh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2svkzejdg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2siqzasvq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vrxuihbm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fnlszqbg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbbrfxqz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yykrntxr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kelbentr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mrpkpmlq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eopegwmd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nzpgqimt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rffobdkm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xgysafzl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgqtkyed.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tfjxajbm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xixpdymb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ehzcscjf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yygxasdw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rrmlejzb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rszhpqfw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2scoqcuyk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcbeglj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjpqays.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2foskkfjp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bwijuwmv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ilgzgmwk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rmijndmu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mlpkuoez.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zjhadlfu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mvcvsbif.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqcywsza.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kziaqbgr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2atfzftrx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkwzcfvt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gfxlzzub.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kesxumdp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2lvjzlwpz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2syxcnvtw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pcbtxphj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sndvicqb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jxlrrkhx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mrkhvczd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dkmshiro.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qlljuanl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpgoupei.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ljmgespm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2caumtakj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2foqiysnj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cvvwtkrh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jweldkni.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xloplywx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tvdttwac.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sfpzqdqw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2arejavja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofukomgy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lmopbius.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lykkwttf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggptqzrn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2snzzhnvq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bvfypfea.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyusxgmk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvykwmcy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hawawrin.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jqanylsq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwqfjmne.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rstefofz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pvpjkdzm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ptylusnh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcuzcvor.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cewvpaxf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ggykomrv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bersnzzi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uyrbwujc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fidbshnb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hatkisjr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2btxkrvdk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2meiaaxos.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2tndfuhpf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2atjwcjpa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ogzesort.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvupmllk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zcdbnbku.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2temvumjn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vgabmzff.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eaymocqy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wanlpzcq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2scsknigo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ruubokry.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ajwxxtdd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2aegcmxhe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sldwjcql.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2szckveqe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xgirsdim.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kbgouxbq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bsrgpzlj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dzwcyemo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cgvpsskn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sezgfjyw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fejdragi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lrqslijx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2krgixtsq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qquckmxq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vqhmaoow.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2peebaawe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fidqldho.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2srztyvfp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwbbqgy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jpiwxfli.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xgebdufe.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dvmrqsof.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zismnycj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2flgdpgpk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sncfaxev.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wgtmmula.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ckxtzqzt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cthnprmy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oyvcvipy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2edpjbtps.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zecsrbqn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2eknlqeqd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gyeppbzm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zzrcifdo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2puqpgvrk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzmklvvl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bcyfmppw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mktbpzpd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2teewjzvu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqxruydu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gmvqdvod.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2fbbmkqrz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfqfylcs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2szquiubo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yvosjllw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2csfddcmk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlccwwqf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvcfgyo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2upjuwaxt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2obulmrsn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fjxksxjr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kvurhcmp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mliwtken.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2dqeimplg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dhxfasml.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pjiatjxt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cxlebshz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2poruxvkj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kjkonkvb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2axylfqai.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uqyfjbyy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2iiyilolw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xckyilur.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fdnzejqe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nqccvvrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xfdzccfe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pzvtzmhe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vtpfluvb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wocmzmmz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xqcqymya.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rdomxwqu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vrzglimg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2htmaobza.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2alahilsk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2negakucd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dcxmpjoo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2krbduwya.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2deftosdr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fwleuymx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjfteysp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zpxrqkso.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lqivcson.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2chxtojyr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rbjeplhq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kdiwowuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2irnylgns.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wqbqmzpe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2iptgxtbn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2avyqmpgq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pxsdolks.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqecgyal.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjfygbbx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tgvdszmm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ubgpkjfc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kjlgjtla.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kpgehvvo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rifwutzq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uomyivsb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2acehoeyp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2quxbsozb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pljfrjym.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qmqkougm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lxlsqpfh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wznduwvy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wqnkflbk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2twyphcwy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rruncftm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vbliuosg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fvqtunim.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgepyo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wpjaeyxr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmgogtko.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqzjipnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtrxczjj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zwewcyjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcbwjisw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sqdgmjcs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2geervuqq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zxqskyzy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hpdresfb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ryswueev.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rrfpmrde.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2viqayqds.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qgncjzkp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ozegrtie.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2byycgemh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xfjjmiob.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rndkghsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tgphlcqk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kpyvucow.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kjcivgli.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jenfdhhp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gutadndf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jvnzyfuq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rzdgavpp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ktyyikzt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gjylvuaq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nfmqxldv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iurqdvvq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xezfyxhc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqbtzns.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfobyutc.html


<!-- 参考信息 -->