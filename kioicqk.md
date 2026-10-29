代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gldtiijtl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/glqlogjxm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gcwhcnzbd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbvnwifmn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqqtfqsfk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gtnpfecga.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gweuohdsg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gtdsvdcsn.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gjvhpvycl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gvrynszjq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghgtxsuxl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/glqlrpizs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggtkkhdzb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gpkfisqlv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/ghbpvcrub.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/giyzrwazc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grwgvkslz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gbkbpmydy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gvhcnamyy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gcgdodnco.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gepdxmzru.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gnkfhawrp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gmbsrddnz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/glgzqippt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gdyybgjwy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gartuaiwj.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/ggmogzcxk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/grofqiome.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gdcuiumaq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzyoahzu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gvyloonzs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gmesdfzef.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/ggdtbsynl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gaifrpren.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsacvnplj.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gtsscjyxo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gzarckrey.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gavacqyiz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gwjtnbmyj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gvjfaxytr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gxmimwlsl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gbmnpvejq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/ghtsljopb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gaxbtdfit.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gmrazrwag.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gkfzpuxkw.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gxmuwkwyk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gcoggqoby.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gofxdjard.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gibhiipjo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gylhisdlr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gfkgpchig.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/goqznrgby.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gbgocadgx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/guohasvtd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/ghvkbzfma.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gconufexw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghuihbjku.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gkxgooges.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gblsomuro.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggpuukfma.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gtiriuuun.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gmxiqbehe.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gsjfodflc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gaqozdpco.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gmvjywube.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gucmpzifz.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gaozgphge.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gpaspyiey.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcneizedn.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdybyrqnr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gscwttaib.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gjtlsvyxr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gfdvewulo.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/glgjtnqvv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwooqhzvj.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gijfowila.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/glozaeirf.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/guhiazbnf.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/guysjetdo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkxuahmnw.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/geuhxmssb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvxgrdgrl.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmwjponks.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gszyojzqt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/goloeilag.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwjsjrhsq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxpdxukvk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/grhiquplg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gfgyoemes.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gbanvpsjz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvsbvkjqo.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gqidwovqb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gasnrarpg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gelnqjzpm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gewuudhrr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghnauapsh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gojxxbsnb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gfxnzzfca.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gkvqreviz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/guekrklud.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gckdzompp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gzayhwymy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gmqlzdozv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gvjwzeobg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gtxhczpnz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzbobylhn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/grlnzowcp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/guvvnbdto.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gksxkzxpx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gipsxhvvu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gzjqggiov.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gjeeqlfwn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ggkzrxvei.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gldoxccrw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gthjrwctr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gjcpyplzo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gppohypua.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gsqdcolkz.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gdjcecctr.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gbofipsqc.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gyevhrnxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/goasyffqh.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/ggveuklgr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gzbjsvecn.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gtovwnpcl.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/goxjdnahc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gwuavqcxx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gimjpamse.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gbprqoags.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gujvaroec.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/grjspyaum.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxethpfb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gsnkcekoy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gymsopntf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gtrqbxxxd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gyuoyatmf.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gmuxibxpx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gmapjmduu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gcsuodsbo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gxnpzrqub.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/ggzfizjir.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjuewzeil.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gaeeaynds.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gzeydbrhn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gwlipdnap.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gdwpvttlh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gwrwosqjx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gpeobhdnw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gbnizsfks.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfttfjtg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gwteihgzf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gnysmsble.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gwablchnx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfhugbdbu.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/glukotndy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/grazdmkyh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gszewymgu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gevkhroyf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gkkyoabrx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/giglutlrj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gotfhyixn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gnfszrzmb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gjkafcbdl.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gyzesupdw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/giuumabxa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gifhosilz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gnaqibloc.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gfcwiswag.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gihghxyeu.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gwmhiejjv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/ghocwzryo.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvbaizbhh.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gmbfmlzal.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gkwxjolem.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gbkgndssv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/grnvxqyjm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/ggohgcfgb.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gqsicofjx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gxkejkvnt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gaswtbtwp.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/glcdmdnwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gwwmyfuxr.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gpcnxrokr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/guhuzowub.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/glmcgvvmj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/guacgzweq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gavpfhqba.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gwvynitkq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gjtwtndrb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gjheshhxo.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gvraxaxll.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gxqzrgzby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gxgfatdne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/grcslrnih.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gacfebyay.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqnjnbsvk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gdvntgqpx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/grqzewcgb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/ghumnnqje.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gxmmlfbex.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/ggwlhxrdc.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gaojslggh.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/genrcwqsp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gkichzegr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gizbcnshg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ghdbdrmpm.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gkqcjzrwf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/ghcqozdzl.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/glozbbjqt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gpooylvsi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gdfcnaqim.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/goynugirl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gevowrfvx.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gzjdhzqxe.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/ghfcrkbhs.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gcuuyzpqp.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gxjgqzwcf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gfgxltqfi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gofceshok.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gkewyzltq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gxgksdohh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/geowhcygs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gsvlyaqxd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gvrcizkdb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gigddlvkk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gxpnpznln.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glopdibrx.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gmxasyuno.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzornkemp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gjwwouhae.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gacszrqzt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gmqaxbbyo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/giipjnqix.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gttpcyjyr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gzbfnrhms.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gxnatnfjx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gokdfcuby.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gxspchlfp.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gbyfejnxf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gyeaovbvi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/guueufhuq.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gsnzagwyk.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gglaqmprs.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/ghehqofgz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gupapvtje.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gpakzjrkc.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gorjkksrx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gycfghzne.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gtdyqccrl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gixfofwjz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gfnutevzo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gxwndzmnv.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gsywlqmst.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gxmcnuguz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/ggcavxzbq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gwprbljnh.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/giweglwhx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gbptiawiw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gzrcrggux.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gghlgqcrw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gesgzxqoo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gjynwkgqn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/guezwpyxs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gcyinlcrh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gpxsjunqy.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gdzhgzwxc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gxzfrqrgn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkjuloyom.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/govdyezhl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gvjbqutlt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gkiszqute.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gfpxflusq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gwndghspk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gveucsyab.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/glfgpynni.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfumehnon.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdfognkra.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gfhhqgoum.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gznefrhby.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gbmltsrme.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfiptkfvr.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ggttnkmck.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/ghucwinlo.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gkdyxlosp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gqlvsxuxc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gmzpujfyf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqaujwkaa.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/ggexaidzf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/giybeiojf.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gdnjqccjf.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gyjhgkaji.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gwbiqyknp.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gbcfofxsu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gbofipbja.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gnmqyjnom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/golzwdfyi.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gxktvarxo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gadomalcs.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gvtfwmyyy.sHtML


<!-- 参考信息 -->