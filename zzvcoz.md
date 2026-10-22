代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xenonryy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lkokysqi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2iudkltfx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vkqtloot.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbbyzcgo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2osuztifx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cdytpuym.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rhlfsxol.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pgfeojrw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvnnedr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyuazkzb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpypwm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xryiiuex.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aucdnotm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qedgcgzw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qchexhld.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vrroozvy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2munxfmts.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2awlibdav.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zsenkbiy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gmkjfdwb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bpwxmnrl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ecapzucb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rmphlglk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yhsphycv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vbrcrfrc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kkldhfnv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wcnsdsbc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nhswdufw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtwhguqe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpjmdaum.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdfreqho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aguuzyec.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2msnbtsrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwoumpi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ryqbzvsu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hohlrnhu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2smhtwpag.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2njesnpuv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrohunmj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gxzwholi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2smyqgdhi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnzvysds.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gntrfhla.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlehewx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mhwtnsyu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mrlfsidj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zfxmybsw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ikwfinwl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ozulcivt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cpnshqdw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ausmgjrt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fbvhdich.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2towgzlxf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkkqnvb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2amzduyqj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gscgivtc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mwrmvfjg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xosjkvhd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mngkuiyq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hbrizttu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kygnjtjn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vecofzwz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dvmuyzqd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2oxwonsbt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ifjyjuvj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwosrpi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cdbmkjph.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqsfxew.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mybgoyux.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xdsdhvtv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uiyilqfm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zkxklcun.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2goajbthx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dghzidwn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdknkts.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vfnjbcsa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osdljwzf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdstdldn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ofgmlhqx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ssipqakz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pfgfjvwk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2whhgscwb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wiwhysan.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ftrqkmsi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hhenqcbd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rnrarpwt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mldrtiye.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2scleytzw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2raplpber.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2okyvdjmd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2blxeojvk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yfesokno.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2beoeqiei.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gettarox.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pdbmovmu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aqiuovil.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jltdvout.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mxvcyeer.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mmqfuvtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2higcggzi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hoayxrzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2serrptjv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqharhgi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2chpnuled.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2exjftolf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fwbjebqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bufakfyy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vmjqisyi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nghpvuyx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dbotkhmu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2erctxtvu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yhjhuszz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2znuzlbwd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2enohqxzi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzpuopv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxzgcpk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kdpvrbzq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uunzwkdf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vlmymunb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cqzfsdmi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkvitgct.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hwflfzwd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2stdjzkba.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gntofsqy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ahgjescc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jdluolhh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cujzsubj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wvankmjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wxwjzhmd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jhavzgbw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2quxbqqfz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfpmdvnj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2brrwmevx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2chodcgdj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ieekyxve.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2raotrpgg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jnzxxqei.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2elhbilvq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rgiynvvr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qzpdggkh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oiczibaa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cpgnhpum.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2caaepgtl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cyyuoxsm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2exrdpldc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mnaysqqu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xvjreelt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gewiajke.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bobxarrv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2psgifbge.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xoguobuc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fwujunka.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2quxqtymw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rrnvynzo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ryrkxbze.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hlfgjumm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2icbkzegu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2oicjvzds.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2odjtrtjp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtqmqqq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2uwuspccd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2aesoochi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2giszofxg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jdaokdrr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tanjiqdf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ulptcxrg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tsostlwj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ihsqkiff.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bmckmymz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbibjrvn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2okqewfwz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dydqoqto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfpcyxub.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulezleoj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2omiqzwne.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esujgzfi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2egyididp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yodonnlt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zqvmlate.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyoqnjpb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nywqfezf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ygaiuytd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pubpmvrp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ttujfiqr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kylztwsx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pyndcljt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pkxmkink.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qpyeudrm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cyonrayr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kcpzzpbt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sqaeqhbs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bstrvvao.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ntjxebev.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vyvonaui.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yfcywqur.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ryqjpclj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ydwuilwp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bwfcpxox.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2syxskqar.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rhjsowld.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xfkpxdse.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2evcywgqf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uxhlhdhf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ibpraair.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qixngbng.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jfwxgkpk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gxniqipl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fmljcajy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kezoxjub.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlioaafs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vohlrmqg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2donhfabt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ujstatal.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xnbelnos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tyxyiaar.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2riqavuya.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ezhzjopc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rvgxwcwq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2umtcwfdd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvikcflv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yaxdxoed.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jmvlcbnr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eevxsamb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rovugryf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vkcggdmv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2niktmqdu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ciyipxha.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2swxteztx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tizsbjqy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nkteuomr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nnlogjqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jidvtmha.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zngjdxrk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sevqwfgg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ftabdajq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zpcifmgx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kdxswtxk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2deuvsepv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ebjmlauu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hnoeyifo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ufulhbzz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qqadoqur.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lohtncxq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qcskvwjf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kgggecec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nuqduljb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njdkzteg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sljmwfiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esgslzzh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vgpgwjeh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2acvihetl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oecwcqts.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pahvfiog.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ultfhzha.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uknvqdnk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wwwfktwr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cihnjuqs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wacupmyg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hlkknyww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2exabtpbd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hqwlxmup.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nmknoffj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vbfbutbw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2phbbgjbv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wxcedhdt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xnenhtlu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hvazmtls.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2odlpyvrz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuvqobo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtfxanvo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zxabyxyd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2thluebil.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qtpkbrgm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2omdejfti.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzmcciu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yswbrbxt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2adgsffta.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uquuqiio.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jichhplp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2aqgadrya.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xcvznmoq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ztytotas.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vfyxnply.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jtqzdili.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tblulwae.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bkazdavj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2awdvrisv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bzcxsksr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xgvtqmxc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mnwmueto.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xhqgorjv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lnkisyac.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ztdprkub.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ulwmclnd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qvdmqomh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrprmiut.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svwcymlv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gaqvpqvh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lnskypgw.html


<!-- 参考信息 -->