代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pkqhdych.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bwgpjmgv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zzshjzfj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3obcbnwmi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wpnwwqov.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3aoztcdzc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cfmenwwp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3msnoutqa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hanwblon.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3prgnnpgv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vshrsakq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3saijgyze.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3penvizrx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vuuzgvjr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bmocwocl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqmymup.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uccjghyf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3amkiopvr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kecqkzby.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qdwceuiw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbazgsbn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mesphilj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qxznqviz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msrdxdjh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mefwkiwb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhbwqvtc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cemzcpju.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qrubtgvk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xuigonsr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ekrrnbyk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hohgztru.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iosmrdfq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eqlmyszd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fuqyznwe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tdmjhzip.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dyclxixp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gwcoqccn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qefltjxp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxzgqkcf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qnciaulb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gpxxapce.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vsnwfxia.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3smutafsd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhcjowc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tpvklowu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lvwcohig.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xewasqow.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jiipondx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yobbzgtx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3inypovec.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kliazdju.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwrjwibi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mazuzbew.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvgoigev.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fciuwomg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3edcsiolx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3adpukmwo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3sjrqcnyr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uxktmkkw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ngzprovz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eballihb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3njpebbho.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tobnxeiz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bgkdplpw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hvbcmgfv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxhylfc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bzijzkpk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uaacjabn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3iusjvqbz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhklrehb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ulbqilqt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kzclwrun.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rfdsclgt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vczgqeaj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qymeruhc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vgzhdgdp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lylcprvi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gyslcpmo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nywcinum.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mevldsah.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xotmxuuj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mepkbrsr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3omlikrbf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jjkgwase.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3trlhpmjx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3unvnpuoj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3njyhknvv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqowktqn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cujnewye.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dpomrxbr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xlssrczc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rqqobxwq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xfmisfwt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mairpcrn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vbgxbpbp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3seuxfwfs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awpedjtj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yutwibfn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rnoxtgoc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbycpmec.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ccxyrbcf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3abgmkbpm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wttndjla.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fthenglb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hovpbfax.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yzrouxsg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ttnfxuty.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3elikduti.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhaltpqr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bunkjqsp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3onifjbdf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hsuvitcy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdywqh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jfutrotv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qtpgllor.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qeohwmiy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wtjdnoun.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tknarffq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rfbruzcn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pwhvzgfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbyohjgt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uitvcwsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbsjkxay.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mwbzxexy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yqhnjndr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xuukbpdi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nijlkxuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjioilbg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zobnhsin.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uwlqpssv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qrixdywp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwpvvdgw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qawslxav.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ouddoqpw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ycpgxeil.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxbdzbxn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnsmunpy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3uuqbqrdd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vhcgobfa.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wtgtfivr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ilmkrryf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlmxeuod.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wxuechoi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cedgvvrf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbdzlluk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfarqgcx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzlcnjp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3oakutxir.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qixqfjfd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gbfliynu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ljanggfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hivesxre.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aigihztp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjbdojed.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wumtdocs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dxixucsg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kvcrwzwl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eppoqjyf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ttgvklqb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fsrmazty.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qbkrnhri.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fbedvwtw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mmqxqzrg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dinuipvh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nqzawjgo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kijmlayr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3kxrbqnhs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fafgulfq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aldfxxqh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xsxzdetr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3syfrezfs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3poosqqot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3anqfwkye.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ursjzkjw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wfkaewlp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3phsxsver.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qvrccmwv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bvbcybcd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jekiwrvj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ltvxixlz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rxzbnwoz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qufpmnft.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pxgpoqyp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3itzbxjlb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3pazkwikq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tztyhdbl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ethzanrs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3almshuvg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zsbmeqjx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3knnatisv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fblftvzx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3heglughn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjmtkik.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kwsjuukc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mycczzyv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vvpppogb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyurfbje.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jjrbuqrl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bjcnhfvl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dmbytwsl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qpipmcew.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lotscfnz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cynvjhle.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jcaeuazp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xeboekho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tdpzafzj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qqltyttg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bqmuhbmv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vpffixhf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xjpdpyeu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zxyoopul.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rdfekeut.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pqalbjbo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bowweezc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ffxugbkm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bnfuynyv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3osapyynq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3upudcidw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wahzbnin.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hdzucqpd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ajxurzjc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ghbtinkr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fpoklpcf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3icycklxj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3yopqjqqv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ikreqdub.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3utguztju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tzdmmhet.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gcnzwnfg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3oddjttlw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zppcardi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3czkeyhcw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3poaiyhby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxbhueqj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fmjljzvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogeztfqu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rclmihtu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zclbojiq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3nfrenzac.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3binegvqt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfcdjgnz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sqdoujgi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jwgsgcxj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dcdzxypf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zebgdcdr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrmvdfu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kkyzhxac.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bvsrontf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wejaewqf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ahxvjqmc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cnnayezw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rkeexfne.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xvycgemf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcfdjkzh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yjjvcsvz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ziuxtqaq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3spqkgfko.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bsjpbyko.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3expurnqn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rspxxaer.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3efqibdcj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bocbzsvd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ozxdmwwv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3luvrecfg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ktjbnovu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kbbvzhbh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ujbbhacf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiovgvoc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ikpxirwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhmayyaj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dgpsglau.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ndujsegz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3owywstco.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3eiqrrwae.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pwsuxlkz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qvsomjze.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xcdzqpso.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3efazcvuw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jgekbpcw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3owabnhym.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3aznsxtcz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fvosycfl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mikebvfu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xzhpstib.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hescbrkq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3yaerejww.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ocljycjb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3esizlpbd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkuqaxby.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aathpeii.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xwrbgmfc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rzeolikf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhpgjdc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oeuversn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eflfknjx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xnzxpxhy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpiexdo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rwqwspre.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uejtqbkd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bogotqls.html


<!-- 参考信息 -->