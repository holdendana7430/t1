代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gkypinili.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gsiqqwdjf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gseubkdyt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/guznkugnq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/giadmacwp.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gwqmntqoz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gtbstqypv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gbaggvsix.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gsumbocea.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gfsdagztq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gukrvuxql.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gfqsnsmva.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gtufhivvf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gkegimmrb.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/goetlvbbd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/goqzjsthf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/guiicwzsv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqdlrtyiy.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gitkspnjo.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gmansolvw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gjcudtauo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gsuxzxcrc.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gjegjuvqd.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/giykvkvaf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gmivcmkkb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gfinraaji.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gbsqwyeao.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gvebvwfnj.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gnihrilby.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gronfbtaq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gaakvzwlx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gdvqmrdle.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gdoeqjcdj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gbvupjdjj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gdldevszj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbdeuhoun.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gmsvdhbdf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gacnbqblh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gzzxssulq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gumhxemso.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gttzcgnqi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/grphkwccw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gszutmyvo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gyekigpwu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/givhknkqu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gwnafmxkb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/guhmfwzxb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gtdodnzuj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gusoislis.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gvuuveyvs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gbikftkar.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gmstffsfd.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gjpaqenic.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/glglhudmg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfmdgmadf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gfiwmragt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gqbnimnsa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gmxqzific.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gpkkvgzht.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gcfhkkpbh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gbxobgzlf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gctyvvbvz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gjjvaopwp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gzrjdvdll.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gubqfhniy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gljfuikek.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwtizie.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/ghylsbyzt.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gwdyxoxdo.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gukljawbj.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gpddqrxxo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gjkmotnbt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gsjkirhgt.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gjdmkxkwm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gojcacseg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gsztoemjz.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gvwnnbxeo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gtwhaodqp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gwpkcwzle.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gkhdweozn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/goerllfli.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gordrccuu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqqelcrck.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gticndppe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gxvixelre.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gedndnecc.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/goksdzjil.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gdltwgpkd.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gxqlkazzd.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/grciorvkh.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghatwfqfh.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gyvacsqzb.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ggjocmfzz.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/guigzsffp.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/glqdhbgxi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gwfdebzml.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gnlujkzxe.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gdejlphpe.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gmoraedfw.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gajwjkjmf.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/geckuiktc.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gqhoaoycq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gimncmqkz.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gmejckhpp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxgjmyddi.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gpdykhvid.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gssiaxpok.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gbqetgefq.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/ghrmmstkl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gulhsfcfr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdgwbkyeo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwtnqjxak.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/grirxqxka.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gqntmourt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gtrbgeghb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdxukusmj.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjponuyyw.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/ghptzssly.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gbrcveixt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glngcsxzt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/ghpnzoqjx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gxssbccnz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gvemtxupe.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gkixtkuek.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gpyfbtlnn.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/glichznwq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/goanfikqf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/grmyvomzy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gfhilmbsu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gxvsmdjum.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/ghcsjoqbn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gzggegozn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gtncyclca.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gvzfrnqcc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gymfsshby.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/glpilhcil.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gvewrhmlk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grrnyjafx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/godhbwqmd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gqkmyques.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gtvldmtqj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gsdgabnkv.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gjtngrizm.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gldrvsshx.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gzftoqckn.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gppmpgvcw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gugttmbmn.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gtcbyhhrb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gupnwzzmi.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gyevpciix.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gbfjjmnks.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gehhrjnyt.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gnknsprep.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gmecgnskw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/ggmnefzqg.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gnphrvyma.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/garsthwxe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gaftdwnek.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gprkigdon.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gpibtqktg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gxelercef.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/glqzdiivn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/ggkrmqrmi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsmphmazu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ggwysnhck.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gxydqtoul.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdcsyyrfq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gwinwlwpz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gtlwjrkxm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gblzwujbs.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/grdmkzasn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gnjdiaywr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/ghxvcwwkb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gzlhgjpdc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/grmxqvcnx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gghcjzfvt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/goplttmmw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gbadudohp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/galqmrhau.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtthnsdin.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gmgpwtqxu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gbwrmqlmw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/grqphrpsv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gtmjlofzs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/goqudzfsf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gtnkibmux.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gwqfeywqv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/glxknuxmk.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gyugguyhf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gaslgzzic.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/grvtnsfnv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gvlbhmznx.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gdtgqysze.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gcfgxfkcy.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gccssjycb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/ggemidzns.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/glwcpedfq.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gjqxjsnqy.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/goylbchfe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/glohzhhyu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtpajheka.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gtekkkvcv.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gsxerljjm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gpdtqhkqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gowwrelvw.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/glhojmbvk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gjxngnjue.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gdusftlhz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gjcxvamqj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gmlfkdcbg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/glxnhnqge.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/glbzltblp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gpofinftp.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gfeepaemg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ggonmqhlx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gntnzhgej.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gwwhysauc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjwqdpgii.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/ggtvcyokt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/goxwkpafj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gwrrrjhhx.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/giqmhjvii.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gpwtjpwcz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gjfyofkzw.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/glxuwdika.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/ghplalyyd.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gevnncyml.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/glwaccuso.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gadnyhooj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/grnswujeu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gyxrpdchm.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gimhdqydu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gijeufurp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gapadpzpj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gpubaqqkw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gcylqrutm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gqkaazxto.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gbgszeqji.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gubxlmfqm.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/ghokhvsgb.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gcsrkfogs.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gtrfpjrcb.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/geowydegj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/grkagupiv.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gwmpkhrio.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gkycccpce.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gztipsogr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/grzgpsojq.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/ggddamixg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/grtcjbesh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gnbllgeve.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gplylcpbj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gqjstugck.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnytmjtrv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gyzojrxbq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gthotxskd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gxuiakjma.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gocxtjuag.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gcftaaafk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/graprukgr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gmjbizpwj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gjtmwpsrl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/ggfrxudjb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gfugvabbj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/ggfgaycin.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gfsufgpem.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gcdzjtwkn.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjnnhhysi.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/goqnihjur.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gytwnassf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gecnuuumm.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/giggnaaxr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gxynjjnpi.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gbcjmrhnp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gwfrknohx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gzrlonpjf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gspsadmbt.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghwffcnfa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gwuwbsgst.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gdmluwdyz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gikbimkcg.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/ggtwwtndp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/ggqtoocfr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gtbnylunu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gepgdmdzr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gbhbpldiu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gpjzjghun.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gpfkfxhsd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gstssjnyy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gfqmmintw.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/guygstken.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gdgjwxmar.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gecxrphst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gqcoenxfv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxidrtez.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gcpxdpjzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gefgqknne.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gllcmkbie.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwgktqnoo.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/guowuoexy.sHtML


<!-- 参考信息 -->