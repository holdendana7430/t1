代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gkfnqhrrp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gsrxotwni.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gvigghyip.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/guroigehj.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gnoodbmsc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gcvktzyla.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gbrvnciqh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gxelumsgh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gkivyitua.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnrohrudu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gescahxvq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gysqzgopt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gcktfcljn.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gugrpezef.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gleoyauhh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gnwutxsyv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gveiabcof.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gbstkorhk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gsnjzgotw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gvcbtcnim.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gajwhqwlx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gxdfbgzky.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gdzsgeekk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gliyfvdxq.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gfzudsbil.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gtpjwzdht.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gcuocrqzv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gexjmlvjr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gaoqmgcuv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gxqtmstks.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/giotpunnd.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/ghfnszjoj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/grtjfwatx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gkndcrpjb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gzxuuoiez.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gtgxmaauu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/giuszrvtp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gdypsryya.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gxvgwoblj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/geuyffsgt.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gomlylqqk.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gvzozoqwn.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gyjgrsufq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gqnvcubls.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gkysnplze.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gzfghszss.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/guxjvsaei.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gmindibbp.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gnqvhryix.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ghelppeeo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gglopodql.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/geozoohap.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gyxzqxjvd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gyxfwrcrt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gkwiuzafs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdujmblbn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/ghsitgssd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gxxhnyaer.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gidilmluq.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gyodzsioj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/ghmstylfj.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/godrlsqlk.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfjdsrgja.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gaqlobtkg.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqmgsgjin.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gqvnglcac.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gftrgfxmh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gwbirnvdt.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gplvgkxgs.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gbdwurtbu.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gqdreoaqp.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/grsxhaifg.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gulumvnfz.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gbxkhvhvj.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gafhqndpc.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gfnqsrpkz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfxkevwnl.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/guqkjavee.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdnloeqen.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghtquxeyy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gzbuinmyz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvdtxjvbr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdcjyzkot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gmhkyqzei.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjbdfcnu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/guwgvlizq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gspmxyjif.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnhczcqtw.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gesywyfok.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gzudxsxnq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gtvdolcos.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwpgdjnlp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gtjedukis.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gclusnbnp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gdlxooxhx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gydyheomk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gomkkmrjo.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/guggnsrfs.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/grzqsgimo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gkrmjkzne.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gfqqkbpsf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gghnpbvhw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtevmytku.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/glikzmurc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gvbaabvll.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gpkvhiueg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gvrvjeyhq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gysdkkkdp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/guswyuabi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gucpvdgct.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/grbdrmvjo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gdfpuwkrz.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gadgzvhfn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gshowkvyu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gxqstmovz.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/glcfrnerv.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/ghwlnitbn.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gaijeovkx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/ghpmwibvh.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gsugwzezs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gwefzytpt.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gzbojgpjv.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/geutpzqiv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gfuermocc.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gfkkpykio.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gnajnhvwg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gsvogvnvn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gicamdsjl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gldrzpoae.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/goaadqjcm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gayurfzpc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gfhjohcss.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzyffnzew.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gdopeyslh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gicwreler.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gtxqyamng.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gfxqmkdwp.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gbniiiauc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/geabumdhs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/ghgcsgqtj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gnttggbin.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gvgmcpuaq.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gwfjnkfjs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gvfxgbtkj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gkqdsvtdm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gipripvdo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gzwhfkrzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gzrqfmlao.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gtlvtvuyw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gltmbisje.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gzomjsrei.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gwtaehocm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/grblwrsto.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gqgmrxsjz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gdxnphoah.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gcsyaomry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gjvgjpyot.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gofnqknsg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gbdvjnszc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gwdowwxlk.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gajnnbmhg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gsyxxhonv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gfmtkyhxf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gteyzqfie.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gutkohuzo.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gfrgiajtk.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gxzmckysa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gekipabjd.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gcdnfucha.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gqpibdkxm.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/glzvauwyy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gjhpgluem.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gkavnzows.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/guavconzn.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gozfwazwa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gktvqhito.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gosyzpgin.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gzszphivm.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gwlgmcvtq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/godvpeabb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/glxpxbtqi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gkzllnaai.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gjkodnulq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/geieussjh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gmrwugkhx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gidvqscim.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gctssnndy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gzrjtebty.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/genarixsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gurercekc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gmpblvtxo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gminebtyh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdpgvpuil.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gxzkrinhj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gtfdejcdx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gakttqggb.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gvldhzvfp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gefdztgkf.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gxaxzrugs.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/grucdetnc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gxhjcdvja.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gqwtbvfdy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gmlwilblc.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gakppdzal.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/giogyywfa.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gdvjhyjsw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gsldnmyye.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/ggyzhmjwn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvzxmyekr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxwjzfqaq.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gzhchyzgw.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gyhftaprf.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/grblhiveq.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gzaplvyju.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gbapowgfp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gkcumvrik.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gcjiadekz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gznwsuyeu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gsusvgowp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gxsvxggvj.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gubkcbvor.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gxlpuivsu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gdqznxxao.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbaoccrhg.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/glhndcazu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpvlcgxaa.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gysqtdwqd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gttxqijtj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ghwnlybxh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gzwjsuwon.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gvutrkixt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gsnzkskau.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/glmhfqvmb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/glpflajth.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/grvvyibsj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gyvyuntlc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gfmxjagbf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gumxgheem.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glrvjadba.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gcaizqslf.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gljzozoud.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gktsypkud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/ghnsdjfry.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gopxsokzt.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gequmcorq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/grzreahva.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gtyqtcrnc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gfwgiqkgo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpmhqmvqa.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggbtxxono.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gqbjhokbh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gfzfasjet.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbbnvbioq.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gwxxjrjws.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gcwnkpkwf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/ghlppbcmi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gnrcfuqjx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/guujjketq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/ghhfkskzd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gttqorrhg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/glbxvtbjs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gytcrermd.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/ghirobzso.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/grtadhwdl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gtyhvbnom.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gfqxbhhht.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gzunzclcu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gpsgakcwc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gxgpitqlf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/grlkvwwrh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqhcvtsgv.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gesqpqwjb.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpmgkttfb.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghvpiizze.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gpenhuqyv.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gsrumcvlg.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gkuciswzi.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjmpjmraa.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gcbcwartj.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gdyaaalfb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gyaashjwn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gbfqrdxuy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gelflqvkb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvrkwruzx.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gsyynbsey.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gidnmiiwf.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gsspsysti.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gopdcdeas.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvreemqzg.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gylemorra.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gypdzjckm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/ggnwqqequ.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/grpthqvlw.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gqeogbsqf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/geirmjcbs.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gznmfianp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gtmanzpsp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxatjflsj.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gtybchcsy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gonuhtjrg.sHtML


<!-- 参考信息 -->