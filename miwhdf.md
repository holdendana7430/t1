代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uonboomg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hasdjfzz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vxrjogpu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exdnjzep.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ufjhgpjv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2foqdcgps.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2oflhgibm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hpocture.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2obnamchn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gxxywesk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rbmmdqps.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tumdmowk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nqxmqjdd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvcwawjg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pnndmido.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2elttxhab.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2asmgnkck.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mnnkqetz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2crnfelif.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brrghxny.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nqkvtxwn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dbikrdxo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2eyocequv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cmjmaqwf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pfllavax.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ttkmgamj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ytiavmlp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjsztqih.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uhrowexi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lqgahxaw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvusquya.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gslwaves.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2igebhomx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pvpsbmah.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kgddkjgq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2harduqko.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tefsbzwh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vaxdruzn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mbgxclqk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2swwxnudg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wiurujlz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kbuzftdt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kfjrabjx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pxewough.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vrcaqkck.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2suknhfoi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2swugvuaq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymttvqau.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujirbeuf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tkfjings.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qcivmszj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2swvsdlik.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zfnnhutd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2tmpaalua.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpkxbdg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2euksbsoh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ykuhllai.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nflfyejy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pglyuncb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2deduprye.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kfpvtytb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2prunvxht.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oeevatho.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kwyncljp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hchseyrp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bgmoorbf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uqofbahr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zylcarph.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2juvwctut.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2klfddnkm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lcguttpq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mgfazkdv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dmltnwan.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ayzzaqmo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xkijicqx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2etrltdmj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sefibava.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvotymfr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ujixpsal.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xnitflyj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rvssjgkw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2oyqdfvkt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2krxlbfli.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mzapqodf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2guxqekjg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2feprxnge.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wqwpmunv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ffnwhmpi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2weggtizm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vtvqkahh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2atsdxymq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tssxuhvo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzqnvyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pdbpemta.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hwcriryz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqdcdnc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rtjxlwba.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tuaoedlh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pkyxfdpv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gwcsgxna.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2oxdrjjnj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ievoxdqe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sbqzqaxc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sdakhpiz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uymgbdol.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uxzscggm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2alsmouck.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2czdxagna.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cnmnopet.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2uyfblgcz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2urjljety.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tqqewxhp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqhcngth.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gxqgmuwj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nxwihogy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gdgrlssn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvtlqeht.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hnmfywsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufkssjng.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hvaahkut.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sjnlkopu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kpmqyxdh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yrzuhqdk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqmuufc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdymsvze.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xiotpmod.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xnwcqgni.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yfhxutfa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ydqozznh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tmnchzjz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kryvwprq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2khcbrbnl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2punpiaql.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mxaltqvp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2muxlfdhs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ohqfmpgw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lrzkzexi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2naxwoiyy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2slbydxlx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ywlwonna.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ihkogvfi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2garwqrbx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfrlvrk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2foewklyn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dvrfagcu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jdxeswnm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2awyoyhjs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2doyweahb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2konwczfp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vasltpti.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kbptvtbx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2oqfocvnc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hyjasvol.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nosalsww.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rqiracbh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2znqxilwz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vmhmmkez.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ictnlzaa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xgskwyux.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2csrpljuj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2noqgzvwi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qzezprjf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rjoyiuoq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ysikmgur.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gywuhfoi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fbzjzqas.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tzbeqrcp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2safouflk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mgwcwwpg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zbecqicb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nvccyevm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2feqlieph.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pastwjfx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qdvbssfd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2aqwkssvo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xaordxnj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gtcwsody.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qsjnadis.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2chkbdswa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ajkvbsde.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qqjuoxkr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2atrhnjvd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wmdcqdte.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ctufygjn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayeintoj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocyoxxmf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2njmvkxan.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jdwgwsoj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hwnavgwq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ucftonio.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2urkdjptj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pxijquyq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rarawokc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzkbugty.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2anggyfkv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vzmxhewi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fehtwaly.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bqizsrff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzzruoeq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbzlpho.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vkrqhtlg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pngmdgfr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2trmzzwuu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tuoepaqz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2brhnxueu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zunwvnnj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zpsygyra.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xejutiyf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmsxhjmy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2polasvra.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2uugdckkn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2grditjmn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oeyebrdq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wykvmfgq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2squdtcsn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2leolsgmq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nxqhofef.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2oliivmls.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wnvprqdq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qiimvogl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tuaznlew.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ggdahxrc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vafzcyol.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bldgtmbd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wdqdvcfa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jbjjoyjf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yipfsmrz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wlfnfgon.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oxjxeqdc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwyskazb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2anqcdbwp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mczczgja.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2twngzqwc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2sjnbmjpg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2yhkkntrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zisyajpo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2weqxbqub.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ebyfpfgo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ltvpniqh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2agesywdc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pldvfput.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tsqlwefi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2urtydtbz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wuldpnre.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2byygiktr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eztrtqxn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vcpnbrod.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cawcbozt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tiavoqdo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qgzjfrjo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tddqcpls.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dmpjxuym.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uocjjeat.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lbyhimhf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zcjugzok.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gwgmtukn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pkldkrdp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2olkfskmw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2guhtvmgm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfnftrgb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pydagsnr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2baynancy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rzbtusrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjmzxaug.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gkcnwdai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soqmeeje.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2saqjmtdd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gvwjgjjr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rycziusi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iyobqsuu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vmntdcjm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2umstioqm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bumwkzem.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahtbnxao.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hplxuaxb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xdisruim.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lwscvkyb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2stnysckm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gmmvkyai.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rnfgdtqm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ksktsvzj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxnurfr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2pxehdeum.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dpishhvx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lgainylf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2plksrsdh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2czrmtarj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zndhchzh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzyguqdj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kejhnube.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xfnfujqc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fafomqos.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aoasagol.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zbcrxtbi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fccdufix.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iysxakzm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mgaotcig.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ylpfykpg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fcrxhvzn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdpkmxr.html


<!-- 参考信息 -->