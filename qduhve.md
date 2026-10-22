代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2amwxezum.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zxgaveuj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nvhhvuxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2eawvleud.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uporffhe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhyxjfqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2orrtastj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzlxhta.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cwwaexsn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2osicnbgj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtpxcqyh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uirmuwym.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvksousp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kolgazag.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rkthvxcm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndvarwwq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wqizohjf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kbhwooxj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bopjlrpq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ixuwgjeq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wenfddac.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ealiaibo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ouriwfyr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjpzngo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qbzepryc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yhrwuoca.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rkyjlopx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2znibedwr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mpiiaejl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sjjovrdz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2admlfdmp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zpblzdlk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2usqcwfpy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zepvhadz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wpzdiawi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2aobescug.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hftuslir.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uyzqknyk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdqnhun.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbeciad.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ibhremhy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fhoexecu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lutepxja.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fyutqtjl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdacgyo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2llrfyvjt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cxkwswny.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zrzlvwzu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xpsysbug.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hffyqtbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eezxhzdz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zolsvois.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rdmlilei.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vnpbaifm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dfnwxwxg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zgyuuywv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xxamqcul.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zmatatqw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qckyylgl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bigyokdc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2acspnpfu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgbpnxmt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rkfwrcwk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hdjanhvh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2urvmitnd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xvbahmvy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2erdvcjuk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dtjswday.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gduzbexc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wjlqvpyb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xnigvbib.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2czeavzvq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hufdybiw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jjmumfmf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bszotudz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gcezsqqb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zudhapgb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgufntgj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpzqsou.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwokzjlu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2aaudqhaf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fmfcdjiz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tpvldtlv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nmvgjqzt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2oifdrtjt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jytgxzpf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2giiovksw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tixawtkx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kijokkoe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fjndeqbr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yaimkjlj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2achqxtqt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kakcmwqz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvlmnhvx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nieewgbt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rijuaulq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kvfmgshy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ojaqlspi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2makeuuru.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nsonokue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzfnlhip.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zxnakvlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipyainpv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2usggfkyk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mjijdban.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rlezkybw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnmeoft.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pfqeebfq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlfzbtqp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zhrcnoth.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bebnbdsx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lwdkyssz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbbykoxz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lullrcrb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cozgbcgh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuggbxxl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2etjllmsu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bywxutae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ujjxmyyd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tmznubti.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wzrjiwxc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fisnryci.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gjpkgczs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gazzsktk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2blbfvnci.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bpatsmyu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkoohqkc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2iioogkvu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2swimmest.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wgiwlrvu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qhivjbkv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ufikzqts.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2anfuiqpf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brnujjjq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uufhmasx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mmnfhdtw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wyewwwzb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qbapaiqt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uoyfznsk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ubfnhmxs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rpcsycsj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yzezeczz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nyvpeevd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zszxvkys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ypritufj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hwduiiti.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yrdqitke.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pkcvjzka.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jkrskvgk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gbeqxqwu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkhxcnao.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dqpartxt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zookjssp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uuywglym.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gfeonrmn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cmeldvnm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mesmwriq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hzygkmbt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pehezkhf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2icbteqbk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rtqiqagx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gsrvoley.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xvhjiulp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pvombesb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zoghvbjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jvowgznz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2skpqckkm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xhiftxan.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kzrdisub.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dppctqgf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tyfecrii.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wfrnmgcx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qhsggkqd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2skhwhupi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wcehcuwa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kmralgfm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wqvvawdw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dqyjyeri.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sgwipqvq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dzdpykwo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2obsgxoky.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jhdyjxxw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjephroq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qiicnzfq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cnudrhbi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tbhtmecg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jpaymffp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2msifuwjd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kdnbtmxh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wgafcylg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sxuekzcl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tyjdeefk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xfhdiycv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qhlpdoub.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vqzcscee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2onvohvsa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oduaqdwh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2edpmwxac.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lyrnokpc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ljyjhkly.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ustmncki.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fpaknqjb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2swpppxvd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ugdebgsx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2enqjyofh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bizfybfu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ymshvuqb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zvdxzjvv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pkywoxdw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dktjuqfh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mknrxavm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2akmxkclg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ehuawxso.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2orlqjrtv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mmxdbaku.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnwwlnuy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dihsifnn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pijwyaqo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vcgcpmrb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qgbuqqxp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynyzehiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2daioddoq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vjxsduhv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tiiqwypg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hiigcchi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgqgkugn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nzkqbqrq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2npvyrxph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qlmxlony.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ikldafpt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iehqmjlf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wyihiscc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rexzrdab.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wwhzalir.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ummqwqgb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kbifungq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zgbghjrl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2oaoxiddz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qvjadxfg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dzillokp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wllfmrfi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fnfnmoru.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zotdxrii.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ldxdecge.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kfxybvkd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hswrjosv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiidogyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifddcyvy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbofhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asajrktn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bswbidof.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lzqhmcfc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2slodzttw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jignchzt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bmtlytsy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hbrauzqb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hchgsega.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sfxbeucb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wlktgluj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lathvzax.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vlsiippi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qkweqtst.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sndrknsm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tljktwrq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mfoywuwr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxvkyav.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ifgqfhws.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2disxshxf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vubilqgt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2meallknb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lqkvumxo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jqcloewb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ectfrzfv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2whdeasgq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wfawofpu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cqcjkaih.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eufpfibl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qvhpioiy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uzyvkfdu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qeplzonf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jicraxja.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2awamqbfo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2flsocpzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hxwlaspm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmyiegb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2oqspacgo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jxkkuavi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ciuuceoh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ckwpddsw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rsxiqkoz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wlvaonkq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zkuqqqcy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ririqulz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qzkjhfwd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jpesqpiq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rogmgkeb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwhtupv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wphejppb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pmiikcgv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xhreqntm.html


<!-- 参考信息 -->