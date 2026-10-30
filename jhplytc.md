代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/ggomuuwef.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/goadofgnh.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gxpmpbdum.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gbmpxadhm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gfiiukavz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/golnnlwbm.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gwlhuoxvh.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gzfmqovat.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/glzmymnaa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/geviycrpr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/ghmyczktx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/goljpfqhy.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gdcybotig.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gjcdcmtby.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/glcjqapaj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdnzjocqh.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gvfsdiuxd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gkmqybjth.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gltwktokh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gymgkedxq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gvsmusldi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gbzjpjati.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gmrdolcqk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/ghiizzzor.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gkpgdsvrz.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gainwhpzq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gxusxuzyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gcniltrab.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gmdgjvlts.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gzxmykrdg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/grjupsjse.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/glmlrjybc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/ggivvksnj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/ghgofwhdc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gwyobpqvz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gplgisrxb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gzyciupcc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gphbmnclv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gosmoahbd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gcdlfedfv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gmzywiedp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/ggbxljeop.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gzizxtwjw.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gjwxygbty.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gmpsgitpc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gnidzmuki.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gzxpddssr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gczmgqfji.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/glrsdjmpr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gckaqahbq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gunzllglb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/ghbxlgpba.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gemkzmtnr.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gcabzwwem.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gpqchfcmm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gribyjqdx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/ganaceuin.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gzqdycnjt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gvjiexdro.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gqdbskssm.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gwnyyuaoc.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ggyjercpn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gebakjito.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/guyvpnbpm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gqpmhhzdt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gpmmseisr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/grghidhyt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/ghbreinhg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gynbyyfso.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/grrhmkbgo.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gsnycmkat.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gkkntmfzu.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gsheqvdan.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grlzqqqip.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmvdcolai.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gyxotwsje.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gbwxvzlqy.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gebiswvql.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gupuedhnt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gvazfbolz.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gzoevgsbb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/ghihomcen.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gcsqiaiuv.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/geyrqzwfj.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gmwcnxooy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gsucwytgg.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gizcpqezn.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gxpbhagjo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddfqwwba.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/guxxnjkin.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnygvnscb.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gqorijgoo.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gshuwmcch.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gqlhvjcti.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gcgakbsym.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gduqsuyxx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbutwfmqx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gmsywuqlg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gqrccgaup.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxkacpqf.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrkgfsk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ghnpxuekc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/glerjfpwv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gnobhfkgt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gplzwqezs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gkkuazprk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gnhmslhev.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gwazyyguz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gytkciuqt.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/ggjzojiyy.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gtykqdgix.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gmmppfvup.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gkedlgjbd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gvyddoupj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gwjtewapf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gonaotbgs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gctehpehj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gyxtavklg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gddmsgkfj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gsoxztxxl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gfufdblug.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/ggytitegj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gkdazqwdr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/glgdzwpiu.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gbitmhmuq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqauhunix.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcizlfwkr.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/goxfcbbhw.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gcvpoxwei.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gozapxrzk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gezrynncn.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxzvzpw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gypmkkver.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gniuccfze.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/grnjrjoof.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gwlrlolvl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/garebnzxl.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/ghkfcuadj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gwgjizexy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjjoztfoa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gosrjisxb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtrlbynli.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gfklegyyu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gunasxeer.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gcdmzapnn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gqhhhjdhp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gublgztyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gnoaukztf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/glkpcpxrq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gdrcgduhq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gcoimwcac.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gkqynlymx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gcrzpnrbh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/ggeggijhp.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gqlgduckn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gcdrimzqd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gwdrpcvsr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gilktrlwv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/giqcncqse.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gtvmveipf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gshecurjh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/ggloktroi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gijvtuuwl.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/ggzrkzhys.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtffydgct.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gvgslunqn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gfuuarqxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gykyayyld.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gkymcfoea.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gskcyqpee.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gstfdlbnk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gtnkudbso.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/ggxfjcbdy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gibwxadqo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gvezlbvlk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gactctuqo.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gvssjfrhq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkuchhykx.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gvwingetz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/ghkyjqefk.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gwyflgrxz.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gvbolwgic.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gkzspszwb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gekytxjdz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gpuxzagxm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gdqdeczky.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gzmprcawx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/ghufdgsde.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gluzdjkyz.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/ggrnmdnhb.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/grfewlcba.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gpnjckldc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gpjjjnykd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ggzjwdgns.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gleerqymb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gqyuhthkd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gskrjjnqp.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gonnjztyq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gcdoftdmt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gluszwsih.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/ggijxlmxx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkslitlwb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/ggordgtet.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvqzmesnq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbyiiwbjg.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gwychkkin.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gdtbhnrih.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gbnsneglp.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/grggqxerl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/glgcjkuji.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gjjrrdwvj.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gxfsaiqnn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/geoxnkfif.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gerqiooyz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gixroaobr.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gyxivgumw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gglyjoiqv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gnrisdzoy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gozplcyae.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gtzcmifuf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gexzodfou.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gbrasomqp.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gmylgsftv.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gobxgkfxe.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gbryldcpt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/ghljqqjew.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/guqfdcfmm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gfvkptquy.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gvbydjgba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gszwkermq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gbviwfcnt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gdktkquzc.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gznonobgl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gzhbabbye.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gduyaibwk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gguxgexnc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gyshwurxm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gauuyhsss.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/goilqmtjs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gzipcjjjx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gtgyxtlrs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gjcosjbzq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gfopxzlhc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gzqoslcrw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gbpfxelnf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gibukttra.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gvihhxvmx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/ggkfpidhk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gzoujrlrk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gehbtymxq.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gmpsjaped.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/glhzonysw.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/giofenvyo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbjtwhudf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gsknkojfu.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gteytabnk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gewwucmaj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gebsyfcdf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gwkqwdfhw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/ghkvtrmfw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqwrbzlgn.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gxtncrvwt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gcgiwcsuf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/grixigqdh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gywhmvwyd.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/guyybblfu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gprbyibwj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqafusrm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gocgeoctk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gtuchgjnb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ggzbwirgc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gcjyzdlse.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/guwkesjag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gnaszefuj.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gebblgbdp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gokljeahn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gkxkrcsuq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/glgmcrqew.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gndjxjjns.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/graufhsxm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gqtovimem.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gavpryrer.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gkxnqoojf.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gxuntnnnz.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ghqadwnli.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gzykpupog.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gnflapzgv.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gclcutmss.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gfedyhfzw.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gkevbtudc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gsgjgbplm.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gzyhlvfjb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gafxqfoef.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gsxlpsoty.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/galychlqd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/grxmyssdh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gebwnqvmk.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gepvghrqn.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gsdvphhwm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gvrofileu.sHtML


<!-- 参考信息 -->