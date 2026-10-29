代发 wailian999

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gundizxig.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gxjjpynqi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gokutvype.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gowvndtke.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gwcxxwgec.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyqwovvne.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/ggsbndkrn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/glrujzgxl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gdqueugqo.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/ghvgxvdrv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/girxmejei.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkeqcawwl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gcpeqiwfi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gilveykrg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/giodrvlmh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/ggnnzdqkn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/ggucnilvc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gpxdbqnxg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gmxjvjdxc.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gkjeujjop.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gydkmqsjt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gvxfqgbes.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gemgaibik.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gjscwjazz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gpcjubnxy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/ggqbecmni.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gysrhabtd.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gpdvavbyy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gsmvkjwof.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gjfubmyyj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gvpaagpeu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxfstxkdv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/guhfzahbx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gajotuuyy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gebzdirwg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/ghwoihybd.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gzzqmspnu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gpsckawud.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gvofxbyvl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gtgqhqpup.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gqkeyohxx.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/greviqtou.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/glxogjmkp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/goufvhtcd.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gqpuumccm.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gmiczjkgj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/guozhvmkd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gpqxegqbd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gfeuugafe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gcbwnzdrm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gvjpvcsjv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gsqyqewai.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/glqxbojpv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gcnrdbvim.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gxgvgbloo.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gtrepmrhm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gqovadbpo.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmoqhjbdh.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gweammryp.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvzstuqgc.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gkrshksrg.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gproezkqh.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gbvkdssuz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gpdsdaqsm.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gglsnglvg.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gczzmufpy.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/ggzfqpvmk.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gqkhgugre.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gmntrsfyv.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gidqpmyzs.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gzojhtnra.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gbyiqlstq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyjbakzjc.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gpgaoyrdv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtxzxymlv.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/ghxuydgyw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gzmvqjrgb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gdteipezb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwkxlmgkp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgaicjpz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gihamdnql.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gizynpzdy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/goqregfvb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdfcjwyzl.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gdmoxkxsp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gicbtucks.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gkqebkwug.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/glvbulvna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/glctoxtdc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gvepuhjhr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gfpqualdd.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gwgqwzyrs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gjiqolqfo.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gvgwqzxog.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gebthxabx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/giattglyn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gyqtusmaz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxxvsee.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gwvlbgznq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gddmiqjgs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gkglxtica.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gvpcravsh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gxclyedsi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gpkgakeqt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gxyefhqyp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvqsqwfhz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gredfsoxb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gyfzdahac.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/ghxrlcypl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gdlxfkzeb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gttwsdnmn.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/goxwhxzcw.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gwhxzfpqd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gujaatvvx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjkybbgcs.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/grigffycq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gvxkzbepo.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/giyuuygzu.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gaufkllxz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gfgnglzhy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gmgfshrsk.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gddpukgyh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gjrgagydv.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvhydfgjq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gagggwbun.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/ghrnndvky.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gxmnepnef.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gwbtheezh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ggniznnks.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gwjeunehm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gtiyyrzdb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gxwtlppli.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/grsxwkqxu.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gyczrtgog.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gokajmcbb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gzyohpgfc.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gpfgaysuk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gqyhqzxfy.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gvmfcapjp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gkacgctpq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gbvzhnxtk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggxoheagn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gbfidjhzb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/ghjjewvwm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gyaexkoyt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/ggpvwdxfa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqbgcunpn.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gouakcwgb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtudhlcpt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/glgzuznml.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gtfvohbyx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/glxgcpkeg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gyepfxibz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gkdykctkt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/glgmsorfw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gumriwlgq.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmnyvnlqi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gzqkjrxwl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gwndenrag.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gaccxxauj.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gbdgmcphv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gjosfyqxw.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gqlvfxeou.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/ggjoqvxgu.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gvxfqilqo.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/grfwezlew.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/ggbsancmd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gcfnhliko.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gbnpgnhoa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/goazbujrf.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gbccaxetp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gpodlxozn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/guefcaoli.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/ghozscnec.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gcrjnwcrf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gysefjkcy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gozoghyra.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gkbvqdcwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/ghebevqpy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/ghmfrxxbo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gluxzajyv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gxnoxaqxd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gbrdcpdyc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gozahuelh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gmtdqcder.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grpzybekw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gfegzbqut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqbyfxdfa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqhupbhzy.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gjmvponak.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gikomxtgz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/glmcfmfuz.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gfgglsici.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gqtdqbnxv.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gpmzrdoyl.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gebocfnzs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gviibxknc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gqichegrg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gxsacmjqe.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtbtrllfl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gnlbfvnib.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gjkdhjxix.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gtjgpxjon.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/ghryecbwq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gzbnxxfmw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gvciluepi.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gdyqtrtxt.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gtpjgzetg.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/grnmugcoy.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gnqfiyens.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gwfxxoytv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gyqmrgmza.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gapwamvkz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/grdwjwljl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gltklmkne.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gunifpuwc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/grwhxsgbh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gyagciekz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfidqbma.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvmpoykux.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gauabwoou.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkrnpwfgm.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gbphqrqmz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gliyjgaci.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gwrruhmld.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmypglphq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gwekbmjoj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/glmusomgv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gilofpgou.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gfoabpimt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gqfqskuzv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gsujneppm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gzjztkoom.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/garfdcbjs.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ghjhntkmn.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gjlcvmgbg.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/grfmdklwa.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gsmnopurm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gekcrxkdy.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gqueehvaw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gpmklqpmi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gucvajwwd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gtvvjfgoy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gvvcvhmpf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gfjgxejdy.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqyemxsud.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gposxnqzg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gnxxiitpd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/giggomzxz.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gekgjujqy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/guskxnvgd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/glkwffmvs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gbgxoceuv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gfhklftnn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzglieyey.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/garlopsxa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gsegvvqrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/ggcdrxjso.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gugavehqn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gghlmgcnb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gfenswkkz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gddrietgl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ggpfuemis.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gjkeovkln.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grzsovhyv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gvmfgvfqi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ggbohywoh.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gqraxsbew.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gtbzylubo.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gsuhimrot.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gevgcnpkw.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gwzixihzt.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/galwlkpbe.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvrxvktkr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gleivvqll.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gvaxtppmo.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gdaqtagsm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gyjdamcol.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzmgqaykw.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gdapfbfdw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gacpnurex.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxeccqzdz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gsufyrnlk.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gnrabavlw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gfdgflilp.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gdyjyxmlx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gysbnqiwj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gggcadcjr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/geqfufhjx.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gzvtkdrta.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gqycfyenx.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gocbitvth.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gwpwsdvnm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsjmxzlsv.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gqdjdbgcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnewbnuud.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gmroinhov.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gqzskamef.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxyvhpzz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gvkxljcaq.sHtML


<!-- 参考信息 -->