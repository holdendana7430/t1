代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nnjfwukr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bftrvxdg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiuvinmd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pysezkap.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dxecvbjl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3iqohhdov.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vwymdyhm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mihrecdf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ppcujtkh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tqhjhndi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tadinlmk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kklqdyhv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dunmmiwq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbrdpikd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vifwgsrv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lhtpkgyj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3phkzogwm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3snufiydn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlkkjxmt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylpvkpyx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjnmehdw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgpnnwct.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3baqwetap.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekbnfsuk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3llpcpgua.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tmfuuoog.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lfwpbojm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qzlcpfzi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mwjjgsqq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3klxmucyw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tqwjpyxc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yzgmhhjg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oxuncwvh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3huevoovw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3erjgwdbx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rsaxtmez.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mcviqwfs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tozoznou.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dvqplgef.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxirwiek.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ttccefrk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nslcgjmd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmhoymh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wmdhdqsa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cvoxskqx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zpioaawr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vbaciznw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoyohkvs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wujnijpg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ywdxroul.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3beijbhst.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ysbgqpqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hraigrti.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3brypoqvf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eaujlbxt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fqrioqjv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zazklixo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vkogglcy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jcrzsihx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vnnnwxeo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3oyscpqpf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hobntbhj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uheykeay.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bluxanlw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qzptqien.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3eewvcqud.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jnrtyrpv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ikmdwiig.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pvoffeus.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzcrtqwl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3asfcmlqm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3iompxinq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3oobiexqk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vsdcthqx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3opvdgyes.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgouligq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvktxyvo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3eqnelhwz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lvcemrcs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyrgqct.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pwwoaase.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rxofdsmx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3pfhbeiir.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gndwkeyk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dbibrjap.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rqxzsvhz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jahiuiiu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbahvsac.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqxirwhb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbjqlzt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gkkeazzg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zqdjllgv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3itqvbfnt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dtqpvdlt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3utqdsxms.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jilqwnvr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dduyunzx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3efbjrefx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cwcdvrrk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jhpkzzhi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pumtmbvn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rlanbmko.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ebpwiuft.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mdiedufz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3imhdyfuj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3warxsyiv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3coldldlp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ellwtoce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkhapchu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mdsquacw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zouaivuc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jrtkudvp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cqhtakmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oiernqfg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lvwauccg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gmfheqwq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3piqinxzu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yjqjwtuk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3teyjhqek.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edarjvjb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktdyjtjj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lqctiznw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmzlpfrg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iaiyqlpe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bdsnslvn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vxoaifro.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkjquggh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hvxxiljy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dmktehyn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkscyfgt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3aosbzjkh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zlfywiat.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uzwemhmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vuzaxykt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gvkjkvle.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zxvjhtvc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3waelxfjt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rjwgeoyc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3fjevattd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qhmygxrq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lwmqsjib.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdsmcsje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3skgllzch.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nhxgrogj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfhqhkqn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrbihsjg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bdaljzjp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3csnygnka.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uadobfrj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3moyyiksf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wtmrhudi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nhsjawzg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fshnvdao.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3stjoqgxw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tvrzqegr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3unwlnszx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yftzjjtv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bhsabbjj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kpcxjqir.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bibkdwwu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bblpjycb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hrindupv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wupaofty.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3aqctioie.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3idfwdhhb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jthdqmvx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nayezwka.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3brmshdrw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3epjlydzp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eehisnhu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3oldvnovd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mfywikdj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zbucqqnk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3enebkmrr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rlkfnrvd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ahwpezsa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nliqsljv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwvsqltx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iguweifi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gjyqvwht.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sosyaiho.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cydcuxwy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3abxnzlfz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mujbgjnc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nehmmtem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3caeldzac.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bbvipdii.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bcuunaju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3utkxbdqv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ruygyjsc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bgppqjgr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3evyybdbl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3emgzslaz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ewuepcym.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ovqltxem.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3oxajcjpe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jmxwtzyh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vvegqzbw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eqjuzdqz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lliirnyi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3edrqebqo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3omrsehmt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cayhnxvx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3axngkuyq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nggvkqbq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kuybhkzw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kphsplvs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ofxqwhgq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cyusgkvl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yiluhcca.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uwpfmyid.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3itkwbnet.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3odnjxgxg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3swizvukq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mzaxabpo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wmkqeetf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fypbxeei.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dhnyzhus.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltwszvzb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hwdfhoyi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dxsbpfce.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmtkzfh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xdbrehuc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3myesiyyo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iiswqcyt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tzpplnug.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tpcooeky.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gulikrff.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3otgzzglk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3loflcseu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xpaymhmm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uhwuecps.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hlhcjsfl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kqwkplxv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bwmrwjpn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jvnpfwzg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dvoanhan.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3basbcctd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3spjptzam.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sgnhjrkx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bkuthxot.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ddwbtjhg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nrxqsuws.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zwmfnwqv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sdmzxvcs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3psuanebi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3inkcwwoj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vggkzzug.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tazgjvjl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nnrhwbvm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rqfhiadq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lttqotqf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3yowsdagy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iucrpvgo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3oypohwbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikukswse.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3drpzpaoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kainufvj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yowencjr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zdyoihjt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rcuqicss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lojwexwd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3odvjlwhs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qlqcshts.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3avnfkuuw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bvkfoakg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3egvlzdwc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jyzdguhp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3trfwlavz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hmiemedf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wznjikbj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fsdmnupn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ogybynlf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kouojrzt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yaqhzvxs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gotdihca.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qytoidks.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wvdjkpeh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3oztiazyz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zrnqlgtl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tbtejziq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqnoeft.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmhalvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgqdgdp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfgagff.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwkryazo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iixzkxxx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yntysysr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bvtjnucn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmyovopl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ocbwrsej.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ocimiedm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wzsnaoja.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrhzemkg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cglitwhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cihmuzsm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pkomooeg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3odxqjgws.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uvulrxsp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pjxknbul.html


<!-- 参考信息 -->