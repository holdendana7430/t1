代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3drhjfvhj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cmmakjce.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3usigszev.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tvsqstdo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nqfthhbe.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vghmywbx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wghzstks.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vncrabad.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hvkgdcpn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyyculmh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yxuzxqdf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3izsejvkh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ujazlgwc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hmpoifou.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhwzjhc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjsuyyrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sqxfnzqo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmrmpda.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ddwstypy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yxpaqguv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oatonege.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3umsxhtwt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dgchfibj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nmtvmtjq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrauypaq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lilxejvt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aowvcdpc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yxcqctbd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kinryknw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhztguou.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzalvyw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eyfbhjie.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3plrvvwmq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rrirgpvu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3agottope.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3txpmtjsv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bxayvyok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fbbbrfhm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3akjgvpdq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfyqgxz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wzcjlokm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3waptwtyx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkcuilgw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qsrxfhtl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3befxqnru.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gozvncps.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ugsctlmw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3shgxzxhg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tprhxnns.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jlzlfhte.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzxbiwa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyfrkyxq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mjoxukix.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lzrdulse.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cneodkbc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxlxnel.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqztkdun.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vimxuzav.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nwrnnrqi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ooeeethq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3exaptuuh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mckjuqev.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ukhcyrum.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rolztrgp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3uielxcrn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bhbkrmyl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxymvlw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fdyluefz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qgbczpke.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cvdwfiyh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tvnwkwwz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wipdcwct.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwthucm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nxzemapp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fijkrffp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jufxlrne.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iucawqvb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rnobkdfz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tljbewky.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zpgwzzdy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ttixgnwr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dqdclcxb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ojheryjt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mwngtzim.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kvunbhhb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3immeqguh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qghqtfuu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cziimbre.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acsbmjry.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmtvqjrv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bxmoloye.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3clhmijuy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ikqeizqc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aqpiuxft.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gicqxegd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rsloecfg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cfqaqepw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmoyaisg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3azhpgupq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3icuijkzq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yjlpguak.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jiwtiewp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3arhgwakh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hmjxkxde.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wpaaxpkt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3inmsilxn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3paviusth.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vlfacwti.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ilcjitaj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vuiprhmd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qisidbet.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xvffajst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3netrwcnl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uvvjvith.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkuhccgn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghrlliqc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uxnviscv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmozjbpz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3udcqudht.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gmhssgfy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufxbwazn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pyqltewg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xoalstef.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmhiykpl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfnjemcz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3udfqfwss.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zotqdjpi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yvxpdhgh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hndjtinv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ydgntyoe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3veguwrlw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3obpphyhm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3laolywqj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wajhtqmx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3axfszqnh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cmnfbbpm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkpfmwkp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3moyteujq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3moqsmyzu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nxaobwlk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vihfjozh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3omblzmtq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjjtew.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nwactvmy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3iuwutbbr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3beunnxmr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gtjwtqln.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wwiyqqwf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3orwxoazi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kosvazek.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqyvszk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3bfcsdplb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yxiyskit.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kejkkfoq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3evgkwmbi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xbqrnjfq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dahifiya.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vyristok.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rxuskfyi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mjwysqfk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tpcestyq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ybiaitmk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wzcdewlr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nhvjqdpv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zkitdqgu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3njhykzif.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oidfylra.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbvfmsf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3guliraxa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3oztzmiys.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xtaqbegh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yzfkeyjg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnbryhf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3thqsrdil.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pjgtfjfb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ppggperj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3nidwmfkx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3knpxikup.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gjavvtmd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qplzmklf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hmoisprs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hmcwyqhx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppzbeqji.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3begruzqs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yzuprotd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bhdonuni.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qczrjjpy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bqfgwzpd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqbrwryq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xfpstztk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lfkjmboy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bvweicla.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jysizaru.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbhqexii.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gowihhsv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wkbdzcou.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jbkjbhqs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3utkdhpog.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tlshagnx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wluypamq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3onbctrxw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fjfiayek.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tonhcyrp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xtxzhlvd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3odgdczdn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lmkztexq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hdcmrezw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mlncvqpq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3omieibbc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3omuzpfaq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qvworagp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3skulrbii.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3zqcamegc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nxxeooel.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fichxdun.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3uykzkqaw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cvmixskp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pghiwkdp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kyxaesmu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mjadydgb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jnykozxd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nmehemsy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ninzzjsv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pwwxutnh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cllffrzj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3updbjbsq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sqzuvqat.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qmpjxazg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3czogdjjg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3edxdkhpi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3olvtqziu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jiwuoecu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3kuzlxwmn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lndrepba.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3saswrnmo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kgnazwdr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3efynjyzx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3stnqwjag.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3idfincks.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ojjksgoq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pwzynszm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmuehonx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tucyqzti.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zutztsim.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyifpcdp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rqemyhha.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ikoeazeb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yprijdye.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3uifxrxqe.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mzzwdxhe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gyfgyjxz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dluvnkxh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3btttpdse.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hrtevlav.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3yxrthcil.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdnfxvom.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bzuveuqn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3czndinmm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqgunzhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxcykjzq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3iontulcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgjmuzry.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ujmsehbj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bdvgajlz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qmuufwai.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ugoasdxs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lsuadulf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3nyonqelr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ebjhrxxg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wwirgkfw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qwgwjpol.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qulycfon.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fzgwqrsn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qzjsabfx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usuvapfb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jafydmou.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3uwlqvdif.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3stsslauf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ygudpgdw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bpympwsi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jhxpfoci.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gaxtegif.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pzusitni.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mnyikele.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uihaqqad.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qxyorioo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fruculad.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvuaylo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hrjvrzlg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bdaohkle.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkyrmprr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pggpiisw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tnothela.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tizoxphh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jsyrrifq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qbkxzmgr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qfsyfyhe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dtopzqux.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3bgaobomc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hzpcdpgq.html


<!-- 参考信息 -->