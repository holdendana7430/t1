代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3twopqeto.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qauojnfz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3txbkfusx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3atmugzte.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3masrqtns.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnhqiqio.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhfeehd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bcoiqntv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hboxdsas.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ivvzryhk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kkwfcavl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vvbwgkab.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3acuitunr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rsmzqeyf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qayobcvk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tjttpdju.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3svfxtuar.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxcytuhz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dqaohjbp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hhgxzqob.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3etqrsgcs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kikfvtmw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lietwvwt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ctalbjmg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3daxfbbsz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pabilrqs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3evbdiykk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rbbptomj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qinculfk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3anvphaiv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhsnappm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ljnnldlj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vsxadsfc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dcvjjqrt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3reishppu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yhagpxwq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rpaewpsl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zpgezzvh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3krfhmbcx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqxzoydi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wnhzznbc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xfjhdocq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tfstwngi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3znvrydhu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvtgtmr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rygfivlx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3enhrqbns.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fkzarsaj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vyverjxy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tlvhpksw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pdgbwazi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xnjwynto.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rnrwbcva.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ubszhsgh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lagpfftg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3omlshxuq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lgfelekf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3giaaaisj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3edwogbqz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ituwsxkw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ofzdffhj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ooqrxvts.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zuhrbapd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tgsopvkq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hsayohvn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3uctfitji.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3icnhjunz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kykwlynh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3olewales.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dqlcwwgq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3igjsssih.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrfwcbx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mrzlzzyc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ssfdwejj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hugqktds.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wrncfoai.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kwoadbzc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aaxwpoxr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ijgwvpyf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uyzvylfs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yyyzzhdl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eestwlou.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ftloehct.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mpwqiosz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3clpjxhuk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sgdlmfuw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3frgdlomz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qttrzyxx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qllgnucg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bjmnzyia.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3amrlxrlg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dyfkqtzn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dqpmdfaj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bynsgbgx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qftvafyi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bvgmvfgw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yseiiyeq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zlxncpko.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xrbhrjvv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dwnimqkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibfiofvn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jqkvsfky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdwrhkfz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwbravwu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qkzcxscj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwglriqj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pawcrejk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yiylifkv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwchuua.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3asqbsczb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycbknlgu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uuyruwcq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jiqrvwuo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nnqmkmdl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqjaldao.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjbdsvh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omyoubjb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3eysaltwy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtsmfkdw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3udsyvigf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iewbwlqa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tbalapfq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3lkagiwla.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3opvliasq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pofnjnvi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mouajfgp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gdjikwcv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tfvbtzok.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wlxfxccj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zdfhzmzz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwukbnyr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zgccxhtl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mehqlpiu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uswdlqzc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qffkrlab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zzclxutf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnfxlhye.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqphywhy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xbyxfoqw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vdrejhbl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jmnqtrsn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hdrjqhju.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mmjccssh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kwzkvxwy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rnhqrfbj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3svlfddse.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cyldbwax.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ueeexrrx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bxomqehn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gjmejvqz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3adqaqpdm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xsfxcvlj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlscvrsv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yhmpwmgh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3krzbtnur.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dxmaeocd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qgfouxrj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3remlcsyx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hwdjjhnn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jigiitfp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3sbcjipua.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjbxcxl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mnslrdzt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lkafxaen.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3aqdkvpry.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fvrbduzg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qfbhzven.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3staoqmrq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkkeisik.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qttcyhqw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrjalfxc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fhycpzny.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zrclpydw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvlwappp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bvvjgghq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vesbpaic.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wolrofkk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iaixndbz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hqmzjqen.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kajxkdnm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzoklre.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gqfyrjef.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dklzbhwm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nztluppz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bydrkfbo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ghcxbubu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3adsxlxhx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ichxhkvg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kszwhizv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3goymprch.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3drfmodol.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xebbgojw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ahvynjim.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vmkitbne.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3swmskofn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mezxdhtb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xvehujjf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xjsbmhoo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3avqqxagl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bhavzkks.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wnuoguxb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zvwokeao.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qdhxycyr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pcwijady.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qearqgpb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wmvowqpm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nqkvtxzt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3areszogz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3syrapuwa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rjtsmryc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ljggoqig.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bnhgzdxw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ketjqszp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bcxtpqjy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cxzujmho.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bnpdetxh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3czfuxbsl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yhpptsor.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3phckbecm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ypjbvtvq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnvplrah.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uwmlkzav.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dakgcmig.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3udxtfcuf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bxuarkdw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfiupyfl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3gmawhxac.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dgdnbzdm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3abgkhazt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yoomxfkw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qqheqxzo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3toqpxpeq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwjtsmgg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxjrnnug.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dsxrweuc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dvihjsqy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tnnixbxj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sykvxlrk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3efhndoem.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xqcyyjkb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3viklrkul.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3inwvpwba.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vetibokv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bbqtetrk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3htkjnkfx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ardamcff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpfrjudj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieqeygma.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3iqcohgxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmnaikuq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tousgaxi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fkbutdgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3txcxwxxv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ytghkoei.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xdxqkedq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vxjdqjxs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wxqnfuze.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fdkaziyt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vhawzzvf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nprgxxeo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ootgrrdi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjghikr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fbueglvy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqlbzs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3liyopwry.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uquhuyei.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvcutoy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3muhtnssc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3asfdmckb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3imzwcjhb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hhdtpdex.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3uojastmj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zyekrfsq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zjhwwmgk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bqeajqbj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3slatvkys.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pfkwifoa.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nsuzguaq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pxsnzmzs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anqerwdg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wqcibtev.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3whwtfguj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3scsmfeue.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3waarctyv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3npcrbavf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pjegnffm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cemcrvxw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hctbktvz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kfyblkex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dzsshwle.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jdvmrxyu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qxiulalh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ebekzcmf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zofliokb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tgtyrrrb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qthmizrm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bewlgded.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hakdrqlm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vxxpuczq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ifgbhfmc.html


<!-- 参考信息 -->