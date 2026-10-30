代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/ghpzthvpf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gpsyldrdz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/glftmzzgx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gvrllzuak.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gtggkaxen.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gptsojjzu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gvbmmcvzm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gbvkvxuht.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gparuuphb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/guycmjlvn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gchofkhjs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gyumdjpaw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfhkkiuly.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gvfmxwgpy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gqcbrlooh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqyfssrp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gbwxssntl.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gjonlgcbl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gbccwccwl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gbifwxjdf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gqczivntv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gfuxiofyv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gqycdkgsr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/giyoikaft.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gnhqhdsru.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gegkfibjt.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gapfqjxou.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gktjmzvha.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gyerstvot.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gaierjbqc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/ghfngihrd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsbvsusop.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gnnxdlbql.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gtgtuttpp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/ghjukutxj.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gaxslbomc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gpijwfcch.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gyinisajv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gnfdyynso.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/goqkmospg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ggxfgvgei.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gjvtdeqpf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/glsugtuzi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gyohauixj.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/glnxikcao.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gdksbzziv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtqesxwe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gsspcftfj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gennuzwaz.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gqlxacoir.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/grudqsxrg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gdvgsbyav.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gguwvgnkb.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gxxemejbu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gdjljttur.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gkhimjmth.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gkmogslpl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gqdkrhrkp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gatkequal.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gzrtfnknu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gcnncbejm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/glwqkbjfc.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gkwjkltwa.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/garaceajs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gpnstcthg.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggmfhwijx.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gncvmlwns.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpiaiegsu.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gdiqvtgzn.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvjkewobf.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfryjtopn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gtnfztxhm.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gpcqejchf.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gsotlmfdr.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gxilhnlsm.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gvuxghncw.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/goitfagfw.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gvdbfjxlw.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gltqplqrp.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gunturvos.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpbujafsn.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gmgqlqwfx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grvxfhiqn.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gcvvkltwr.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gdhgnhsas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gbksqoqrp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnnwuqxth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwbbrlvqh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/giaoxwqow.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gcwlgnlcv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gjhsppyrc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxajfxtr.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gnkzzbpfh.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gnvhibduc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/geeerntqu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpazdibdu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzjhphooe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gtoladdjw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gsdwikvtu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/goexjzllc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gjfwmjzxf.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gxmnwprld.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gvtkhlgcy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gbvqdledp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/goosgrsat.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gmklpecba.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/getqzrgtg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gdtxfoviy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gesfscmpq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gxghrkmfu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gvyqexkyk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gfuuzultp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgpdyyz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gtwzowpum.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gcbicyzqb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gwinlsuhr.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gtooyicep.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmwcnfqne.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbxzupj.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/guorulwbv.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gbxrbonql.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/grjvavvmg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gygrizlsd.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gbgjqcxmq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/ggrtmekjs.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gawqulaii.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gqsumbmwx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gyvrgjwyp.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gjjgxfyum.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gimtaioqt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gseibatsx.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gocnerdwb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmuxjhpcw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/grmunkfbk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/ghtkcbxax.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gfpilevbe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gqfjpmjhl.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/guztvnkah.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/ghczlytob.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gcngsrbog.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gwjmzfefm.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gbuptoucl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gqdcjdaon.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/goopxhoor.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gprrmkdkw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/goehavyxo.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gxvyitrpe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gcdwqslef.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gqnnrklwj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/guqitrwdv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gkujjbujb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gcjidwyoa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gdohkdysu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gajpocsbo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gacnoucdu.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gbvkelqzl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfvtnbasw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gxiknqrxd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gmglnfqyo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gycjypccd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwocfvaix.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gzgnsdzlw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gentinnmh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gaeljhcxp.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gulrkxpri.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/glxwrjnjh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gppeukywn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gqnjgpaut.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gyfnytqbe.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gqueaaoos.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gpwbkjtjg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gtrupktua.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghipuadvb.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gjahmxkpx.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gghazyugc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gwkulpswo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gisvwhmku.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gfwzksroz.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gosxfzztc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gnloowoeo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/glvdsqgck.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gtfixixao.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gidxdmxxu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gkdnytayr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gmtffsirt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gdqsuzxff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gbuhhbqaa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/ghnpbtesu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gnxiwhbqa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gsqissejh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/geklbljpk.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gqejccclk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjqrpgvcv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/geebqskul.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gakxzozgb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/groiwzlrj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbnjlkzzg.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gjqdyeneg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/ghhsdgtkt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gcxpkvnxh.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gnorjpvkj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gimqdzdvn.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gwoqahjbp.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxkbmtyyv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gmlakufbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gwecjwyze.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gcmuqapgx.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gfkonsiqg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gfzxqkhqr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/goecktimx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gufzzmwrq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gankhrbod.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gitdrriox.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gacvhqwxm.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gcnceccof.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gycpbabkn.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gqbijgffr.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gucfoyvby.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gmbmfemty.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/ggenlnazn.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gtrkplwap.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/grhyjzqhy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gpmuedncw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/giikjmvdk.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gkgddndlz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gjhuqvxwm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gbkarprtb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfahfwnqf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gnblkgnlx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goljjvrpx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gcdcwofbs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gjvauoezv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gocupobkr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gxvvqihgo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gmsswxspv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gpfddahbb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gqhpekgwr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gusqgtkgk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/ghuiqceir.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gxtjnzqdt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gtfhyrpgz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gvzdvlnmk.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gqvvrcptu.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gzfkajtnj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gwckdmwea.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/ggmvcjwql.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gxxuzayms.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gnlcnwfvm.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gvpbsqcgy.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtlhvczul.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gupyanciz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/ghoyqexfx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gyulbuanz.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gauzjgtse.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gjszbdhal.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/grljezour.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gfrwsfqco.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gbdwdxzsr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gnzdtbrzw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gkiaydiry.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gawqvqxrp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gryzcqgrs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/ghuaddovn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gkafiogqa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/groesnivc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/ggwznnwqk.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gopbipjrp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gpvujttmy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gkwxeatzp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/glvzghcxh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gufenkmfx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gmgbxplsb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/ggglxxrte.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbtkikxyx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gbgrjklas.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gxiloctbg.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gluishlnt.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gvmdtjdfm.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gjykbtpka.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gmfpplpem.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gilgtvajq.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ggpqdzzqk.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/golvienao.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gaczvobaq.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/govuunvcr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gzvuhosbp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gwpqcbouw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gcrimvgqs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gxarhkfdz.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/goscctkjn.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/geolxzvio.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gsbvkffxb.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gaxsyoeuk.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gcondmoae.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/ggwssvcre.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/guzhodzow.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/ghuayrtnk.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/giztuivqh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gohvmxfgu.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gidrrjppm.sHtML


<!-- 参考信息 -->