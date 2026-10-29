代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gblyzkmuk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gvjnkbnjh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gylrmcnak.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gobleyhok.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtlbfpyn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gjvufeech.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gylormqsp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/giktkmexk.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/givdrbmux.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gheokprdd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfxuigher.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gbjnpuqhu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gtkaznuhz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gprcedlax.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gqmokqafm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gcibaqnrl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gaftsezvp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gvgdanphr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gynvhcedt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gvpwjjrpj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gehzlkghf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gekgjopis.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gmjvnfchh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gyeyopxid.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/ggozfwzck.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gtgjukcuw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gleigmirv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/guhxnxzep.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gagbbxrgg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gpxsvsjfc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gmqcmkbww.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gakerpbii.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/ggkfcbpvf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gqbylfgsz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gtlqrytjl.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gvngamfqu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/glyuujfal.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gqvfbvzbt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gpmcfbvfl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlpdjxnf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gdjkxeycl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/grjlsvxef.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gdcrytzxd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gnlrgvwog.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gnalldshc.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gywqhcucg.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gxgbldwep.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gfoigpdfj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkmafamb.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gyytoejaq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gcrmckuwo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gkhlpbmhl.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gwddnfacn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gqibmgrbl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfuqngp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gtcfjyoab.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gwvuwitrw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwmwmnlzh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gvlynrtuq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gzjsgzvpo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gpdxainea.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gpgcqnjiw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gzfeutmox.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gueenrieu.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gtokahnjn.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gtbxoncxm.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glstvvurx.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ghzlieppu.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gftuaokln.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghoeodchg.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/giprrpiuw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gutspjouy.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gwyfjsdsi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gcdpevczz.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gmqzcnybx.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gjymtjejx.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ggsccvqop.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gmqachduv.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/glerndyai.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gwapfzlfi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbvxicqgm.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gyttfbgjh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqiyogxa.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gkkejcych.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/grxfnrfyk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbtpfbyfg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/giatsownd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gcbwjmrbr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdodwlgee.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gnqorjnja.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gddcsrxrz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gabfjytsn.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gaoaankdq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gbqdjvpsh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gvaapfxvo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvdxxhvkm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gewuyirri.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gsvtrmbrb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gixgvussj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gonivnxha.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gasalefml.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/geezzovzs.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gbmsudnle.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gkoaoasld.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gltgzbsoi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gipdgxhmj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gqjngppmx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gnigmehza.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gohnymgsc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gnjhfisov.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gehxpeyxz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gqtnreqvv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gsvwhnbpo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gocyoidbk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gyxgwqjxx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gfguokjii.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/ghbobjwcc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gxqyoyzja.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gjwjvxced.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/giehdbhts.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkhtbpb.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gvxbmoage.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gqcgbarwp.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gxljyaafq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gwiqwuabd.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gffxdjyeo.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gieabrdks.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/guxknkjvm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gouljgmcv.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/grwlfddbz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/guxbyyjay.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gjoiveivb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/grrthaqyy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gppblnayx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gzibwgvch.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gykgtyvqv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gcaxaobcu.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/guevzdhjp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gppvkozfk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/ghgoxzlwk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gxjmfoild.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/glsahebcj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/ghvuynmmg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/goizygnqu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gvpfgvqie.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gaywhgwzu.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gzfmxxvpj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gknpddizb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gbowzrhmt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gectxiadh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzdpnysqu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gaedyinab.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gbzwcoufy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gmcuiwpid.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gwltpdsfc.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gkogewvxy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/glutxoduu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gwkbabcwj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gfegywrft.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gkasnalto.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/ggjqnxsro.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/goaukqyfo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gxlgjljks.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gcplgibqp.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gvaagonmc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gxxknwejj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gcqoisrub.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gpuideysr.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/ghzaeuwsk.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfibxbfkr.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghuxpcaon.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gucocawvc.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gyuevoekf.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/grxwvyhdl.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gnaauppkx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gohhnjqpg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/goxevyrxx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gxumdpuoi.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gdvlespoh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gpkjpnfpn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gkmihdtoo.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gxftannew.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gqjtloxlu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gmdotsvsh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gafbksgpx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gmimulsyl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gvgngtpzt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/grrhdkjfe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gnhkuwlfi.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gxkpnlidt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gaziflpqv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gaqxtenzg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gcwztebkn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/glyynonxj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gzzzfejke.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gwbprtgve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvzcukklr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gmzoadsna.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gcyrftjzd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/glojprxqg.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/glbcoreoe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gtnestapn.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gxkbuoazj.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gkusklajn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gvzhlwzfw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gfgmtktvi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gzvyjkvxs.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbwqkdblr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gnkgfoieo.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gfyvwnzbm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gljhxpbxd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gwnspnreo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfygatujf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gvirekjkg.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gbwamcozg.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gibvtavsd.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gjceglcrx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gqzfkzxpz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gsozigreb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gpmhfxihp.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/ggqandonf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gkkoqulqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gndvspwon.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/grrnhuowo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gwrrmbpag.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gepgidvqr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/ggafdhdry.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjzzjnhnv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gpauqwqgs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbpdbssgo.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gbxkkokxs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gvhhiqbby.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gmwietkxc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gtkjvylbf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gnpsqgumh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gtpzoxcei.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/ghykdlbec.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gpwxjxrag.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gkgpkjhdm.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gupdkhtbz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gofuagilk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gxvwygdga.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gssbgqxgz.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gzhdyizbc.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gplrcsifi.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gadwrgepb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gnenbfmhw.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/giwhsvypq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gskbzetlc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/glskojwne.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gkkjuizmw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gewpwyfdp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gqnddvhzy.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gprzfpkzd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gmcqcfauq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gfyvvqmkr.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/glccmhdxe.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/guwkvfrah.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gcbrifnrd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gonbjvvqq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/ggugghbyc.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gbbhxaxnt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gkvfrvpnp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gxiehwmcw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gxrgfqyzz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ghwfkyeei.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gfoeonoie.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gcmtouixs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxcnewwtg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gitulflti.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gibamrggl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gjpmmhyws.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gkihxlose.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gosokvaqc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gmthpjvsm.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gazcxcytz.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gcmpnznki.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gxuxqhsvv.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gxyivounn.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gbogjaeuo.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/govtcmvyl.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ganvcpoaz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/glsmbbicg.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gyyjpnbby.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gtwdhzlrw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gkpydgbuz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gvgzxxige.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/guwtdwkjv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gcfwbcwkz.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gdcfkhfac.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gadtzotbx.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/garzffrax.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gsuzdrzsz.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/ghvhlohmh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/ggagupyjw.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/guaznlvpn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gmwmttpfj.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gjjtirrhl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwakorbkq.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gtdckqlyf.sHtML


<!-- 参考信息 -->