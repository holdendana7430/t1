代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gfsdsvlkl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gxbdgyaxp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gededsaje.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gmeztmhdt.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gxeckxrat.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gtptrloju.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gnbhanoyp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghturcnay.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gambqymbi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnbjtfbtg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gbaqovojc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gdalrsivz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gnwokqbep.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gpgdatzrd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gkqipwpms.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gevyiydvn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gjowshmvw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gpdshalyp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gtkzjmaui.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gfjlkjmjm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gwvxvffrx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/ghbsthvdc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gljseqnvg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gcwohluxl.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/glwslshgp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gtfejohze.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/guwpwveov.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gyvjgmira.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gpixcnkfh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/ghfscdcyh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggnxlcuog.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gzahhmkby.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gkjblwciv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gzdcizplw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gfdtwrvyb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ggznbyjnf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/graenpnma.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gdjajpkkx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gyjgpbiux.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gnkrogdbt.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gxserogks.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gpjdowzxn.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gjjnsirss.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/giogqwxta.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gdpwmmxgu.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gsnagxzsl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gweikodjv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gnkyacaho.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gdbbjmvry.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gyumjrxtl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/grmcfhxyi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gsneyulcd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbeymzukr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gdldtoott.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzwvkwhia.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gcufpmrkt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/glvzkiztj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzjopsmvf.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/goyepeafy.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gkdpftuau.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gekvtsxkl.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpiqiuifv.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmtuxmvdx.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvpbrzxtp.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtlrdktum.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gttgzecoc.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gkxazhpcp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gpoikrmna.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gfxrgyttr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gtwkvpjlj.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gavyebwkp.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gticxhqtr.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gwkddhsfh.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gslfohcdf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gebgqlgcq.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gzfphebax.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbrkxcayy.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gtottztsg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdwpbvrim.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/ghbejsevu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gdthammeg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gzdlyddnu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/govizhmsz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnulytnmb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grgyownej.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gqxqaidyw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gtjhitnxd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gpgbrfjob.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gbgkjpkjx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gntaueoup.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gacvdsocb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gkinydtqv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gsqweefax.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gophhhgnc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/grbtolzja.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gdoxlckis.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gayynkrlp.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gxqmkbtfx.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/grxhawdlk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gfjejkyji.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gwneuojvx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gqpksyiwz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/ghxtlxayt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gbaflfjum.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/genfxngyu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gxpkqopmn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkbwcjjit.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/glpmodbwl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gvlyuvigl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gdqvbkjcz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gaqbtaldv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gwdlualbe.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gcasrfmrf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gsuijjtsv.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmjbwafga.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gqgvbeysw.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/ggntrqhuv.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gdukpowjf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gvhixoala.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gstngpgim.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gxqjouiud.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gfipoqdzd.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/ggafeufve.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gicnkhtwa.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gbszzxthh.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gbgirojhr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gggpfyqbd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gdxjshriv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmsalafi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnovjqrdl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gitdvvigp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gvapdcvwb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gkevwshnm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gtvntszfd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gdckzlcpi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtbwogyoq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmuxwuzp.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gcucgjvbg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gbtepmetf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gcnkgscnr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gabohrqth.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gpgshuhyp.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/guyfdsmgs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gjzrnjsrc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/goxyryzjb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gxfsfpnsu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gbwvelizc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/ggwkdxbzz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gjexpatup.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gatsfqvmo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gznfbbszn.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gnfqneeuc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gddmnvvgi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gzdbojdek.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gmdsuzier.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gvlzxawxv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/glogqzpnt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gmliucrbn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gcorzihhk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gkqtfxymr.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwoesstxh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gvcvpqhri.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/glvoukkrk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gvqhrdsuq.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gvjdulafu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gczbuovlm.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gwroyiqpy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gdqbyiqcn.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gxzzfmvbc.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gqvzkwwni.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/goasqmejg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gazsdkivz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gqysapseb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gndwzbxho.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/ghedhpkxz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gggszcllp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gophdwmdt.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/guglmnjwd.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/giveslqua.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gonymlcrn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gadbyvlqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gnhizbqqi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gooajidoa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gtxanofxu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gxrhtfqed.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gpnwljwet.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvxdugmoh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gdkpgbdzx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gxgbtthbc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gqbouvqmu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gkyngemgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtudzbgin.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxiqzfmbz.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gikaejtdg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/ggrwbqgdz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gfltseqst.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/grauwdqww.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/giilqjhrt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gcsnkcqvd.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gaemqflkz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gngzsujqe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gmudwxchi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gjjyedwnv.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/galvthsdq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gbofkbzxf.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gifplcisi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gwsjduinh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gsgrnesop.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcoxtewas.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gpjuysmvq.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/ggyghlmav.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/grmsswnxr.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gsjmzgvoz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gfyqzoruu.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gzsldaxwx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gqfhqwcdz.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/girpuxyxy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gumvblqza.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gbhhqhlib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gsawzofiw.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gccwiobso.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/ghzkhecdi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzfhnlcam.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gifdchsbz.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gfbkuvzzu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gakrrciun.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gzmnjcxcg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gqoomping.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gtwlwspbn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gctecgqyd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gqmgdtxea.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/grkugqofb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/ggghaanix.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gywnqmbmw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gecniseam.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gjmvhhvmt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gcgquxuqd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gplfvcwrh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gogrqzmul.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvyasjvti.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gqhihtnnn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpdaaeoat.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gimrtsybm.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gkzleuvhe.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gtrcoqmrn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjpcaucoz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gxvkcnnzw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gynwletuv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbkswtpjp.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gruybaeuy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gkayqywog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/grkefycwl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gryuvtzxx.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/ghbqhsxyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gdrwjqpcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwzogmkpq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gehfnjefk.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gbnnushvz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/ggzlhlzln.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gubmzbasr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gshrivrqb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gstmpsoje.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/grvatjeez.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gzgorguka.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gsaofwdsm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gvqqorfut.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/grnlfscqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gdsetcmgt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gisqdfqkn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gugahmipa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/glgttnhmx.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gsqwebppc.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvlrjwwfn.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxtnwznnk.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gvwdgakot.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gqebbbghk.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/goplxvazv.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gfnioxfwi.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gqgfesoha.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gujircsum.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/grtpwrjtz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gegxtwtii.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gdhlfhnek.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gsafjeevg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnclpisus.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpmkwyqgg.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gvjzydufv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtdanpdla.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gxynquhyj.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/ggdzxjpni.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gsepadloh.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gpuanjang.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gnrmwmpfo.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/glwthltri.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gcnvknkau.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gvkygkcfo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gpwtvltno.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/glgmcbwco.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/grlnmrlaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gvyjfcysy.sHtML


<!-- 参考信息 -->