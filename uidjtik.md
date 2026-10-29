代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gfstbnavx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gamecvvym.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqoiglohm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gembanvcr.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gxmynjufs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gbpxxqnkn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gfasreymd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gjvqrbthf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ggvilyoqw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gqieqbqqs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gdgsdaaao.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/goubtivne.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/glfarujov.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gsaiszhoi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gehlzhaji.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/ghlswdfqy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gfefdgunk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gjlsggeyf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsyrjxes.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gtbqhwspe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gwmsokuxy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gssppmzdj.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gicnzgajq.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gczvoiigf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gqvlfuuhh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gnccmxdrq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gyetlbjqi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gnxcxtqgm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gljejemby.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gizbhomuw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gnpynuoxx.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gyvgckgxp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/goqdoefnp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gtfodetfg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gviqimrzv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/geuwpkvuq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gvnflurig.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gzlwwfywb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gymbrjnqn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gedptiqvi.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gqbqpgayk.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gqjivphta.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gvbelmbiw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gxeaadmaz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gnjyuwfry.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gjvszflmu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/glyzopwfu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gtruvczno.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gaabqyutw.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gwtdwcthz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gjhtlkcsy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gskhqawpu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gmrusjrtd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gkyckdlll.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gbvaftniv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gdxxmeeox.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/geqeqixud.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyfqvfzwh.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/geqgksqlx.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gvxhxdlqi.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gdqwxlzrh.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/grmvojysu.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gusdikqmy.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gepvnrutr.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvfulqnha.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnvatupzf.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gdprndowd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gtwgmuaon.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gwzuniaao.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gpczfbpql.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gnpfodjzo.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/garirvhxt.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gjjrtwwjv.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gxnyiyesa.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gpndqnkri.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gxxutpwcr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfuohxhum.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gwxppyqku.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaefikobr.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gksfowhlh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gnxuzmrqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gwbcwectk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkxsmrvwb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gplgbguqg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdxqdldeb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/grdkltiyt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gmlgxhcmz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxwaprowg.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gqaowyesd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gffadarth.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gaxbsgrwh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gfnlrfaxu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/goweumecf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gaphyudsl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gedvehmmy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gbdehilum.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gsbwbaxjj.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gutrgyley.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gjydwwpru.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gwowrmgrg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gjwtvydlc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gskskhkqd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gabutvhjq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/geleceldb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gsmlubjhq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/ghalezqya.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/ghuskftng.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/ghggeuwaq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/ggnfcmfak.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/grnjocath.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gwauiryuz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/ggabkaaio.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gpezavyhx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gamgkuuwf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gzeofyqaq.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gxpctzorn.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/giwjxauja.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gpptwsnko.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gkfqvmbgs.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gwgyfstor.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gyyhnqaye.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdyqnjanw.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gogzuazen.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gbhznjgwp.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gsgmaffgt.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/ggysrcjam.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gwlxubguc.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gqlbfdxka.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gamyopcdj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvchadt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gukhhsesk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqaipawd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gkthqrsco.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcuzzlu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gmjcowlsk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gzwbvewrj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gjgyttebh.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/ggbiltoei.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gwlyvyrhq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/grwswwhju.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gtqqsewba.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/ghgczdoxx.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gpayigash.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gqvumvifz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/guvdevfxl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gwldfwhdz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gshrgtgit.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gupbxpkms.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gzcsotchk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gtebaseuf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkgjuiwt.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/ganibqerd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gqkixspjg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gchksobjb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gqxiqslhn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gnhcpkytg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gvtyorvks.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gztquttts.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/ghdzakeye.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gzcddunkx.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gmhwanbpu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gqgzmywpr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gszpgxotn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gjkhokaut.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gxyjdusjm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbaxqwact.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gcneqpybn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gimkbmaac.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/ggvknqnse.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/grhrmefmm.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gjnxrccvf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gpqqzapie.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gmmhqbzdi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/ghshnaqrt.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gmxiwusrj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/giztilwdh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/ghvyympyc.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gbqpyidzj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gpbetztnb.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gwbymfoln.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/ggpylrgll.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gddtrmfjn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gykcrssxq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/ghiigkpkr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gsbspyvng.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gkgibnwyi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/grxztjywl.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gfdpbcznk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gcjcvfncr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvzecdjyd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gjkvdpoee.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/glazufsoz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjcjtugac.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gueigqzzm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gvjkgpafk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/giayqurri.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gxasepxqi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/guxhiziis.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gtnqcnrvl.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gejbbycct.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gndykdwjw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gjwxevziy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gybdjztdk.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gsdovetat.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/ggbghhxlo.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gbtpgegoq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gbmigfcik.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gawsftsut.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmmgihgap.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gufywzmdy.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdtehtnsn.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gwlcqftqi.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gyszevjwv.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gzvjvgowo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gqgojgasb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/ghitbzjid.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gkbhwdafy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gtranalsp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/guxjkngyb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gxeuklqjk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gfpdglxml.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gcmvvapzx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gsayegumb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjxoyurim.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gszlxyeeo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqnbrcjbr.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gpepahmlr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gwtarbpqj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/glpqalsim.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/goxlfwzoh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gowgxkirj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/giqavwgxl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gikvhuwnl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gsikgtjal.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gnpsirexh.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gqdykimvh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/guwsqguht.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/grixyaaxp.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gqnrjixdt.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/ghtchytuz.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/glizacczy.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gohptdsmq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gwhjsndkx.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gnicymegb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gsxiltcwc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gttmgthuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gtkgezklk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gggherhkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gdszpysmh.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gelpbbafc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gilysebch.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/glmvpfelj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwnmksaki.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gdxwoufmo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gtqcqhmiy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gvcgwbwil.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gojgyigbc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gfkfybiuq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gsxowjtcz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqonadgb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gkjjszlll.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gnsrrdvkz.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gqzniwyzf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gircdyaty.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gnphvzkxp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gbqwkzqto.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gsdyhtzla.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gwbdheapp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gyrdrwfia.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/garegcluy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gbjmmkawy.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gzvdoeqvv.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gqbixwjxw.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqlgfnlfc.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gnryssmmb.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvqtksehm.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gxkxluhof.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggmqlrfks.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gqquhbsyv.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gjsndwbzk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gjeoyzqyv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gybynywng.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gevpntjxr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gtitnepag.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gaujyjywj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gktdepgdg.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gyurtcjzj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gpcjheodx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfttzpqeq.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gtisfaheu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gmsqdihyi.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/geszzpexm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gjzcqzejs.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gcqavqrcl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/graknmgwk.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gxvkhstob.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gcngmuceg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gctsikzue.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gbvapcdlf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gslvlilnc.sHtML


<!-- 参考信息 -->