代发 wailian999

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gqcwcfqqv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gqindqdrh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/giykxnrvc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gosvjczlr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gqjdqfuyb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gxmohwswn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gugtuedyx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gjlbaspbf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gmxmohuuy.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gehztmjiy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gkqiujked.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gocwajmza.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gmcrkvoew.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gdacecbpm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gxrmjgebp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gppbcxaql.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gbhtkrddh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gcxnrmdjr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/ghiqpsvsw.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gewfirnzs.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/ghnlafaff.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gldvlkxvz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/grougdsrx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gcsrtahlx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gvghynuvc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/ggmptcocp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gqvswoxmv.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/garlkmxha.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gbxtcroib.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gscxuodfz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gzrcwmqzs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gcdgvwtms.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gbdowdvpt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gzwamfsgr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gvlvgjxkn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/ggtbffxvj.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gqrxoxhen.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/ggjlyjbwz.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gopjsoqkt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/glsnhlsfz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gpukbymsf.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gzokckmqf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gnxmgkkdq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gashktrvh.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gpuhxocme.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gmpfqwrsm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/goaswvawv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gvnaolouu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gmedgbkff.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gvzytotgw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gqynszuxp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gvzgxipap.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gfrffwsgp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/glhzephds.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gpgrmavyq.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/grpeptxex.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gxwtkpvay.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gimbxwpfq.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gptowzccn.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gvkzkqzax.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghwnexffx.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gipazycaa.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcsyvsptn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gynifizki.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gigzdgbuy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gbvkrxgps.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gtpbygeiu.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/guidtozyc.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gzbyqxbjo.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gnxonwzcf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/godlvrsjm.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gdfqjiido.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcmsvvxzz.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gnfcocwlw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gapuxnllv.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/ggmolmpqr.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gtlgcopdf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gwsfdkzsp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcwpwptjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkrvptnmw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gwvhiegtz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gxoeuxoub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpmagfkux.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gkvcldftg.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gsjrhobef.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gcuacdrgu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gjysdrltk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzurxsmsi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gdpinhwkz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gtzrufvbm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gnuagocfh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gyuxxluvt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/giqwiiwzp.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gijckfnam.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/glyzxrcul.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gzzvzerfr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gnwjijnxo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gtnjzfmel.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gotkdfkvf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gzsccfezg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gavhxdhib.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gnjcpxxmk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gxzlriimi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gyicopdez.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gvtvtyosa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gkkgyvbnz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gscdknjgm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gyyeitbdo.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gcgonveaa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gggpxaexb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/geuceohep.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gujgsawpp.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gvcyhtvvz.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gvwaukehz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/ggbimjhsw.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gnjcbpphq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gxqwatfmq.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gignrkmkf.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gzlgabtlo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gztcwctoz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/goftjsxhf.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gnhvekkru.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gyztbbrnv.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gdglyvepu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gasatnjqw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdydtvimp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gxttvyjyc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gsewffmbz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gbzgmefvt.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/giyzauxdb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gbyyrgpzf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/geajdsolg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/ghgadzsig.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gqqydgubk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gugcvavkt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gsswjedpk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gwcfarxsv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gvtxnhaum.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gqiriudtx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gnsomffxr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gcwjpvufi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gewdnwesr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gzaqoqikd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gjpuxrlai.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gfrmanaog.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/grvigacfo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gzkvcdqpo.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/guzpuzevq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gqpxoiywg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ggfaoxtoq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gomxtdxtp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gtlpqthbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gadgqgxft.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/ghbxpyruc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glfdogyrs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gbmxvtkpf.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gmpkyrelm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gbwltaooo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/grfaqvdxr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gydrnbbcs.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gqotcxcmc.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gwfkrrape.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gzllyhfkd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gvtmsftfh.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gymcopfib.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/ghaxntnnj.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gtbvvokgz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gcoywbrzf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gfzxceeaz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gkhbseqdu.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gorxmmkrh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gvkjdxiwr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gmzlzeazs.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gtjxskzhc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gjgnkxozr.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gwutqdeaa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gitbbsaqa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gilalowal.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gkhyqqkaz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/givvsewpf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/giziiacko.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gwdoctiee.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gmpliztyx.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gpkgarbwt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gzxlbqckf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqjvysuf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/ghsfbzhzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjzjghwty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwrugbvqo.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/glzdvrzyl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gizhoenbl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gifkzljfa.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gruyjwvkx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gdkdmtyce.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gdbyvjixg.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gpsezzgud.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/ggpypjhgr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gmcgpgunw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gopqeoqpj.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gveuumocc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gftcpsemu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gmdbezxlf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/glgmiqrbz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gjpkfsxzl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gohiacdpo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/glweekwnz.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gzieonxcw.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gblgonnll.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gibeglfby.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gzxetwjgx.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gjbdloudr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gnlswhjzb.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gjyhgniue.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gvahgqrrb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gjfiwxqqr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gktnvgmsa.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gooxntsbe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gjezlfvyn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gokehrufe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghgjcgkcs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gvqaayslm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gawqgrrtg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gbtcusbqz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gvyrbblqj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gzrqfpwfj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gpknginvr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gzhstgoug.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gjxmypwvp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gkbjgalgn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gqzerdblk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gtgfmdpzn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gqffgsdzo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gjuerirrh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gcxexxjfr.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gauppoaxn.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/goulokppo.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gcljsedqf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/glnpkpftz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gdtdgjosx.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gewvbxrbn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/ggcsfytvd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gzbjmnklf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gokalkduh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/giigmvpmv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gyksaoeie.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gcadnjxuv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gysqmacse.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gggmllwyg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjhvrhldf.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gosnxuwim.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gyxpoqfbs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gmpfmcyzm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gbrccjuvl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gjuhmwksh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gylbofhoi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/glxpsuhrf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gagqjwwag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gbanrvssq.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gqgfktzsk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gssayuzxi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gpdnctovo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gbbztzuyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gkmbupwhf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/grdsuhebd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gdefpvfyn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/givrjoyvc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gebciceqo.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwhepojtz.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/guyvdooav.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gkqwlvhwr.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gwvzyggwm.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjjqxgyvv.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/ghewmxiaa.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmmbfkjsf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gmsothhdy.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gwprkxbnn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gvsjqslai.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gookwigkc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxvophgdr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gfrszypgy.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gmjrqzivq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gggifgtha.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/ghkjwejhy.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gveozunsq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gwuffxqlq.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/geryrwwur.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gpkzcyicp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gjonbbhex.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gfzkwnfrx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gdjszfiij.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/ghfvnqmfo.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gewkzyjtm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gxqzsuves.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggdjjexia.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gvjmvveai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gkkdemldu.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gyshxxgab.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gqclnchtr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gwjyavhlb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/grvapmcfd.sHtML


<!-- 参考信息 -->