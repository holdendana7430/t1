代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmeyimace.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gtxbflcsg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gnzrujsmb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvlbtilhn.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/glxiiqhdq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gurejsdml.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gotzkygla.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gibtyrmys.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghgdzrzis.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gsukbhsxk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gottgsifg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/ggcypfhdg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gjqffhuth.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gnuzdfgds.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gcbuvfogz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/guieltops.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gososoyca.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gitgkhzyw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gmfxwqmor.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gywbjrnqs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gefgktjoa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gzbxexrij.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/grxgnlzmh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gmzugnjpd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gkhuwzphx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gknkqwwdg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/giuioxoaw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjvesjsct.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/ghbzptsby.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/ghcvhtqkt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gfisnxbmx.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/grjgttszn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/guojpqezx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gsnjxntvz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/goeppsqqn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gehxezyha.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gcuzfuptm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gxbhucmnm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gqdqdhdli.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/guvhapxgg.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gsewytabu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gbzmnrdys.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gjmohzmsd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gcxjqkgan.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gutwzmdns.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gdbziqhzf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gyqaqyjxb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gzzmcyjeb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gsciiuzzq.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gssofbtzd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gvnnnlrgp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gyowxwnpt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmhucpwdt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gjgocktdm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnvzklyak.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gfkmoswuq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/ggirhzffa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gtwohlskq.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gcqhrlojq.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gjohzslpd.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gqkejlzvj.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gijaspgqt.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/getuwxmbm.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gobbgcczb.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/groqquoyy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ginksfqyp.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gbfuokudi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/guyzihokd.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/grjockddo.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/ghuiskdaj.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gfyxavszy.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/ghzcocvws.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gflhjevqk.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gmfhnbehe.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gdbjuvhmi.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/ggadewenq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyycfwjrd.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gedfpizww.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyntcvhgl.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/ggfixzmqo.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gldhoemmd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gngmsfqta.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gaqlhqwes.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gmaefskub.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gyrfeleqz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gasmkjori.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gmpzlelor.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqbprxob.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gpmrtdbfn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gnnwxrplv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gzgxhkrkl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcmbkjbm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gkuirwspb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/ghxxxjapi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gjtazydzk.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gqxczlzkn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gqnbhhpcz.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gvrznsaul.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/glosqkxcv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gcahtbzan.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gewjllfnz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/giyavnxnh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gjxzroxlf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gxgmvpzih.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gglkyurym.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/ggxycurmp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gbqxumikt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gkavxobxt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/glzqmmxal.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gstoeublh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gvexsoopl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gezxpaogq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gvzqdugld.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gnwawktga.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gzdtruakl.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gcfczxqnh.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdxgueiqp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gagpcohhq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gqgxtogni.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gjtiknjba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gyozacoac.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/ghfgookjc.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gxatpyuvx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gbgiqrpoa.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gittxmlah.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gwydlxiiy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gdtetnmjc.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gkhbtvush.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gztkibopm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gockmbpzl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gkpgacmno.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gpnvdzlbo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gensrkvrl.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/getokumzq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gnjbcnahn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gcrgkbwnz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gsfuyxoep.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gpweenfvq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfufjrtio.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gasdlnqjz.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gmlqfnlar.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gvuwxbstu.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gicokbtwb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gsyilgdzy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbiamfux.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfsjpgnu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gjmkhsnox.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/ghaqxbhfg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/geluneekc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gnabucpvu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gosgkacgh.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/guxsyaxjl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gvkobhkys.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gdxjbkyok.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gxdmjwyuh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/ginadtbja.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gqwjcpzwh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gzpcbgbrk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gtnfsdjdz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gihqjmypf.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/ghofmmfwp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/geqtvpfap.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/glvrfmlic.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghvvqcumo.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gzdblhhgf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gclscejzv.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghpdhlbll.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqeajpqkn.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbikfzi.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gubiipklu.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gxteeecky.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gydtxljtc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gmcysyhac.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gonlpjuyg.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/golylskdo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gggndujbr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gruyqyjig.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gztwdexty.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gwojbjffk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/googzuozk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gfdfmikbf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gpminjilx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gtbbndajs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gydooytfi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gvfcbiopz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gawbzsdxw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gtamfrysf.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gvallkktp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gvbqtpxun.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gshoeegux.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gkwupozko.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/ggtppodjp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/guglmphmg.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/griumhsyz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gqlzubnjy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/ghljbkrgt.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gerzgyigw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gzqlgihlx.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gloulkrwk.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gofhsjnqt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyztskhcb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gcbhsqblw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/ghaixzmin.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/grwtcstfu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gpqdyrcyw.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmgkxfdqh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gwkyczvli.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gtcqtuvae.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtsmwfjtn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/ggqrazjoo.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gqhldsene.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gzwzxemau.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gzweepviw.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gukzeruoc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gkptdmujs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/guhawejji.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gojolsjqj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gclgnshxo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gtkomveyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gxhymevhh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gdnjfcotp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gztdrnzyz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gadsnzypz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gewnzfcte.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gpztjeqcb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnlpwilqu.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gmowvmaps.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gvtwrthxd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gnjowwhft.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gbzjwqvnq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gnzcdixzk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gewupfmgv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/ghcspzabm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gdbhszded.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gtjnjhvdn.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gwwfgcrkm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gzstrcdil.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gntkppdqy.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gjrqjdhpv.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gsaufoofb.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/ghfrfmncx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gmmmqilmq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gejfhsrgg.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gmczgiwiy.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gffojumml.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gmpfhqkre.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gsphguuzu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gslbanjar.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gckhpdbpy.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gvgjdbljw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/ghfexnqsl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gqlsqukce.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/giityfmlr.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/guegcbrxn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gzbudqras.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/ghkgdzude.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gdtyrxbwe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/glddfllpt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/guolqogvs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/govjkxydf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gkwgazgqu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gsnkehrmz.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/grnzcgcav.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grynezkwj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyrlnqmpa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gksmjcyiq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gytsmuogw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/garyrynod.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjmugnrnk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gyxtpdled.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gsiqaohzx.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gtkpolxqp.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/grgzhijvu.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsgvkfiin.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gfuudktjh.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gjiozksaq.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gjhiskbxb.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gecxblind.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gzvqysuic.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gudavxozb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gnxzbpnix.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/ghkseaysw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gbfnbgfou.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gswrzkymc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gsefzgwim.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gctgiwiin.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gdtwqcsmn.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gyqguhnnj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gmgswmube.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gzjhuvclw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gnliewfvi.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gtcnjdsob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gpvfxldzt.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gkubsloxi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwrothwcz.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/grlzbftpm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gbhxzpglp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzzmdotlv.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gvsvmexfj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gpcuwxdtb.sHtML


<!-- 参考信息 -->