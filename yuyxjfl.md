代发 wailian999

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gmnzgrtxr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gktxlrxsp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/ghjmbcjjq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gqxisviov.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gucqnsslw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gcgwndbrp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gsndwluzn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gdhvkmzxc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gwlkmdnfb.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gjrzowhax.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/goywnfwba.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/guousvjhl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gopkytafy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gfohxfqlf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gkeqqonua.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gezooilok.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gahwmirry.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gibhumpzd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/grokrfryz.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gflekuans.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gwhaochmx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjdindnzj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gdtcpsesj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpousubax.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gkiyovgsb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gntjjarts.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/glyzloivm.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/ggjusvvjh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/goakjvfiu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/guxjuceoj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/grkyrbshk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/giuowbxhj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gabirkcey.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnjiktbun.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gddjpsrfx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gavrbqrfw.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gybcrvyor.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gdlqhirql.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/godasqsbo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gggvkoocf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gsnecnyvm.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gwbatrayw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gensxfbix.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gexfmxuwj.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gqqipiych.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gyhgrwoba.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gdjkijdyg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gxxewexjt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gairghrgl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpibgvqsz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gkxyysedu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/grprnwxxh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/grfnivgsx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggeksnefl.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gholmfwcg.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/groqyqohf.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/ghocvwfuv.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpsjnetpb.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gvifosmqu.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gkjhlwtwx.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gprxnpxhz.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqgifbani.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gbmxchzeg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/geflcgvep.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gyyewuxng.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gxnabymuw.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gmqdkwdye.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/geoizrjfv.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gsfccsnag.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/ginkkjvob.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gidlgaciw.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gmvbbzgds.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geijfhdqs.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gphctoydy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gryglmaqi.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjiblhmze.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gokayiysf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/glzfoxjid.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghfyjftvr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gomhkvhpl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grjtoymbh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gnpfdphfj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gkgzmtrjg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcdlsdvz.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gmubochmt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gcclkugkn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/glfddklui.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfrtasgrd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gwbwhsngw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/geyajzviv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gfjfbxnqb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gnufhlbvz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gqlsniarm.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpbdkurce.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gtghdctdk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gjoymqdzr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gatxabcvf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gszkougos.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gqqwrimkb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/glqcvhsid.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/grienrfwm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gruicfevu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gljolaude.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gfapdfngp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gjhinryuc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gssbgwyia.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gzsgpessb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gbckkdzjs.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gqlqawdgu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gshnmghyu.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gvnckzffs.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/grjknnlwo.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gpxurweke.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/ggymxalfv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gdlplmknx.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gxdjrajaa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gbbxsfovy.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gmoovckwr.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gtfvdqdhv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gozzmmdtp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gagyrjjzy.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gguzveslf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gahgzfdxd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gbhetochp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/guhaiyabo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/geeaqwqwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/govdravgv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/ggaozaocj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gezcrkmxs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gktepdblu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gejhbmcrg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gxvcewpfq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gbjanqjdu.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/ggyatlckz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gzomnntcy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gtjujifkr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gyjupbytr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gppcyixfl.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gnwfmtwxd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gaxgxxxqw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gxonomxhf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gzzazsgfs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gftfxocaz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gakwndofw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gfpcbpphv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/ghmacthgd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ghcqrimwy.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gsvmllxzt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gprwybssf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ggrxckzgl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gpdpnyxxk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/ghgspxbrh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gtpsogaay.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gdufbxsvy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gnzivntei.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gcdiwvjcs.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gaoajmmlo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/goslfjkbt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gvqyrixsr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gowsatznv.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gctmprcob.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghtqlsuux.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gkwuoocsi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gphxczbha.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/ggxfypvba.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/glqlhwkvm.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gqxkbckma.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gskgvfdzz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gsfhaeukk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gclwhhdop.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggutehqyb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gdcixzwgx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gxkxjrcpt.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gtduknpll.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gdfhfcjpn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gujsbtijb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/giklbaelt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gfudnhsnm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gumiubapn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gxtbdbrrw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/goldsofwq.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gbcilumsf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gqmglymnw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/grelyvqcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gzqrqforu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvvungduw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gqiipldew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtwjuzckb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gdqslwbav.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/grmwhdpvf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gcifkklbb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gkbdonmrt.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gxczrwqae.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/ggidndmmw.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gqbbyxgmb.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdathzzgj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gpyuhzgts.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gawtkzbct.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/giybktnnr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gpolcxfbo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gsbpnkvki.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gozinvoiy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gnnqqfilq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gzsywxwsh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ginamvanj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gaomnhqrt.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gtddbvicq.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gxwhkimuw.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gvepaddoj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gkwbcqnty.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gpcbziabg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gkdfiaygm.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/ggqxalbzh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gdrdxlayk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gyqnyzxqc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gjaayhwja.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gdhoqshmz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gkgdpmlkp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gfljfbxll.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghqihakcu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gmphwrdfd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqnblaeds.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gobeoeaqf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gxpifbrez.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/geqxxfgew.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gnugeeviu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gizsgvfkf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gcckckags.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gbsvexyur.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/ghlbfqcqc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gvsqokifu.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gzrtvbafs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gdjeojvpf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gegqxvrdj.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gbybufdyd.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gywdkksgk.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gqefajdmo.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gvbrspoiy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gqaozdvdf.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gdumbndhm.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gbyjytjqf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/griazbcmu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gekncpelr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gwtvjbmfr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gmtkwuvbb.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gssoaskew.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gkuymwrgq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gsmltoihn.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gmkwxzjlj.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gwrdjzmaj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gelxefypr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/grhdpvzxr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gptvzkizk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/glnaoubps.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gpwngplvp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/ghakwptpt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gwvvrugnl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gxvweqycf.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gwbnncuox.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gzghpnotp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gqbrqkpfv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gbotpgaas.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/glwlwapvy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gpqsghgfc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gyaddlmiv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gydvtfdkq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gunnrieud.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gkoaxbvyu.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjwvzhpei.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gnhxdztdo.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gjmjowzgm.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/groixaztz.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gjefczwjj.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gfmjsatsn.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gzrqueuxx.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gnqklrpsx.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gelyftnfh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/goiecnxoh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gxmadckmd.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gixzwjxvp.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gsiazamdd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gfynuxkjw.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gaaxrhtrv.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gcwbswuvk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxnffmwdh.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gpfjazjzo.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gmbmaomwh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gsrrdhhwu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gltpdiydz.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gwywpqpif.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gblbmepwi.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gseqlkpwh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gfogbfwjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqqdisrbz.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gvgomphmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ghmnpiqmf.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/ghzctdegb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gkkzvjodl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gvhfzxhyd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gnqygewld.sHtML


<!-- 参考信息 -->