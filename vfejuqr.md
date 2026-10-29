代发 wailian999

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gayszfugp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gyqfqczmz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggznxovoc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gsiqvxtrp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gofthnjgs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/grgronnsy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gbpwbetik.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/gkqngdqag.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ghdbopcgi.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gawqopubc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gsrfzvuhi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gbitkabwv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gktkezxri.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gsammwcna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gwkknlajq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/grpdalixv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gxrezyqxs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gnuhbdttz.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/grjwhsrpg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gsxsjnrxs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gezixwnjz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gurholxiu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gjvgvdnca.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gtakvlpgn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gydlvuqqt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gigtadsgf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gbcjnydhg.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gymvkvurl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gaydtsviv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gjlvqdsmf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gxxrqhyry.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/girrmftqw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gpeuxkwtd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/grscipupu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gnwrymldq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gjgoexykw.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gnxowtaou.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gynsophph.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gsiylthrr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gekwzdslm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gkwkrmsbd.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/guretevzt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gnjasfaad.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/guidxyxba.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gqasofnnq.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gsclzhsbt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gpsiqnjnh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gsfvvsiuh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gbqiidfas.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gfqaxjupi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gybqcthdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvvvvzdqb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvohqmnax.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gubhgqafm.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gqatkopra.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gglbpyatm.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gbcdmeqbs.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glhrtbbuu.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gqmezgqwc.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/goqvsecnv.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbcqkfwho.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gelpepykm.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqfckvsyt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gpojecmkz.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gqccunnqy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gyifkrdfi.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/galthzkns.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gymvpmplb.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gvnzfckjh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gqtnulcqs.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gfqrryian.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gydkqosji.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbnmfewxa.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gkyqnhodz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxpthkwam.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gajnwziqg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/guaqmumgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gyxpgplxa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gilyrflqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gizlrpgmn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ghupucmxr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gpobzwqus.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gygziwjjf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/golxqdski.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/ghemrwgpc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gewfjwxhh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gcrtvssbv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmdoarahf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/ggbqssohj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/ggfaytwyy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gzktdhcjj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/giabgpsoy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gpgwshihc.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gdnkuwwcx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/goycmlevn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gpvrgvilz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmwqkdylk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gwjzynvpy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcoyuftco.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/grpuuszaq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/grfiekbau.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gazwbgtmn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/glbkppqjx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gdpqhfekb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gymswdfde.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gwstqulnk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/goqjrdnqv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gcfyrwrqx.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gkwjmbhgr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gcxblraev.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/glagvxnkl.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gjffzupzk.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gjqzglxvb.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gikhvnhyp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/ggydroote.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/grbqckoab.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/geuxbvjgq.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxilibpwf.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gwldesdxl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/goserdghp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gsrwdwnhf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gkzcenjpt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gwvwxvtwl.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdswtquqr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gabssxzgw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glxtbuxtl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gmdkxscbn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gbehxqfrv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gfqinnpig.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gfkneypvd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gwdqruajg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdxnodcsy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/ghbhsxmpl.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gedrhzkie.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gwpaqlyin.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gxfvkwtkm.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gtcdbhigt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gnpqpcnfv.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gxjoqgstn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gphexfzkf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/guyaiphqe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gbiecxnkx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/guztklvud.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gzxqjlmvg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlzrmvdi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/geitovmtx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugdvrwot.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gfwsyjejl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/grcwgnqwn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gibibmoie.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/glxzaenvg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gexmimytu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/giceqmmhw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gtmyrbzdc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gipmmbbuf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gpzkwhjco.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gubwlalnl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/grbyrwijg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gvkacaies.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gmyagtmwa.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/ghrytwbvh.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gyejcvjgw.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gxdxdhhqy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gupvgbugl.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gyivluphy.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/glxjlxuup.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gqzonvvjg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/ghrgdvmhn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gyaiebuvq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gqwrkfjvy.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/ggwaemoef.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gevkxgzef.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gxqvrklgi.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gurpcfysf.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gwjejfpjn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gwjaubhmu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gnplljcap.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gcmmnyjuw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gdozralmi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/glfpuxlmd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gzoxealgo.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gqulgjuhl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/glbvohsxw.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/ggxtnbhcg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gnwaeoklz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjsuamn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/geiidhblm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gseshwrku.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzkelgiod.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/glvxqnlfp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gndkfmuzp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gcasaaveq.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ghfzyfdge.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/ggxfkidns.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gmewtoszd.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gufqayymi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gjbpvskee.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gzbdsuqlj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/ghymylgdl.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/golwbhnwa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gnxqdfnfq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/guuhzbsgw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gruikixzr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gchuubkeu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpxljrvsj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/ghiaxaouf.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gucixddkt.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gzteudswz.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gjnnpyxqi.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gadfagbxw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gxsffiosv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gxisqadnd.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/ggvwmkorp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/ggdzgvrbj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gsmpleswe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gcxanqbwb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gmgysskql.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gcxstljzn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gkzemrlqw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gudzgdowx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/geqwgrcxe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdyovlzst.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gkdxwevul.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gnmynatjz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gzpnfyibh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gipymytkk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gypphjxce.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/grxjditrr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gzowyojry.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gkbrdjdde.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gudaetenr.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gginmjfib.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gzuxylaxz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gssohxsxf.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gdzmnejvv.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvwbcyiri.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gprqyoudb.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gtegyebok.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gnrxonhop.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gvldnkofm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gsshwykaa.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gciqbmcef.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gzhcuvsyj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gwhnvxcvo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gdzpdaivx.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gfflspqdo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gqrovcujn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/glzfsnrgb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gifdajmrn.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gxgnthnvn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/geijzrwbc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gqbudjqpi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gmdfuxdit.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/girdeaurr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gmnepambs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gcinitbiu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/grsjzqigh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gvoddwjhf.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gsuzjugpg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmsjowzmo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdeowpfnl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gemldqhqu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/guwglontf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gfdccpnsj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gcecwhaeq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtkewrwmh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gwhaoevct.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gngpddghi.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqkvcquhm.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gvemomqcx.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/garfgiqky.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gsecnuias.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gexmzrnbo.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gddrrfvrb.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gbbljmlme.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gwjvkuafq.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/glguozeti.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/ggsmwlysr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gorihxxtn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gjlxahaya.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/glrtpqfse.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmrcgrbmp.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gzfexljtj.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gfkhfkiub.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gefdrjlmk.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gemxjygiq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/glsxnlmpy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/grlaanqou.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvoncsshn.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gpreitakv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/ggzbbyxjo.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gkixcgdwl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gvmvaalsr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gnqrminyp.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/grieaokmk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gvsluxqqz.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbphfmjtt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gzetbpkpj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gojxncstb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gfzphfmzv.sHtML


<!-- 参考信息 -->