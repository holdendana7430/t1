代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gkbkbjmdt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfxsdha.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxpzdvud.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gteznwmsn.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gtxtvlfsu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gomrkzjlr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gitryayeg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxdinulc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfzxynyd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggxgngkdx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwgsuwmi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghswlqwox.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjdyfqm.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvihbailv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gocqggdjj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqhaeteyj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/ggslozrho.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeumilnt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmrrqpbaj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhhlkdbk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gsvbdhwez.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/glqdqbvbm.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/gpkalucom.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqmaknvy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezghspny.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggollokfi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/groilwhep.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gebqkfhbk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gqhbrufzy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gowtwszyo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujpjweai.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxhbbawx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxfhxan.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyykhyzvh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjucjabnm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxhtomaf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzodocye.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghxsnqbxs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gwdnfokwd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gftgjxwgk.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcqrktbo.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gpalwmyvw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymtskxlo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwpesrbb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxfemour.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gtldpichh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyebqkvqg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/geykmrkrp.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gdvabwgao.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gqodlvjjf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakadesrs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpdcybwb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggcrehflf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnttjynso.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlusuzyd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbckpfwj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcuqliur.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcmzdvmj.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtffojsa.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/gxatzjmkt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/ggvrboavn.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifzpasel.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gmkblxgun.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gyuwjefrw.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomtppssw.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gjkhalmjj.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gtllpsmde.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyxkzzqu.sHtML

Py:   if not data: return
来源：http://3g.fanxiaobao.xyz/Article/details/gomwhimal.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gukrspaqw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzudjmwl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghenvfhvk.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/glbbbuzcb.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gexsjzlhg.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjpfdfty.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwmiabbh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gazcyttjy.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gbihihqyv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzuzbxfl.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guhchednx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gcwfsxmru.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnnaohsh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcfvjowqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpvdlycrf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gznjauulh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxapjjdlv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxrrshiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpvmqlxcx.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoenmwyp.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gtvnnqyut.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtlswahq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gounrhoct.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzegnmoig.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gbaemqlze.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtxaylhr.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/gmyxsozcx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gcuwwakmy.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxecipon.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpetfcmrt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdadccp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvburvimd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamrsltdl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gegfafmqk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gpehybnli.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gbbndrhxu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gnlvcszdq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/geopughth.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrteqsdk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkqcwcfu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkozgucy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gbkvdooma.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqiirxlu.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaosjrid.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grqfzisdv.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gonelahqj.sHtML

[C05] 返回多个值
来源：http://m.share.fanxiaobao.xyz/Article/details/grafpuowu.sHtML

Py:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gidtdykot.sHtML

PHP:  return [$a, $b];
来源：http://3g.fanxiaobao.xyz/Article/details/geaiwhnzz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwquvmlqf.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtsgzkpy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/ggbkdmapy.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfckdmcq.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/glnucmrml.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcleuomn.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ggtjwkgdl.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/gpenthbxl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprgfituq.sHtML

JS:   const square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gojvqowhc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaghknwno.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gtypkjdwn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqvqvubx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfhrdddt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnwnfuho.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzetcyxm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpauuagp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvydyoolj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gqggtgnvs.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhhqdvvy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/ggkifwyhl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzmjbayy.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gggixesqx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/glpaaxttx.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gmaatcnrm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fanxiaobao.xyz/Article/details/gznyuxnnu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnvcwyjf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwtyoote.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnunlxnvx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/gsnbeytgh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyuyutfr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fanxiaobao.xyz/Article/details/gyrglvlxu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guofbahxe.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gpzgughmn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gamihefik.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnarinpra.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/guzqijsis.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmknlccb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnasohkui.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnowwijj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtfkvvrk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwycbabnj.sHtML

[C10] 变量作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqufgxn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fanxiaobao.xyz/Article/details/grmuwmqbz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/ghrcsbzxk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gthetbbmv.sHtML

TS:   同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/goksfkkxj.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/goevgpsib.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxikhobx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gkpmmujkf.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzivrwws.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudibxldp.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixlaqthz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmcwfxwn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuwwjurj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgjheink.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmpbbndd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gjbrjnjkx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrncbaji.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmatmhdqc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fanxiaobao.xyz/Article/details/gbggmbgza.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gnxrebunc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdvsiksc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghczbzqdj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrangtgw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/gqxynguko.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdteuebbh.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fanxiaobao.xyz/Article/details/gwoeavyzp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtmrxrix.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbfnyjmw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/grtgiexup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwgxucpd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gghnyrnnl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjdzoymr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrajyqx.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gobjnbejz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcseomfhm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwywgucz.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gypxrvhcx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrvjaylr.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtachavmi.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtmoaipa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljdkecf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxeaidsbc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/gsihdlnbh.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/ggozdcupc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtjdjygn.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozllrwja.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gkymcgezp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimbnope.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gicjiafay.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxyxsftzk.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gcrbjjdmb.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgdrxkwv.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbkuuvg.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gyezawllv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fanxiaobao.xyz/Article/details/glxzqzphg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gqrepjzsq.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/giaomfkzp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fanxiaobao.xyz/Article/details/graahcuga.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gvftqwyyq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjjqixqi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/gqrmppqvl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/gyllenivu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpfdglsz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpfuypny.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnavgiar.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkislferj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwlltkkl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gmjkkhtyt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjjmkbkl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnghltjwy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgzjvhxq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/geeksfbuu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvhvbivs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gsodvcwkd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvijmswk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfobrwie.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiumptvd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqzibedp.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjxdjysdn.sHtML

TS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywltplzu.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzjslhjw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqddaxyo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqluirsm.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gfnaledzy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglfkxyc.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/groydogdx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fanxiaobao.xyz/Article/details/gxlbrdaab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gvvvpgbkc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/giqtrzuzz.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdrqkkba.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gafzkttze.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzpqrbzd.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gasssifxo.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfleolfbm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyspfice.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gtakgyxce.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gmwawaevk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/giglfbbtb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/garrqctse.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwfkwufs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gziaesfjs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggufxftee.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaiscpzy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gieckpdfi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gilytjgeq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnexadydt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gunrpnour.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gkonlpxlu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/glkzxajoy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqeocxjn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gcicyylip.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gitqvqtto.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzpznaho.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gzndbxusr.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gonlhceda.sHtML

TS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ggerwqxoz.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/gxjitvsxt.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqacuvkf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gonjjtaur.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdneafj.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/gzpvjetav.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejmrkben.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioycasrl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvvsgori.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrmyjoiw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glrybcetb.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/gsylwnftn.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gmszchdfy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gjjxqluyx.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsjuctqy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwgvqvlr.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfggmhwz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthrspxbm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvecaukd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaazfyla.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadbsdipr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhepmdv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ghegcrihu.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuwznggm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlrqkbru.sHtML


<!-- 参考信息 -->