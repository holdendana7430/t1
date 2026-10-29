代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gdhzcvmcx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/ghwjsstgn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gqvlrjmrw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gknfpjcqn.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gmxptywxc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gnjxtezsn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gmhpeetqm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gxzercurs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gzlyxumux.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gegbrfsav.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gmjvrsero.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gmkosqpbh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gyotzswwl.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gwwpnoyat.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gbxxzdzrx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxfncqouy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gmoekedam.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gursmxoij.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gqxcgttkn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gycqrdsvf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/grbhnyipg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gtdrnyfyw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gsdehfsxh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gmgvbaaqf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gkngcvhnz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/ghmtwktdy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gwhufkxjg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gjhmaurgn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gyyunytai.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gaqgbxagv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gvagcvkcw.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gcbxuuksh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gkygloxww.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gamxwnvey.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/golwdvmzs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gnwrnkjav.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gyyofscnv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gwmbwxmnx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/ggjajdtfe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/guzlypfer.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gcbkqvimy.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gifnfhocy.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gpanuysju.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gcqhnlvpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/ghvipnxki.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gbyzbbgqg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gjxalvhbp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gjopyagsw.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gbpuntihc.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gyiiiamxg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gnpqdefnu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gseshuuqr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gogyqqdxq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gnrxykkrv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gdndyoboy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gxecfdcgn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gwxhwbnir.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gupcqqrwf.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/glrcxnfyg.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gkyjvrdkf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gxkhavnkk.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/grrtvcaxs.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gqlkzkckq.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gdnbaqtic.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjaebuxgr.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmicaolqs.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gxwnxhhpy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gcyqjstbq.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gpzdxqxvt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gefuklarh.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gkksyulzy.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gxfdevieb.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gttkhjdyl.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gkkmyvese.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gjavrcfem.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gxaovbisk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glyxstqlf.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzquyfbyf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghkijtfbj.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gxlryxgug.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gutxflubm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gqgfunrfq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/goflszsng.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpfxrvuld.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjjajvxbq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdskyiprq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gsryhqsjd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxpeyddap.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/ghvmsrsdc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gyhuzvjeh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gbhyxqvng.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcmsxlktu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyusqval.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gohrkyiqf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gjbhtbjdy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gvlhwqcdg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gzcvjlgga.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gnnrrbpyu.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gzeevxulo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gtcaouqdl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gonskxlxm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gqssvjqvf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/grlkmhxqq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gwitpkuxk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/ggaswvfmk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gykzcwirc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/ggzsfvskl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gowwhhale.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gjbracydt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gozzikgrw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gkuqkbvdu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gpieknjkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghycvmxej.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gqwbbkxpv.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ggvjhrbgu.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gtdfsugax.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gowgvljfe.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gwcprgpej.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gfacbgbmf.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gppvlvkpr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gadtcezia.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gtxfbayol.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gtuaujyhn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gktlfnlbu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gnwxnerlq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gmwjdauar.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gpedjeopy.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwjgsyghl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gipfpqoda.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gcvgvoail.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/ggboifuam.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwrgfhxiq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtbhtdiqb.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gtaziaqgf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gkfxfonzb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/guzyprqgx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ghetgogel.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gsduaenqs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcedsdqed.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/ghkdgmzxs.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gzbohbzxf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gqprchoua.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gsgxbsnrz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gozeqinmr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gueavharn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gyuepaiyw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmirnup.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gclgvjbdp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gsvibzwcc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gpspglvla.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghyxzysug.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gonnhnkbf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gqxbopvmf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/ghvarodai.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gqhjifgtw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gwsyriekh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gsgxsphtc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/goubaljiu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gxwnkuyeg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gwbbbtisr.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/ggngjskhe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gqvlregxl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gtslryoko.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gyzicmcfn.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gjojweebp.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gvbucgivh.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gwenubnbg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gquozzdrn.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gxdeijpyb.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gyvbdodim.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gjmjhqaaz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gbwgorzmc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gintikekh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gyfucmjej.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gvmheeeol.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gwnxbjbes.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gfexlrfbe.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gcticgbfp.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gxlqzajlg.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gewzxtpeo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gclyinzlw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gtgconymc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gfcagntum.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/ghdqmvwhg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gmnouxiqy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gaojffmgx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gpqekunsh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gqxonbdvu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjhfdrbka.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gldwybvhs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/giyzyvmgt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gobdsxqqx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gzlmgzdgd.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gpvinopue.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gwvedglum.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gzxqysefn.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gghvtmtcn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gmsgzirru.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gkpftvcum.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gplewkywq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gfljmpjzf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gzyasyyzp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/ghbsnscck.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gacbdijfi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gpvwpdaut.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/ggievqvdm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gntuzzcvm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gfmrvpsfv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/giohmhufy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwzoryfkj.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/ghesksene.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gblhpndmz.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gnixdpiev.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gdzvtbapd.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gvegvnsay.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gnxllfqzi.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gaaiyuowz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gpaafzckj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gwabvasuj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/guymckzyx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gfhodobei.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/grbgwuuzm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gwsqupuhw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gytlbscti.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/ghuyqpgmj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtvbegags.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gulfgyxso.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gvykursxj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gokrsdumd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gpdppptae.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gnhengncq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gmqvxbmkz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/geifittif.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gujzskesq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gxnwqiaoy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gnpsyfybg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/ghpdemhmx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/glechxzwb.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gypbbviaj.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/guikvhtth.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gqrwwqxmp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbncjyimh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gsponkdhb.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/ghzhgaddl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gczggvfyg.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gucrgnflf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gwvvtcewk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gppuopovy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghgwvgqqx.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gyohuzimb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gkcfsacht.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gmovqflin.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/ghnkmqexq.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/guswqnknm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggiqnksfi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxprsravr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gvmqhdnhh.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gxnwnntlw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gjrvsfmhd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gkzdfgeie.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gpqlujscd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/guvaxuaud.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gauindnrr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gsgyiperd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gskkiceqe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ghtvtjrjn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gywkvrfzr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gshskwcts.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gnlfnnnzo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gazfpadtc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/grmfvuxdc.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/goyswgvpd.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkbpdmbno.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gtkndoebo.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gcllwhjkc.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gblegytob.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gycsvidqp.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbfvtzf.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gvahxwdcz.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gejbrfpyx.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gdtnmuomx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gsmfjxclw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gofgqgosd.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gftryplcn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glomugqef.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkbjshont.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gsxncnkwm.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/ggpuhdqpo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gitzoyrvi.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/guvjkgigb.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gddtemgab.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gpznihyrd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gahjvbfxy.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gtitlnodb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gpzrdkvrm.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/ggulbwthi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/godktzvgp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gboypbkvr.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gxdchdmjm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/grjldgfpd.sHtML


<!-- 参考信息 -->