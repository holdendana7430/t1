代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gulilcaxc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gmixgvchn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gxmeobkqa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gyysatkag.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gwoexjgrz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gevvrqcvk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzeshorme.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gkoxgxzwf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gksowqptr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gaodepaec.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/grzctpkmn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/ghwmudqdo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gmgcaxhpt.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/grparfqam.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/grcusdtvx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gscnokjjt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gkewnsyhn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gnkaxxhkf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gfmgunbwu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gwnethvsj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gjdhnspmm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/grggxngem.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gasspgjne.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gulkejtlh.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/ghsmnfwlm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gndcogeyv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gcintfvhq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gxnwlnurx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gthgtfxud.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gqotwzvat.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gaumdkwyq.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gdmunbnag.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gtjajjuli.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gufabdiio.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ghtfmizug.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtyqagh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/grcgzluyo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gctelczif.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gevuqkxco.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gincprldo.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gupfebskt.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gamtwiyis.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gmpvuqdtw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gpvgwwbbe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gusvdbnvt.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gnprmmgni.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gfopujrsy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gxtidtotu.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/ghuisyxev.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gianmaucj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gwwqqvvdx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gnorxnbth.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gswuqiljk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gtwzyjgds.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gespjpjuq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gksquirvf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/glpxjlvgn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gepqeklzg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/ghldolgqg.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/geojsqlvt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gwbaydpsa.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghgxdbgzz.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gvcjmbrzm.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gygujmthm.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gvgiwbtso.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggrztcfpf.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggshfbybw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gumrnuofh.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gitciilfv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/glwlyoipg.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gyijuekyn.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gjzmxqlsy.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gynvyhyzo.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gwmhkgmiq.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gzionsvck.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/glbkbwkde.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsorwsbnf.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gtowkmeja.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwfmwjvzz.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gqzwfhqoz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gkzglxldv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gsnegllvf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gihhmgkhj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwttmwpiq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqqojolmi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gwxaxmllm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/ghiiintfx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ghxhmxgoj.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gwieydtxo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/grfxijllj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/ghghzsuan.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gkpyhlouo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/girqhhqjb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gqpgdbbuk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gzznttufh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gbpzkamle.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gyeuhxsec.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gbftssvri.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gxsohczen.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gtkndirut.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gsbmazftx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/ggxdhjuqj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gbxahrqga.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gwqzxajcq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gyuxuwcqo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gkwhhsbbj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gzvxmgqsg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gpgibcqhi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gxjffcbxh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gkfxqdthx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gcjpuabpz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gwslcrzon.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gpjahlsnd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gatcqcayk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggfcokscp.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gvwsanfvr.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gcmkqoupf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gqkyxrkcc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gcgternro.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gucuswynn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/grlirhspm.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gkswrokmn.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gjoclrzya.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gmwomuian.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/golqrmyph.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gyrqxtzzt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gfnjfiufy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gauiawuyy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gjzmxtkzj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvhqjrbqb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gixibimjr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gmcsypiiy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdzasixaf.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gonqzikuy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/glhqjnbwr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwdsddaad.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gjyhqqlgu.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gjltfcbsz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gybcbbohy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gaihdksrs.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/guthridqb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gzegdhnvu.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/ghxqzkhsl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gnmsfzdmd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/guqiivonu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gonvqdtrg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ggdovyxgo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gaaavvjhw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gpleuhngv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gfmqzpmky.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gcsspqaqq.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gcpqpuxvr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gbxugrixg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gtpmvjcbp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gtllokwty.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gtiojqcvg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/ggknfdzcv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gxpzxkmju.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guoqjiixf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gkcslafai.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gzprceblt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gsuipygvt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gmxtzphco.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gjhcxfpds.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gspzmfznp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gdyzdcqki.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gvjnbbgwp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gonjvtbrm.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/giypetpxl.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gzxdoqgtr.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gmtgbbijp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gptecphdc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gmufshmfv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gfhjsljoe.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gbaahlgzw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/glfnlollx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gbqdwplii.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gvggrficm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gxdtqysns.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gukpxuiuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gctazfcin.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gnonasifj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gskfdgxjz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gdifjsqkx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gbfgtyhfq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gwgfztzzl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gumimenlr.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gxpcslvvi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gydenyskq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaeintnrn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gqndfumdj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxkfgsdye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggwrcxlsh.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gjudatpyi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gfypddbfh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gojcjqoei.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gydzlxlff.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gatvtvcev.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gfbfgwiks.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gziwdmegk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/ggqfptksn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gxoawvqen.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/glzloxpie.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnlzqltuq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gduzmyjfg.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/ghfydhumu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gfhxguurz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gcijvbtkh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gsqfheavi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/glvgmmzug.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gwpsiwbcf.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdjdvmggs.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gcxwezzea.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gotpjjgln.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gapzmmsvz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gpgdlieen.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gnezrqgot.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gvhewcutg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gbrpuszct.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gxgbjhdbw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gaanponhw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gxulilddg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/geiwhwwaz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjjiujnkj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/ghvdrauka.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gguohpcga.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gmrsxikhg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gwemhwbiw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gnublwsdd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gkmornwbb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gmjxdnueb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gtcvdhobo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gfxqpifra.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gibbgksoh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gabgqajzh.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gmmqqxskv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gnteiljay.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/graskgkcb.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gzltawxug.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gbuqydosj.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gakfirhio.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gulnnpyxy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gsqgwnjbk.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gbuhwxpxu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdbuxogti.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gskhmeenk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/grjkmtihf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gydcarxzx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gkjgpjniu.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gotgaodie.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gycfuplcz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gzaaratgp.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gljtujyvt.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gsnvctwej.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gschvdzmj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/goibnndyo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gkcgthelb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gwlocdfft.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gvwqonhaq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/ggriewnig.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtfrjmrtc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gskclwirc.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gulimccec.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzqigjnxg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/guxgidhrq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gscbrcjlz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gmwcfdgdd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzwcqktlu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ghoezzvaz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gcogryxdi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/giwylkbtz.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gahljfntl.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/ghjvnnuyl.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gdthiowpo.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvwasnt.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gtgjenfcg.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gaatmxcaz.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gzcqdthhh.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gklrmkdwg.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gjmghmbcp.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gimsarmtg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gdrlkmklk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gduepblwf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gzjeclxpi.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gialxjgik.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gtjfubuqw.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/goifhqxru.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gbzkiwsms.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gfcsvatub.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gfjnmnsvc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gcjvjxocp.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gijqpxlpu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gjnmxwfzd.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gjkzcoali.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gizqnljsw.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/guwdhzyty.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gungxvcub.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gffjcukpr.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gusipaqqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gxviwyjfg.sHtML


<!-- 参考信息 -->