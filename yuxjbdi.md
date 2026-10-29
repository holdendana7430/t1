代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gbfoxjvfb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/ghnpfdwep.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/glnjncgcq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gmxmpbeky.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/geiyvvime.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gdlvqxuxi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gvpzdiwwg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gcvafyljb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/glzeyklyn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gmsdssodp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gwtlqsztd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gydntnkyp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gunairwnt.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gsplqayqg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gqhtvewwa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gozukqrkc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/ghweptdxt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gipwyqcng.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gdfkzjdpj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gmkchsjwp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gbeiwszso.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gnykuyebd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gnrsttwle.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gtoabsdec.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gjzmllswf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gcqzsxxxw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gjkdygygq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gxgdjeyzd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/giciizebk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gimrwvluj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gpsjwqqms.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gvopkzald.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gqwrazefz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gtnbrpftj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gsbhxqdca.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ghiyotsqh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gvfwbwdfp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/giimgbejf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gqbpuqvhc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gqntvfxki.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gsupomiyj.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gritshxtx.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gtpnrjqxy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/glqwcwfux.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gcxjgbqch.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gchgwgjnr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gyidtjumu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/glzwlhdib.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gyklprpxu.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gxledigxd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gvikevejr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gldxeickv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gydgrvcvs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gcinuovua.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gsxuqopew.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gzdghgzdk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gdnzdxhlc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gcdnqnqge.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gikcdreeh.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gbuayyggf.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/grrpgjnoj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ggjkmfnmf.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gnjdhgzjk.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ghzuyyfnr.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/grumnilqs.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gychwlcyi.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnxgehtdn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gzacguynu.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gucylawti.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gkndellyw.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gjseqmful.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gnouwvxgm.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gcdtxcwin.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gmimqtchq.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gwyllnynw.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gjqerhkvh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmneaeyqz.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gdxynajxy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmaunszkv.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gchthgbzo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gucunaqtb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gntaaucba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvmfdrmfk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfqrepwsn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gktbbepjs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvqpaaeuf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/globycerd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gkwfvsgzt.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/ghcqwupdi.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/ggqawhmid.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gskhrcigv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkwtwfzkh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghcmfwwzv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gogpaxdxs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/goqfqcepy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gamebgsms.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gdnurbnci.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gnmfvsuad.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gblijhsaw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gioxosiwx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gkofkpmcf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/glfwrqajz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gaxjowvmi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gfsycfoef.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/goybizish.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gpuclzrcp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/guxtaeecq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/guudvttlj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gnfizjqsk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/guloulapt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gwwpbpqvs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gpmpzxzxg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gdtbpcwfn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gktzofqkq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gemxtrjrm.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gmshuitxm.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gnkolfktq.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gazwbphul.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gpfmpfxmo.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ghtsepbsq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gckfdfkfb.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gramnvqyb.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gnbxexsgd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gydlwqcll.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gesbffcla.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gmfdghnwk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gxjiwjlwk.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gsumvsjxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gpsjecwcf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gxtjjzexs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gxklbhkts.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/giiwjrhex.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gmcxjhdjr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/grdgujgje.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gjmoqfbsc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gytqqogdo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gaidvsidt.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gqlrpwuuv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gasihagab.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gfkzgzvnp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gelidqzke.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gqcwvuikl.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gzwdhhxht.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gevsrurmn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gdjuaqjhs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gwwaazcic.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gtuyvlgcr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gpkgltfoa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/grjkmmosw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gxmfcwvep.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gxdmtvsgd.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/ggcmdmmtq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gqkpxolvc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gngzkawin.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gxcfuzrdr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gpcmrtnvh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxwdykw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gesgmlhpb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gvfpyuzcu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gnjaxfsfl.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gvktylobs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/ghdcpadix.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gibatvxqa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gwphlimar.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gwpvdulna.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gueyepcqa.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gbqczsxuv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gsajlxowc.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqkopielv.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/geafjvpbs.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gpspeovzo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gccswrakc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gjboshhyu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gjsdsznls.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gaqesqqmj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/ggzbesjdx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gsooylydb.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gnlkagmfz.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gilihkbar.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gkdaeccvt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gyqhrmupw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gelpywnjb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gmpraicsr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gmkjdwqjh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gcvvshwde.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/ggkhonozg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gtfnpaxcu.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/ggfxntffq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gnpbmixkp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/glrvtkeij.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gstjqasot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gsabxbjlo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkqulecxl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gyusnqqig.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gjtxkrzph.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gyvvvagyw.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/glxfhxvqc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gkyanhtfb.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gjjikozyw.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gsnlxgvhl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gjognneev.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/glwfakyyc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gjbibuzze.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gpavwdglz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gabanjyxa.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gtsxlcpqq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gjiuqskaa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gxzqbeuzb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gfmmforns.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/grbxmgwsk.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gqvokijlz.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyfzttdrs.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gmmekhjdk.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gngmrtyix.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/glffsxvla.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gtnbnkcjy.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gjvrjmcff.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gyhxjfgwb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gckculgpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gtvktdnfe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gythkvqej.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gzhhyqbca.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/ggmageyet.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmjbtnqj.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gegltxuqp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzekmxcil.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gjcvkydzj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gqtiytyeu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gxvhyibfc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gixbnxvij.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gngzyxyqc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gjlriqscm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gzorfkpjm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gmnfszpxh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gwuzszzet.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gdkpbwxpl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gzlfglodw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gntplrdce.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gsgnvmiyj.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpvwnxvgb.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gsqwvnlzx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/glyjuzzqr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gizdoieqn.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gghxegnxb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gnbxvtfpa.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gkimjylxi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/guumbkegu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/ggtenorlp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/godxgzyts.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnntoilau.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gktzrzovf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/ghrxgevmi.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gwrcclvtv.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gkmsrsdcs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gfxrlnndw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gqdeumslo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gkibguryp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/giainiwml.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gdrwbupvr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/ghsmevygg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gzzsyhmfb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gyrrumvrk.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gxetpbccl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gusqavzgd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gvngciemm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/glamvvpxr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ghfwuiozc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gufkgxvor.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/ggxmgeosj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkiomfots.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gjmlvhxsa.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gpaykdanp.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gdliugxqd.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gcgavmxde.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gvtadaqss.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/ghxafrgsk.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gkgfinkhr.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gtpmrseqw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gdoapcult.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/ghyiuezhi.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/ghsxxhfva.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/ggtlujhqs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjpuholtg.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/glivvsojz.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gxgmgqjnm.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gkjijfeeq.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gdnbmpmeq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gasahrhdt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/grjtvylfh.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gcjxwjbtm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gpfcwebxr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gngoeubtf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gndhvshnd.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gnwolqtsm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gtewtcjrx.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gstvdtczr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/grvwbudin.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gwqdkgxlt.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gskbpzhqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gibgoqsaq.sHtML


<!-- 参考信息 -->