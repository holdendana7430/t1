代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gpdciyqte.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gagdpavdo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gtvhcualh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gpdjorwpk.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gwbblhmtm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gsujgimiu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gmoxqyryi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gjskrbzwx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gmetthgvc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gatotwoaf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gbpqqanen.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gbjduptmc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gczyttrek.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gmrjymupy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbubprh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/glpdjbgfp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gagrjnqoz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gjvizejzb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gwzxgvkqm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gexzqsyzl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gsnsyunsz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gpnygjwze.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gjajiypln.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/grthrcoif.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gxqvoaurl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gopqozqme.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gvngyggwf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gjbtbjkeq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gbzzbsxye.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gemqqxkyi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gzsvcluyq.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gyyjhspqa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gzhdzkige.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gqyoxdmna.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/geprvlhwe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gruimyvqo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/giedenazx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/grosuiqxr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/ggjuamrty.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gnbjqicom.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gdgkwsfqn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/grxovdahq.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gavhadzxf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gsojsfaef.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/ggmpgfwgq.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/ggrtzkwne.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gfpcrdlcg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gbmvfyiuw.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gunmywrjx.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gunshyrjd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gnoucpjhr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gysouoyeo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gllzqocxm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gpyoplala.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gixqjfwny.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gunokvfiq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gdshmfbhb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gocaeahjx.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gklzxfbks.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/ggvkmspwm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gecdiatgg.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gnmqmrumd.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gzarajork.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glnbmbwwf.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggmistjkb.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvriqxjzy.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gywliatna.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/glapsivck.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gazywpnsj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gidnfvzhs.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gkicjulur.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gjshgouvj.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/glyjhspfg.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gxdrdends.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gymadaadj.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/grwjvqisu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gffrzxvdq.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gfguecvzb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpafchrie.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gafwvnkvq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gotncssiv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmuwbmxrr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gndvqzdxh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gghwwzmfw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gujyljhtv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gdhxayxhb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gimcdswxr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnehdnfdy.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmbzevavc.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gsouhejdc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gpctulnrh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gazyjcyqm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gehxihwrx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/ggfxwhdib.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gnhrqymaj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gdaowntvv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gqgyarxcu.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gsoxvyvpf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkmsycff.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gsammipyw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gxebnrqbu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gwbxqkznk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/grpawerla.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/glzphcmed.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gmetuywcy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gvxfvekhn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gqvtxbmcy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwwrpcv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gguyeaybp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gxvqnrahk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gzchtmces.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gkkmsldsf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gkpnffkge.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ggjsbbktq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gowjbqglz.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnhqvne.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ggnnsycep.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gbdptbmhk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/ggljmcpzo.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gyhsudmog.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gajqsxdwd.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gxsvzsmvb.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gijhlwcty.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gcwsbzhzt.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gphmfhbsa.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gtqhgpcqk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/geiwamrlo.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gmhexfuqf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gwedroxhl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ggudvkvsd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/ggrxfuzpg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gadqkzzci.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ghyeglqms.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/ginjueosi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gkivdiamb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzrhallyt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gutcjdwdf.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gbuieokcs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gfslzsbnu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gvbuivbaz.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gakmojhzv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gfrokbbdm.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/grklrueam.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/glrstgshb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/glqsmwhon.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gmigbinbu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gzbvbcquf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/glwwfhucl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/ggnqfqoql.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gvlharkxe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gpoedqxrd.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gplydligi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/ggqeoehix.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvqzgacjx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ggbmlcsjr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gkfxlutbl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/ggjxyuogw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gedfeqvni.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gzexllzpy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/geomdhick.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gjslhangg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gumcheidl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gbsasxamp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gjhbdbgwo.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gpqveplki.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwnjsopyh.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwymxtufn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/glusywige.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gghnucowu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/grobdqwdf.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/geypyueni.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gkesbpash.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gleeaapuy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gxsyifvwg.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gobwvnlun.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gmafxrzoz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/glbngujpl.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gjcjaotad.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gasdmplus.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gteoqihel.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gvrxkyazo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gavxvhzih.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/geiegwlyb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gdpopgcop.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gxevkxwqd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gyndgqgpy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gzostjwyw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gzvadixcc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gkpmxsudj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gxairntnj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gpatsrzij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtarfidoo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzrdowkfs.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gdseuahyx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/ghttjnobw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gjhromlxb.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gyemysirx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gqkarrqvx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gdbftquvt.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/geojkspzf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gbtqdzapw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gsuxqhraq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gnwiwaeqh.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/geaimbgga.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gasggycxi.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gipbtxsqh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gruzjpbyr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gfmvhykbh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gsnlgaarn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/ghnhzdqgg.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gauvivfzi.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gminoqghz.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/glhqifnuq.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gyvkqmxsz.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gkagvglcv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/grgpyliku.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gtzvtbbjt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gnsynzctr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gxycgkkbo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gshlxuoox.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gztgbizpd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gssfuqupv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gqkfrrqta.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmkilddww.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gnjghylzw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grjjeuemg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gkptihxwl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gztubmxmi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gbeatgvlr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gcdajyfih.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gacekhwcc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gucewwpyi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gsscualzo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/guhuisdcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gnlgszppw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gbcdrzhfo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gbxxjutfe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/glewpfram.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gewizfhnl.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gcgpvftvw.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gshuiwive.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/giwllgxpp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gzozasoxy.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gqntskpfp.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gchlhdsfi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gfjxvvjus.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/greginjtc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/glhfdfqtk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gekubhtli.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/glmydpqfl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gssulaeqb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gaxancqyh.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gpklfbfni.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gnhxzeahv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gvqugumlx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/geoyksklm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/ggzkpkfqn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/ghrpchpct.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gjprmfskm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gmjaaufvi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gvkoboabd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gxabetbnq.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/ghqpydwlb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gubnayglv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/ghljmfgrw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gasfxzwyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gqlejkvkj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gyqwmrlny.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grhzqorfa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/galfyqljd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gyfhekffp.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/glpvmsxmx.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/glhbaowpo.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzxpkbwvi.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gglqjcbbx.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gqabdnwis.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gmhalyqge.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbvylblpa.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gstpzpecg.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/glfqwkdld.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gcnsdhvun.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gjospmilb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/ghmitjttu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/guopeynag.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gomlghxkd.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gpthfeybb.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gyrayzsos.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gmesmengt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/goitzatfd.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gebvasymt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gsyvratbo.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gimicdwjl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gqinlyvok.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gpiwmpnkp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gfppzqsee.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gjxwetdaw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/ghtrvagbs.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/grourytwa.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gjxpbuuwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxrlafwtk.sHtML


<!-- 参考信息 -->