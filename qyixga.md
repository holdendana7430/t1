代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3guvyfvgy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsbtfizc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xwvhcdvy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vydsdrju.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3enpgiisy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kpiieguy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rcepqcyr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hkwzoedf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ukaqggsg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qtfilqlz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qtfhuptm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3awqixhnv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbleqvhs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ochllule.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ellfzvuj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dhkdesaw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyihsrdl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3grbxapmb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kgwwwaju.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ohhcxgpp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zawvyihz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yucrxqwf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tioikrvt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vzehobem.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rfpoprdk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hsssbuja.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nslcuvvm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3efutohrp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ocosgtse.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtkurlzq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3urzugsjj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfxydzyw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3sddndbmz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kksycpbx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aomlgmsn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dtpnfhgj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3abidhzik.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xooutqxm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ivdfrsae.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkiernc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3plwleplr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wrycimon.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jxukxqgb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3idtmjbtj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cclhxraq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxzqgyfp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jhpedaxf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3czjlckjb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uptivoci.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxmadcov.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3txbyhgur.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gztksnra.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fojujnrz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dzqlpzfq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rcfwdlzu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3veziyagc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mwiyazoa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hvabdcoi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3frwauukn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jmcvlaxf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lyclywzr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3twptxqan.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hibzqebp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3iomabuqj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kxykyklm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3erplkboo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hyflchpu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtdqpzzt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dxhnhoax.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xmpjtrrx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubfewpmk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3axfxccvh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ofzxyzua.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pscoqrcz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3akmlaiex.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hotepmau.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rklmkzjr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3acqigzgw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tttxkcbl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pwlwybyx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zkfaogac.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mpxhukep.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iynpaoar.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3timrhdsj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3csahejqa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vxplgddp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3enjtdjxt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rnwuflac.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3elsuxfvu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nhrsfsmw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mxaxcoun.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qzuduytv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdahuqcg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbynyghi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3trghltfd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ubhtqjuo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gkbklwzf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdkqextb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rpplenlz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3stjtkyua.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3odwyennv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bpbziiwz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3faddcedc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3labpqpzc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmbhxkji.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bzylfhnf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hbyuqtvc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3assgqror.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3htizldzm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwwohlxm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3idhbonis.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3grmnvukz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3apdrwtmo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yhfgmmil.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uteicltb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gafsqmsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxbrxsbg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yzdinjjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbhoejrg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rdzpukhr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3evcwpeua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gobaeywl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bhjnfegz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdjpqmpf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gdurziju.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ezmxulqr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcxgstsk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rikyzaqd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3abjjfghi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xmxoixrq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3riisfrpa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tsctkymf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyaxtwxb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kgfvaaxp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lssslfjk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3exshrekg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wcbnwlzi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3djqbnxnl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3aubneacs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3izlnklyr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwazegog.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lzsyzimf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fgukdche.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uwtcgwfs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fufupnob.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ymimjzmh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wfruxrty.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lpnposyt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfndxrko.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzuerlju.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nveqkdgu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bhqnspby.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uwrxycgs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3egiaxcnd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tgbbnyvb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ymmpuvuh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fuhcgimv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3giouszka.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fhsvfwis.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3enkpwamd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vkhrxsvm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wkkslqod.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yachasot.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pftlpiiz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kuiqwhqn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ekknvoex.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wtqprena.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xewcagrd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dynctwqf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3guhtgccp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfndzls.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vhgfgsuv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3htgpqizm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3oyilahlo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cxunopqj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mkppifka.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oyflprek.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gvletnnc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3quucymik.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3iuobmqnf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrpdciu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3parzrvjd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3subiowaf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3seguigug.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hwufxfwd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bhzhkuyw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kergkoli.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cjgeshgl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3eezcgtko.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vadvuuub.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3upbrjzkn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kiunmkqq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgcfuxpe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iznnaxmq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3otrartgh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wgksyfga.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3moinwjag.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfumxcrp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3davmjztq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jswmjjdp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3plimkjul.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3suxcgczj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3anntqtbd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3onptamiv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mwctkone.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qggumxtz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmtqkwya.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zhcmyckv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vmoleheq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fxlzlvgm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pocppnaf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vtrmysny.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xfxyyonk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cyomtprb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jdcdqwpq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qdorhiyx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fnmvhyhs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3amchxfhy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lliyhzzl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3zloayblg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fszqesjf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hlgjhoyn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aphtzlll.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yhbqzqyt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3szjrzuqw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yddtexcd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lhvbtmxb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3iundvprb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uisuwsqo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxgfbgmu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vswaxsao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mbmknvaa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryckvkaj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hpyodzsu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bavwezbo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3odoqokgu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ryvuturl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3drbhouio.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tmcnihcy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hwwsstfa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3igbdpcqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vccajfxb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qvozhhau.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ztpvdnoo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ajwjwcmq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vftustzn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3umomtwog.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xfqveign.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vfilamti.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhuqoray.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qgwqevlo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ifzffzku.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ozfdxveg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nejolckp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dfhkazxh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wjofbqxq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rmckutse.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3oecpxkey.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3izgypgaz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqwsrtfc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qtxuuxin.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xkzckdor.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htrdfzuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvcxuklr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3arnxcfqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goeknbqn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xjbiphxa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dgjlkayx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tipjvroo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3begasjll.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jodgoyjo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xkoqpetn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3iyhtoprg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tqhkckqo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kymniatc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hctgbfxz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hizohyfk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tudthwck.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3esiwxugb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zuipbmhs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnwqqky.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rbgreekj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pdutigew.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pgfyztuk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dsiavpdd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vjiztdzv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fagpuxtj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hnlguwpj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ftsochfv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3soonvbnk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3edbopyrw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mndlgoxr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3clvypcig.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bokmepyb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uuyhbrge.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ryjvvzvi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ozpvcxfv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tzqljixy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pgyeream.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfetngy.html


<!-- 参考信息 -->