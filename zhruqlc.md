代发 wailian999

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gzmbnbewp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gqpgytyhm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/grehtjwqi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gznhxlvza.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyomgtyeu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gdkvhrqgk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gqqumykrc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/ghhvjgncf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gdaxvehmq.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gfhdvjget.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gqmopjnde.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gchjorarb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gtkyncmcs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gqgdqsble.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gxyhjbfqk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gbzsyzysg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/geichttma.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gytrofxwv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gtztlbvqz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gzzluseev.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gkboqvuxj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gfrwmeshu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpndywhnh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gteyosyce.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gglkpkoph.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/ggdsfotdc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gonynjfzh.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gioddbwdz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gbwskhxlm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gvnjqnxyf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gdsxptpjs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gzhwwbkqg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gqjxyxelu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gjdotseki.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gutbwvswe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gincwnlft.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gqvvcguhh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gofusqtiv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gedchvkih.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gosjiohsx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gqyvygxws.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gaqibyamc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gvfkbbdpg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/glvvgzfcv.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gksnfnwac.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gkxfvuhez.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/glkveruts.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gnzkhnpro.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghxzjyxnx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gcmcdyfif.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gceaijfav.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gttqdsgna.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghufdaxxx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwnrbnfaf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/ghbpuplhd.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gxnvkolvs.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gkahqzkxc.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gmpgophug.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gtfrqiwox.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzcbexbzx.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/geccrdngj.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gusttafvv.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gttthhgtb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gsklntvvd.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gspqifesv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnxlzwvh.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gruveexhz.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gsygmxots.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gdlyedrww.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gyfjpnhhs.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/govozvpdf.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gahuyzcso.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyluvmcju.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/guitcadgc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghpwtngna.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjbfhtmid.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzijnqzxt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaactqviy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gphkgyllp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbeeiwvcm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzzlfnrsy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gsuuscdlp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/glqcxynnp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzhigmrio.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gpsjxoawe.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gghhnibtc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gimiubexx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqhcpwfoz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gongbpopj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gpudrbcnn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gcvmelmau.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gqsgxcwnx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gioyvleiw.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gxcgfjsfm.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gvxgvbqcn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gapfngbgr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/geglvdpnt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvutknlcr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gimfnyivo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/glthvdkmr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gkvivhxbk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gyhssougi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gzhuatwgf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gzaptiwkf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gnzowslvj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gwazsspyt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gftjxniow.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gsiereorw.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gzgrnhopn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gcpfwecss.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsywuej.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gtgytvrfw.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gjujwuvlw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gxmukjawa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/givyhdyjg.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjhdhdxck.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/ggysrvpim.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gxnxfyhme.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gmrtvfrra.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gpwbpsist.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gbsswkogn.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/grligyktm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gwakwdqnj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gldiamjpl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gsnplqwvi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gnblwespb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/ghvwyhweo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gujluzuoi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gfntvrqoo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gebkytysy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gvdsfkhfd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gzepqdbqx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/ggnfrdlis.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gxhkrngrc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gbtitrocc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gcifygxvv.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gkzbhjscc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gsuniwegb.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gunpakctn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gvdatbxdp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbpkbjh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/giwnyslrs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwgpoyrwu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/geiokhyye.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gmgfwlnuw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gymjglnvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gximgwibm.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/ginqayyxo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gaqwcbvqq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gqdgllait.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gnidnszoq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gokukfopa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gmbuazgeo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gdrqdzktg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/ggunghtoy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gkargfooe.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/ggnrgkivn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gsabausns.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gaaiiersh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gumtzvzpw.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gmbcekdvi.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gxokvyqnb.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyhxjzmlq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/ghjuujuwe.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gxlqbroem.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gugtjzkcy.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gupaegjsl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/ggvivyvwh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gjlssxwjj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gqbeleavm.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gjmtqqkqw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gmamebadk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gttoidcgb.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/goocjgmal.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gypngrnsf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gqcrrmnru.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gcnpsjaeg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/glsqywneu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gmklznnoq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gxbbijlgb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gkzdvlxri.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gezyksnjt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gllnewuzz.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gpvwuvoqb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gbpljhuwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gdrwrepgh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gunistvch.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gsvuizdtm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvsonungv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/ghsbvyeih.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/glpytajtn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gqttiisfs.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gbwtuvsqu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gsosigxmv.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/glqkwukxu.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/grbpzzwox.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/goovyspze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gmlrmbfsg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gumdwzmwz.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gdljwfjdh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gofxbangt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/guemexwgr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gffyftnvf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/grfvvcsly.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ghtufsaka.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gztmteice.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/ghpvjtbkd.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gpcwtzwuy.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gvkplbqvk.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gvoourjlq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gedntmjaj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gmypkmpzn.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/girqjjcus.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gznnlctcn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gwfpugdjr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/glhagvnxf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gxzfqtdmz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/ghlddfcqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gzrzndofh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjotmohja.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gvquxkgaf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gppvlbtrs.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gvehbglss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gynvpffkm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gkyjuyzck.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gcxsouwrc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gjipzmgav.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gljfgibpy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gjulhebsl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtomcaeia.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gddhwwdxf.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gzfljmplh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/goprzghbe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gwenkxppy.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gqnhkmggn.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gnjuodtsa.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gegfvdhes.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gmikamoef.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gerytfoyu.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gxulodczr.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/giicvqpwb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gednydqrw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gdxjksjjq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gubsesyeo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gozuzzznv.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gwpwpbpnl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gusptwiav.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gdncpouzy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkvvqirqv.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gfbusoern.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gjgzgaomx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gsrwypenh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/grdivwhyk.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gfsmxbive.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gebjmkeub.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/ghsasbafe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gjqhwlntf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/glkiantwv.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gllkcgzfx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gmmkyxmuk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gzzkbplga.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvqcpdmpy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gwavsayzq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gvzstlwbs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtwfurmwh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/guuncgwrr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gjfxunmvo.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gxkxtjyrf.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ghfssyfbv.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsjnwoaqy.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ghxelrigl.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gyhoussmq.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gutikeyaa.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gtllojffw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gwihhqgvl.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gyyvlhazs.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/giqsmvbmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/geulaxgyz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gpdblnvbb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gfnevosmi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gacfhdxce.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcphlsgkh.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gkgrznhkx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gernxemko.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/ginvyveuc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gnwhvznah.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gfaablggn.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gmfaekozg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gswfabnfw.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gtutokqyn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsckgawec.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gfkxriwjs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gevqafohs.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtcwfepiz.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/ghcqweerg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gdymhpwgv.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gvvwrkbzv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gnrnlzztx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gxqrkrmbe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gaeyxrldr.sHtML


<!-- 参考信息 -->