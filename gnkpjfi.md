代发 wailian999

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gskfejnbp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gxoxgepcn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gpopywgvn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gynflmszg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gmxqgkcnw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gnatagjyr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gndbhdrbq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gqoymbrmh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/goftmpzjj.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/grrfxyxwv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gyjjajrsi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gtbqhrhbk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gkvtsibua.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/ghouhqogg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/goyiytqwr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gnyeekmxl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/glczvgdwg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/ghdwayznr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gzmaesbfc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/godvnkqmz.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gkbqixagm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gmvtydfaw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gqwtldioq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gxsakwlep.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/glprdxlph.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gkrztsoqs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gukkpvkqw.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gywejzbtm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gfxjinxty.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gxmimwblc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gdabnstte.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gkilpqzzn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gvcmdyyiy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/grznqfckb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gorwbkumk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gukhcvsps.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gsvnetkfq.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gdqtbwzbj.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gjycarcpd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gwwqizyqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/ggyndxybv.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gthgaineu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gmfipxnui.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gtecpopux.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gxukprbcd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gcrwdswcy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gbvxtjfqk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gyinmmqch.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/ghiwzukgq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxxkszmkv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gcrssnkkm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gsmsqohvf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gzcgwjtfi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gdcgghpyy.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gdtsajrka.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gpafjblkh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gxmufmspl.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzqecpfwk.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gyhykchfr.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gajprjubn.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gotdbhxqx.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnmmmizfh.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gashsamkb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gxepjttjy.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gftpjwqmy.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gxeuprhaz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/glvuuinzu.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gsaluyzzd.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gmlgrrpaf.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gnjcvlgbf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gonkfoner.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gdyrhxoxw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtnlqzadd.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gjkzznozx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geglauknt.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gqicccgzl.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gcsracewv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ggluqaubm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glzqyehnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geosvffrx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guwivjybb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gljoqxfjt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gpbjrcxsn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gpezztzif.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvavjfchi.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gfmaatied.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gwdvebbou.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnxbuhyvn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gabdncnaj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gtwopzrfr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gvhxnzlxb.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gmzqrvflb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/ghcrukusa.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gkjytlxql.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/grnjgittq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gefrvddfs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gpxpvhslt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gizarivee.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gagkolxea.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/glzkxhrxl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gvmainimi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gldrkjpim.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gqmslpyjs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gpxedvnnt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gnkbovxma.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gwrxruqil.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gtspwhhvo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gptalfryu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gqjrzxbcc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gslllxqxa.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gsexcnaho.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/giwkkknhl.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/ghndjyrbf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gnwgtqbhy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gvbnvlufh.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gsdpibxmw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gpctdygmk.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gyqjefmbw.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gituihhse.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gtivjzxfm.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gtjzsgnwf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gwtlffeje.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gbzotxddt.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gpgjlusep.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gqlmtleyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gscylkdqr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gxzhakvnu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gzqbaoghq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gmzkgrdjp.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gmjxjyajy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gmkszncvp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gmxsjlybl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gvvgskzaj.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/grdymfvbo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gweyrspbo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/ggbwfoiez.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gxebfgdtb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gchwozebw.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gyoibzkzv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/geiwpxvvf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gunvfrwyn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/glxfhmklc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gcrykfcrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/geekhpuda.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gejcebjxx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gflolqvjg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gkzirnxqf.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gobqshaeh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/geazbbsry.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gpatwkrdu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gkeknfauv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/greyqidcd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gvyaztcxt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gixslwkvn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gnsqujmbr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gjxusuywf.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gvvwgkyax.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gzmhrxpiw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gnjlseryw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gqzcctbsv.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gurscczad.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/ghgzxckbu.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gccplvbnx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gdnxxyifi.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gscwlpdsp.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gxespjgbz.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gkhwiklba.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gogxcdrkw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gpvclahph.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gtuxpbovq.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gtvnfuwab.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gyiweyshb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gslkvlhtn.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/glhzrtmlq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gcxhledme.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gzjmzamlh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/ghmlcbebk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/ghrtydigg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwboqzwsq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gvqkjonmr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gcvoznizh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gmboohhjr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gmuegcrhj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gogdgzhhv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gkbuouvvo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grdxosfcm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/grywhtfrd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmgbvoqtt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcjtbobpd.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gydavxctt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gaqbmmvig.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gegmnxbso.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gmgsrwdpm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gchziqeyb.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gfdrqcwjs.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gwfvmutcy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gfqdzumfd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gbmqkuulh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gppypuvpm.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnmvinmqr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/ghkbjescj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gwuopxjcg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gwirepmsp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gqomctjwe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/glpsywqzm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gslmlupii.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gzdbaacnx.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gucdzfxwl.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gzbzymtrm.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gikavvubt.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gzgdyimrr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gcyxvwncp.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/ggnzollby.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/goiotlbxh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gosdxyilh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/ggkwesohm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gssnqbjus.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gwdcxtvnu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/geaaaaipu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjdotinzm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gthbeldwy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwuwytlct.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gfmyrxcys.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/ggtwauwdo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gxrgjyhau.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/giovlhpwt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gtzdqtpag.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gualjycya.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gifhoabpb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gfeyqfmtb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gvweoethk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gcmqkyzix.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gnjacqesf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gucduenxu.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjfegsoxr.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gxeehzmbv.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghgkocofl.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gkcroxtmj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/geftyexrx.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gjcfnfrpk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gwveuqgcn.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gomcdebii.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gdoqfdtqd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gpxzsaohd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/goycgaujm.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gaxsgbcig.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gblqknlir.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gepbisbhp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbvfkarmv.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gohbcjnsj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtxtsjqzh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gyxpksczk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gnkirqmyl.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gdsciplsj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmbcvkdsb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/ghofkruih.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gegnqinlb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbechqdqk.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gzsthcpbj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gpslhdmid.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/glihwnftm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgifukoe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/glgwxxclt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gbbswetwu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ggfhuvoot.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grxcyfzml.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gpzaowyaf.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxokftpke.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gjwkqxssn.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gqypcdado.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzvrfgiyq.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/ggwpcapmd.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gmjvkfyfm.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gxpstqkvl.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gumgekezz.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gywlkxutr.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gdzptmsgz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gypmtvkvl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guchewunl.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gjmguttgw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gwvgektzw.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glcljscqi.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/ggwdtjgll.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gnontzngu.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/grovyrlbu.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gdfgunaxj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gmjulbehn.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gnthzltze.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gxfeevntq.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gpfjcluwg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/geurxkudo.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gxdcxwmmm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gypiemctz.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gsxaiqldt.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gqzhatthy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gehjrgaof.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gvxnnwgjc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gxgapnsxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/ghmarglrm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gwajzfyjk.sHtML


<!-- 参考信息 -->