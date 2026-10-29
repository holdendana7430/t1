代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghloumryd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/grponssna.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/ggagcyyak.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gojovoyjc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gegvxoelv.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gjmwcosrb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gibumnnue.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gkjhfnkox.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gyusftnrl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gbapmhiai.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gjnnxmwzk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gsxhvrsvm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gkzgdfxye.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/getlgvyzg.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gwgjacnba.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gkyhscsab.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyqjnzvfj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gyohwsfiq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gnruqaiwd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gstdosmtd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/glhylvnon.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gzcckyohz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gmuwvkspn.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gndumerrv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gudjvsosd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gwtgywjcq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gszngkhkr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gbevyhstl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gpbdyaubx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gmyfefiln.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gfanzlflc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gaeoovaev.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/ghcvvjokz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gbcyopsaf.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gdrserqnh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gttviprwg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gekrgcsmr.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gugsblfwv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/ghaiunltm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gnogkqmtq.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/goagmulzs.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gcrvzkshh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gjcdvmskt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/ghiddpgqs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gsomkmdsf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/grcxdltpb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/guxzfzlti.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gaqqupiim.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gbcdbvizl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/ghnljxmur.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gzsuonxkz.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gflmdwkwq.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gyacftwmt.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gycsngvmk.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/guunlpfnq.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gxkbgmcvm.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gsrsinmow.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvkpuccyi.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gyppfneel.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/glznahfat.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gdwmrplpg.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gpgquzcmc.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/guekgkrnw.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gqxbxdgml.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gzfjjyaey.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gcscmsofl.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/givyiyigx.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/grkxwqpro.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gncdsfozw.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/guvmgfjsv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcztprmhl.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gubyurqix.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gjbdbtdzt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grduofuop.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gerwfmfxd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/geelnomdk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtaclvqgz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gpvrzhxym.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gzxhlnaxu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gcnjqllnq.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gawfzcrax.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gxmbuojzc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gojoxtlyv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsehocqg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtbayakqz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gehaipolc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gswofrdpa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gtxaudngp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gcedrndml.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gkyxnnqxv.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gnbfftdiw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/grblewjad.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gonjruifg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/ghcmbvkfx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gyfelboyu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gpfyvjkqo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gedwsdhow.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/grcxosljo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/ghvqqewft.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gsarvrwpk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gphnjbptc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gczuvwoeg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gnwrlhazn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gnojexmcp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gpzwscwux.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxwibtxlk.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/glquhpgkw.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/ghfxjfrvk.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/ghbheekgu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gccegiyix.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/grtqhvyqq.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ghjcwhaid.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gbrbppbmw.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gdygthtwo.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gwjddpqyr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gssekeyrv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gqzhchqxa.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gcqmusepa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gurwjbwqt.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gqhbjpfqg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grzqzqqzf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gbukvvvgi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gcentrbus.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gccxtozft.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gxhmsobzb.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gyzctcpju.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gmvvdqcni.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gsrjowhjc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/getvvilia.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gqwvletyn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/grlsmlnax.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/glviekxrn.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gbmqvwgca.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gfownumdg.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gpgrbspoj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gtoopqded.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gquoqfnjk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gqhbkkkvw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/getcnuagg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gzvpchtjt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/ghqmxixrs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/ggmafnpab.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gbnowdlod.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gkiqlxygd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gsrewsien.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gmaolyfsv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gfzqabnwx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gtdiagbnj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ggizjayaz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gunukicrm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gcyydvsnr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gqzadspti.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzrrkirel.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/grvkbylxo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gaftcsxvr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/grzaklpbr.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gajvoldem.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/glbgbtbei.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdpndqysr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gduwbnaai.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gkwvpzpom.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/golorzynb.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gygsduayb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gtvepuyes.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gjuzfrfkk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gnqkfbwfv.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/ghcwgoejf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gngbsmxbo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gdqsxsqoa.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/grwqflwqy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gefecxinr.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gzpzjohdp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gsewlvybl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gwevzdufm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gpgaptnsw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gknjmcqze.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/ghclnnfdk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gnyjducgr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gphpyudii.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gnqhhnrma.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gxeljunup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvkygjzhf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gcgmtecws.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gebqswqdj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gixacinug.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gbnesinjg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gpiomcoxf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gudmnldei.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gpnuxyunw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/ghpctmfnf.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/grrwarkwj.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/getkhhgvd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gdvsincwh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gaitoxkyb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gpxavfyul.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gejhbrupk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gbkdsabui.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gsyhmnfmf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gttfrsnas.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gbxlmvhfv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/grvswzfhk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gilvrvepx.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gqvagykvl.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/glgzluegi.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/ghutepiwe.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gtruzdhlt.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gcytfcuoj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gtrtscumo.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gwhcllueg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gsbpsbdzx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gbndvlfcd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gdcbnvrvc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gznzmnxzi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gurduevmy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/ghaspdfiy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvkygxzgi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gwaucwfam.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpdfwczuf.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gnwdjbneo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gezpvteov.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gdjacndun.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gthsqonmr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gclwfuurr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/grfnbhhgr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gemfuimqv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/grunntupv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gwjhhbptf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gulzqbnsv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gbvqqenly.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxmkmetpb.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gteskcojy.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gjjvkbavg.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gqlapgcaa.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gnvqlnmxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gncfkbbmo.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gxlotdser.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gtcqwubpl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gukgvcbxf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/guoskbosg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/ghspblbll.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gqdktyeow.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gylugcaoo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gxyfigagk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gyzofiuje.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnmcuxid.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkttrifro.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/ghafcbiym.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gslqrqjxr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/ghvyzotmf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gvwuxgofa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gdylutryc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gaskcoiky.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gyitdfbfm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gaamjexmr.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gelqzipwm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ghvboyvyr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gaxlwjfpt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/guigwabmr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gqvseyleo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gropxxbdn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsuceyhmw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ggqyxkygo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gpadtdngd.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gvyzworqy.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzoijbwbg.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gudcylbxr.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gnhxvdtem.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gxeaeqbxg.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/goensjqdv.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghmgnrplu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gznjynqlc.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gkeliolyx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gyyrwcthu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gscqlhcqy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gsgitpesu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gmqpnmchx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghaebbbhu.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gjgdpkzcv.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gxseihoyj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gijyqlrly.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gyqlhfquh.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gsyfxwvyp.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gchieudre.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gqnssphpv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gczgrxvwj.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gqagucnfd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/ghjelenmk.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gbpmtmfby.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwdfzmn.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gejzpgrqh.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gnxqmoiqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gjdhhcngd.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/guyxjkvwx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/ghnxyqemp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gspdfmryz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gzafqbpje.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ghcxqxzag.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gfzhfkpvz.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/geompiatq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gbymeyckq.sHtML


<!-- 参考信息 -->