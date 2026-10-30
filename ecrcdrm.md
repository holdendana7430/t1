代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/goofanlys.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gofwpjsiz.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/ghxvgalec.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gmqxunajy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gsoqlesht.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/ghriuktya.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gfpgkrvnj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gmdibdthg.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/getaeuwak.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gvxarrjbs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/ghjcewtkr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ghqnvnerd.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gxyymmulp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gbgbzupai.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gduvapwsw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gxodwqysl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gksawxkqm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gfbcyyxqc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gcssaymrf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gqnavjvng.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grputfvyi.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gyzobocug.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gpdijvngk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gsofqtxkn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gscsayoug.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gjqgvmwie.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/giyjpqhgf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gruyukikk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gokjjujqr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gmlytprgj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gnutchlym.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gywaudvwq.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/guzwhaeyc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gscrvhxgt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gnjyfflwj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gxwhewuda.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpcyczp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gkpbxiusm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gecgoutqe.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gbryyjqmp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gzwhjorde.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gdtzqwdrv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/glwzdemdi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gvymgzhmg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gdcmerutm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gyqfepvnx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/glhepivbz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gtgujlypn.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gnefulkgj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gecojsiqo.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gaflgihng.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gonlkjkri.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/ghizkwtuv.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gyhpsbzet.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gfywenjhs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gugcahqbj.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gqgdclxzs.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gzfmubwax.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gnpzpoyxd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gwobtogjs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gspbxhbno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdlgptznu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvufxxaz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gnwqgpdhs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gxgenigaj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gekcpcohh.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gcuezbtxn.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gimuxkbnp.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/ggkqexskh.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gklxzonsf.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gbsjbrmyd.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbaetaaib.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gjovjkiej.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glalusewe.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxmmunqtu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gvretyqxg.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gqzwsssqv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxismlyc.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gqfeqhhqd.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/grjcgtrwp.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gglulmocp.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gnoeeqyzf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gqjltrxhc.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/grgusrslg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geqquyavc.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gxtamwoft.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtaamdegb.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/geqdrsviz.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gmrurlnag.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnafwwthi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcgmkwscr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqzaxaayo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggywmvnnh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gumhznrzk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gguhmvxft.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gqgpmvgby.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gnradmcvq.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gezksggho.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gawtmgnzw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gerqpyire.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/ggcmmcqpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gwpfwojsk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/grdjycoec.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gaogunswb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjddkktd.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gkqdecvjm.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gieryqoge.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/ggjcrshxz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gxnvazrds.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gsavmueoq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gwjamrsrb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gwuwnwxvg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gaonvgqcc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gzxxngehr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gpbjimdce.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gbarqolmk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/geasmehws.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwzohcjxm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/guyenuyki.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gayjthspn.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gpwtcrwqj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqyxdcfz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gsmoqdcax.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gopenjhqv.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gmrcerxux.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/glpfgfrky.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmxafjkdo.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gkonvufvv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/ghvmdpgyo.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gewsuphvv.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gnbhxshlq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/geivbfxvm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/griacixrc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gnvhjqrvx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gftezyqcb.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gwmvhcwsu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/glttegstr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gxhdxcphp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gvqocnfpx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gjmpupity.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/giuwzjycs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gyynmrtvz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gxhxjzeth.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/ghcjlkmcs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gbgiqsfvs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/govxkoztq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gkaltspob.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gqxtteovv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gvutvowvo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/ghnwvhtrm.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/ghiipucnz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gwwakuyhb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gqtbnmqjf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gaxtsveey.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqregnuxa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/garzklzus.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/ggyqcspvs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gwoqoijhy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gdozhjucr.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gkxmqpaxl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfazwoizh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gbayocagw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gttpkinak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gqtvhdpnc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gwlqjxreh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/ghtmwiygv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gcxmtvsyw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gccnbtckl.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/grdkljgrk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/ggvnxvpea.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gumbuwgbm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gndotozyv.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gjugqurte.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/glwxjiidd.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/grvlklnpr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gajdsoadk.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghqyhbodd.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/ggjobetst.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/ghekjdlmi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gdrmnncaw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gizcnorid.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsmdclt.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gvberximf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gakzznjdt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/ghxutiooe.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/ggjvvtmgy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gsotwqjxf.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gbjqdrpdi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gbedgfmeo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/goqnrmbzy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gsuhfaqsv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gircxfqsu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gebpiiaof.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/guqqlohvz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfhcrio.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/guyitkdbe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/guekgqkuj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gzyvfbksw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gotfrhqxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzeauaeqs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/giafircmk.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/ggsxtfutd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gnhtbcqiz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gjahzysqw.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gqcwtappx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gtudvjyer.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gbfsgourg.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gigeiegto.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gjktqchwy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbabzgil.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gzfrjqexg.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gmiyanxvq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gbitwjyoy.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gequbmmmo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gtyrnlrkh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gjzwpzixq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gagxgpmvr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gzocnscgs.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gwcudpaub.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gsttayfvf.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gjyqjocvz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gmesvvlci.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/glajemiak.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gaswrlzwu.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gggiehnma.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gqqrmgovq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gjbhyfypi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gfasfchzk.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/geghoeoqh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gpoxszrgd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gxfknkavw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzcnpcbir.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gfdkglfpv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggrinaewf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gwnatxxlt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gbptcqciv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gaewfklaz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gamhpfidy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gzzaxetww.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gyyypaynu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/ggngejddj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gyafdhmqm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gfhkkojih.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/grizczwtw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gqttiwack.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gfoupweer.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gpzokattr.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtsrnpmrr.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/grttcbyap.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gefszfypy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ggkhvvoii.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gahgvkacn.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gkbndnddt.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gddcetrje.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gmfkabjst.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/giqkylzch.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/glmryqhrk.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gybmptupz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/glmkkzpoe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gqhafhvxa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gkfcugzxp.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gftjavzbd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/guuyujkzu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gswfbfaku.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gvgqkkxrp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/goyiisdrj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/golgaemvq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gxaqevldp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gelomoqnb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gfquepxdk.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gukmlngoa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gnklkhboj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvwurdfva.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghgjyzjab.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/grmfdfowf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/grhvjtotq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gprwlabyn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gtvawpphf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/goaludrqp.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gbfnrjkxc.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gknsbsvdd.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggaewycel.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gygrgxxas.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gohvfdutk.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gykkghbif.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gtqoffmnw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gmxfjaadh.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gcpiorjwi.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gfdoggppc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gneugwnja.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gwizuzsbp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxtsglplf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gvmdxoxiv.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjmswwhqr.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gumefvdpk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gbnzlorzl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gbevxlcvb.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gfvikztwd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/glqrlxxqz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gcevijzqr.sHtML


<!-- 参考信息 -->