代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gprezftl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fbfchcpi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jzooimtm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pmaaoddi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dywopxey.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uvtjczpd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lrbfdalv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3joppfnvr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kznlechv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pnaqhwvf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wdjmfcpp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qyhuxsgm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rwqgnzub.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3khypvzvl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cxioumfw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3thvrzpnd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wamzxuoc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3myeajzbt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dzhotkum.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vkidjqgw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dlxexjwp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pdvhlfwy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrokmqe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3knxaaglc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gfbhhlwf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ecltsapw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gtjpxpmx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3irkioevo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nhrjtadj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3befgiaye.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qnkpwlav.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wllqfgfv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvlvatru.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bppxdkwx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zfptgohx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkwpznp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3takomaci.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vqflpxts.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vyoosatc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vrihbkoq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xohwlcvx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3egwqvfcu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrjfdbqp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lskskojk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3viblwhxa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhclrfzg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3meazkhem.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3adwazome.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jtmcglnp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3daegfpcd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oraiuctj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ewtvmddf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jkmallnr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zugqgfbj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hgosqnmq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xlechbqz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rkeoqmsc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ybudwmyo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xcftkrce.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wlxhopib.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrvuknae.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkysvret.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3aszclxjw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jxnnocoi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bwtwitdh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vktfuyds.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjaaubn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dtygopai.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zphxcnqq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3clsgvtst.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nlcdwnqa.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3iqlheegy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mfvpsjze.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dcivqcvx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jjlxusdr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lqfflkda.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dsxvtxzq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kqvdwujy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zjlyfpuy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3naelylep.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tkyemxaz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ujeqgjxv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uidzmpos.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yytrttfa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3oqwtdkmd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rjqoztza.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3auhomczr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ihlhizvu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ifzpqjhd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cbeyuhfo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3stkbppsd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vonegcdf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kfeqrwdi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eexugobk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3raoiqtzg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gjajgosd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3woutunkm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3muzhzfpf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3npkywunw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ypvawtup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdhhyicf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dyoyxcuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glcfwmsq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycorrpac.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mruadlgr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oeppqsjm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jaceipdt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mpxarucv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jkxxjrvu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3etavaadv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbmiaorm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lbkfndkm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3prqtbqkv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lznmboow.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cywptheh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyppcqlm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ykgdouff.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kdwqxqsi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3shcfkldb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nrqcctaq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hwgorypp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3iakkbukx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xubkxhsj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xsfhluqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqplmyh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3raosrxcc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vevpyftb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lhajmwrj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tewrfpga.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3drwujyjq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3czzlivhh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3samxjzdj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ginsrhaj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghhyvlgc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nafgwpbw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zhfygyxj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gwihqbgn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfltsuyj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lugrckza.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sxuqwadj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xchcsckp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mzlchsuq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cvbymmmb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zrdisppc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3frrtqfbg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3peovjeqk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qrdhygud.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3plrcxmyo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3srdbdjzb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cfjkrune.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3guaihkfn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqacvaq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ydhvgnkd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nmmccrqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3duwddzbz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3inbehkss.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uzdhkdjb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hqmuqaay.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3otuaahtv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qvfchcwp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwonmda.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hcnfhtmp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dzndwtfg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mhscqfhz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kbpkdgug.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bezdzash.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wybaazzs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kgmlzjoj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhxrvdzg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfgfobm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xgdxjdus.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lyypkkia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3oxmjwnfu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xclplduc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsdbbgid.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lxwxjqud.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pbbxagco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwooslpc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zwdjpdbx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3smvrikon.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bkuzewrh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3foucxxwu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvbfhqz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eyyiwora.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3anedrbhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3heftpztj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xqprorej.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gieeqzbi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vopxkuvn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rhzfdrof.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iqrkjjqf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mcbizegd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qsopmyjo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cumzaorm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zuqbhljb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3widiuhpu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nugiwrqg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fpqrkbdj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3icyczaqa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rbxberdt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wyqnrgjj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ojocpslr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tuxvqfsy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3doyfezck.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ciokjcpv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jwemoajv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ckqeylhg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qctvtqjy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3aydrowrg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3frzmirrp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qavzdxqe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ccxxmzug.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tdytttim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sotplkap.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vbpnnvyk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxuzxmqb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbushdl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oxaejibt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pbbdczmt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jprzerwe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dstufhlv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3elqmnzvr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eodlwggz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lcjkizoa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kimrebtv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3euwckoet.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3czolqpvd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wspgmmyu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wfqhztje.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3srswdslb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3utmburah.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hujmsxlc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nefklxtl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcgfpqvy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bgebscgc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3noqcnueu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3bsyzxcws.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fbunkmeg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jglljdyu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dfvtijjb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jhuilbnm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zfajavip.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wqqpidze.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kxiwfwtv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vzkyyhbg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojdpdejn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voriudtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cahiguhl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xsllmkpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiyjpfwy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3exwrrpox.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wfrkkchi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nrpibsrt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hlgiwljo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yivwjwwi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sdigsjwk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qxupneqo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uzkuxwli.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nokggqxj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3gdyzorgj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mkojoriu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mspbqdcq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxpfjw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yghgwtzf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ecdblfkx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdwiskl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ugifaaye.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3taszeuzv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ouyajlmn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3viqawdfj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3poslatev.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3okaxkqhy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aeufjrmv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wioibpwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwyppht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pnzkdjpf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ttwfmolq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkzuthxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3eamsjufb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lkvcfyvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ltvtnzsg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3obwuugbs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bfxjmpxx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3exqgxtjo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3utvslnic.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cubwnyoo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wrvbjelj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ofgyvkli.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rjykgfpt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qzwqqtcp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3rusdofus.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bjbqcptk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bncxiqpr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wlttrijt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qdgtjoot.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mnqxgger.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3svgxsadq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzkdoucn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mxwolfml.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ozqqehxy.html


<!-- 参考信息 -->