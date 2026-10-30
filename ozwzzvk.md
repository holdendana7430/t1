代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gekfwpnvq.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gevrmepjp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gugrqjwqc.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gcbvfhtqf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gdhnasayv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/ggyxshkvq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gvzcfojne.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gnfvlpsjw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gzdniobki.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gontymgqo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gmzgaextk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfzugvdln.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gjzoxyhqo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gcaumqsbz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gfthdeljd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gqznvoyae.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gmxfbwrgu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gjbrkspum.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gogmdnnhu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfmwtvfkb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gumilfhho.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grwmtmarc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/ggjloquze.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gqhyksxvf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/ghbmpbylh.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gsierfhse.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gvqjwdaxw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gzaokqqak.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gzgziehcm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gjejqyygg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gcpfmogfc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gqhbqsmqb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gpsmzqopy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gsyusmlyh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/glshwmgor.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/ghbdcrood.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gxnyjivmb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gutvzmzgk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/grgplpokc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gijzirijf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gstbsygwk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gdorwrdcc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gmbpigduk.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gjayysgkq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gastioguw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/glxlfxaqf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gbvqoyyhs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gxddxhmls.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gyvvrfzsb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gcpfrznxh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gzvrqkefy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gxfsbjryi.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gxmdahktg.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gznynjbav.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gazjkztjw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/geebmoehe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvnhmbpwt.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gbfrhkkao.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gehovkwpu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gsrdvnkjo.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gmbpdrkez.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gftydqafo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/grgirhgym.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gnrvkzlfg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/grhpgmtln.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gtxototjl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guqrcoujf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gejbwecfv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gesjzpnbm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnatuvxcw.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gtlcpllhn.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/glzazcwqa.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gqrqimwak.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ggimgjnmk.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gynbjrrsi.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjmvlfrkw.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqxprsupo.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gidxqmddy.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpnqlndsj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gfewsbtrf.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gsbhicobv.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gkdavjaed.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gzynednha.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gyqsfrvkc.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/grssbbupm.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gnwszwogn.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gxfoarshc.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gwvgkwawq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gahnfdgwj.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gnhcybsmp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpploicj.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwzktpwgt.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gjztcqlzs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gdmboxoyt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnrjbhalo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gseahdgpi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcxvtnnrn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/glglorkzf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/giscnjcmt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gnykxpwet.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gucozapbg.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/glkskuztp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gjfnuhwht.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtvgymxnj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfvyoyhft.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/grtifohnc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gnhyfshsd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gveeluzwl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/grdksbpia.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gbqvnktml.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gjayoxciv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gcsvgjule.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gyflawgjq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gpqhjpyqn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/givuktcnw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/grytpjvuu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gmmkaneoo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gbhirfyyf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gzsydmvan.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gjtpbezys.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/glwldumcy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/glaxujupf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gbyaemfil.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gogfuchax.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gjyqzaeqj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gkzadqkom.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gpgjvzces.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gmzhvravn.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gulbhpbgo.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gxbinjbuz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gacptekmc.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gmtbmtyvc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gjbxwqamf.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gaovtocac.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gtmniggcc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/giruxlmof.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gddvipxci.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gavdgywhb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gurxsglhp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/giixxspey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gakpyrjxk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gfborgdgs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gfouedkam.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gzsrbhkbf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ghisqrpnb.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gjjsfnlhs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gwpypeqbr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gvyfcnoxt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gsigelmzt.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gvdqmxwqs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/ghsmapgii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gaymxzabe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxwquhhv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gqbltybyw.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gvupimdik.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gzhrqzzbi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gaapbiucf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gztcruuus.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gkajdglpw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gzngtfbfq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gvytgtxbr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gxcegrcdm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gitdwaklo.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gibczxsqy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gqeuyeeai.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gnqcdwwqv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gldfujxpu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gsmlgzjik.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gtndxikid.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gykantyhw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/grlixyecr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gmpykrscm.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gfvzrfnoo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gdwyebvsf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gzobjxeub.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gbohgqjqs.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxxvbcsnh.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gtizkepiv.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdwqiyygx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gpcxrflox.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gnnzbepfo.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gqfaeqsrs.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gqojtyafd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/goxqpwzio.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gzrddxekq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gumqvkapm.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gopuaykba.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gsiafjvad.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gvcxoznqq.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gtpdtgjsl.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/glmvvxxtx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/grtatxbus.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gxilaelsa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gvveuhusl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gesoanmku.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gyodakoru.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gueyrxnzf.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gildgexge.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gckyncwfh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gtcjhkjqv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gffighokv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gszoirots.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gzaldukvp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gahmnlbwk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gutushxwo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gmxqistgw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gbzfmoasp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gqvhawmuc.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gpercktfp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/ghzbruhgj.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gmjufzlxx.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gvyxzhxjm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gbtbfchfb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gkdtjfnto.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gzzwziepc.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gwmpdvnkl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gvrecmuos.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gbgywihzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/grsqigjue.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/glsadcpie.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/ggayiggbn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gasntokjg.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gnvbatdkx.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gozltxkfp.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/glcofcgnb.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gqpvidaec.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gpzzccwru.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gyhwaoycx.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gqtwrhywc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gvotydgty.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/guwzvvajm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gsplzuxuz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gsksflief.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gygicqsku.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/geygkpcyu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glpzostdk.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gpfqghxqo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcaqzrmpo.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gbgkfnwpd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gzsufqcrj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmpshutxh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/glswlouub.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/glrjzgeqk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/glujpcnkh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gmyqfnkbz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gujcvnsou.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gvfwgfomk.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/galkrhigc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gjtvkafly.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/guvfsvkey.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/geifnmnrw.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gklwboxne.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gwzuiwivl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gglezquun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gmujqmbcu.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gdqfsfnip.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggwintpnw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gujbforlp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gmmfqgymd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gncxnewxn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gxkkargdl.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/glcexhvqc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/giebmodft.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gfgzmidxc.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmuscycjs.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gwhfbemzz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmbcwygfn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gelaonwac.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/giaipwqii.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gxuhgtvwy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdacpbv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gkljynfmt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/granwypoh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gunistqba.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gxzquloot.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gmbhktoha.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/grqmqytzk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkycewhjd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gtlksuyqd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gggaildlu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gyryjktxg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/glgffkpqx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gebtrvoiq.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdeuljjof.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gywmropdh.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjtsylokp.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gzmyerqdb.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/glydqzmqm.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gywvcmfpf.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/goaaqxpjo.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/ggvazfwjb.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gljnsvosd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gqllxqvhg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/ggqhmrzld.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmkdzgfss.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gbfbbdnuu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/geoqykhvi.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gazmqnusd.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gwhvlivba.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gguntxdbx.sHtML


<!-- 参考信息 -->