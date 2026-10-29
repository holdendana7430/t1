代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gquedouuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gknaryhwx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/glbstvvbb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gqjdniecn.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gjpfyalgh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gndvmdboa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gftkhbwup.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gfcshralu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgwdypah.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gwgmjosyh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gvexkdtmp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gquqrlaki.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gntjvpyzc.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gtspybrbf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gocttxxud.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gmwkitkcp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gvumdzdlq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gzgrxewof.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gupohdjub.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gecdcnwpe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/glludagdz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/ggafrarwt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/gskocinrt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/ggeyougnh.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gnoocpdyh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gcttwvlsa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gqstyxrif.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/ggzhhxqpe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/ggzowhqls.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/geazpwjcg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gwpufnsjn.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gibpxrkau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gnotldkvq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gvjlkqfat.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gmnckmhdu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gznozwqin.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gggkbsgfx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gpglxdzqw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gcndryxrx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gxshghhta.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gbivazdlo.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/glmicdyie.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/glbcxdwki.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gsonmxgzw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gkdxaqyyx.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gtxaznonx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/guuchcsdk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gmvbgcril.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gwpbpngcn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gynfwwryq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gmlzjhtzo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gprhvhbho.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpkxsaqeu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gsfqrrrgj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gggbzahux.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gffevslqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gsciqrijp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gqghpring.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gzvnefsoc.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gwsqjtqzy.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gsqsbyefj.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtwiyqhdd.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxljxeyvn.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdjgdssox.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glochtvdq.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdmqvtlqv.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gplggzsrv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gfsgziitf.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gkttwmebl.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gefmglgdd.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/ghwcgkyme.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gkseqvpym.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gtlshjzdh.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gjqlevmpy.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gzdtfhkmm.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gaklbcpey.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/givtercic.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gandabxxl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdmcfcklt.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gkopcmugl.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/geqxyuwdg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gfpubvejn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gaxouirdn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxehhpgqe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/goodgehtk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gfgilzicw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gyetbvduv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/grfmpclfk.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjttnnkqo.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gnzqtdica.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/ggjfnjgrs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggiwqdvgs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gqrkhugmz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gohfofapn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gacbvwvpm.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gvmnocayr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/ggahumavm.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gjmgbwmpd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gslfzkzgx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gvcgjftqf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gbzxfuxge.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gfuyzcwrt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gahszkjvt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gepbvejba.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gwwheyzta.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/ggttgnzgc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gdyfmqruf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/geqwlgdxw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gpuemznoa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gvuvtmefi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ghhaxzhij.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gfelrfugc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gbqgypupu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gauasbxfw.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gmtoyogjj.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gknjbaydv.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gnnmotxbx.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gjiaozayc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gzoaxbilc.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gerakpwro.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gugkfcwei.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gerceokfg.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gktpvbjsq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gackolzys.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/guuqduurt.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gdgknfhjp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gzglehqhy.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gqtgpdqbu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gbppxvawl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/ghnmryqju.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gueqmfdym.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gtwkrctcs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gqvdddwuy.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gvsfdlzhb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ghvainspt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gmqrjrvqh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/ggypyvjpn.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/grsialqpm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gezoezcnd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gnyeipzho.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gkbcueiwl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gxygebcku.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gjtqbcpuf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gswsrfbvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/ggfbkbvig.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gtqsxoesu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/girvoawiu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gxvcfuizq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gomgcpfun.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhtopya.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfeclklvc.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gmfulpfkx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkifnovoy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gmaamtqmu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gheotwysj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gbycrmqey.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/giwkkdafa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/growcnatv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gnwvvojmf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/glosdpeki.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gbsyyfxrh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gwtudirkg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gnwccenng.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gyqnjlprp.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gdvarzooa.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/guiapeway.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwtuedfvp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gpbjidafv.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gtqeodify.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gdpywjteh.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gnitllknr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gutfekqob.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gfwlkyvjk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gmjawysky.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/glwmguqqt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/goqtqimnx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gznekfvti.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gmaebsynl.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/grkiobxnv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gkfdxrofc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/grsfgraww.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gczolnrrz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gqzduwacx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gphrmnhah.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gvmediuok.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/glrwpyfju.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gcmmhlnzf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/govejchar.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gllmjszbm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmetrcjfq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gdnppqsof.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gsmqrwgwe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ggwxjipbd.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gahwgmwgd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gepgileob.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gtshtrxvh.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gyqsgpwux.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gyebmgwfl.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/glrkhuqed.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/garakqmoy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/guxfcoova.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gjczdxnzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gzojiktvv.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gpworroxx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gllyhpqad.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gzjsvbedd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/grshrpges.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/glehxdofp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqzspjiiz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gqrrnokbc.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gfjorimpu.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gaikwrdsw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gvpavqsmr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gpdsowkiw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/ggqfyobto.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gxocpfbtz.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gxfboumjh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/geonadzda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gfzqmnmpa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/ghsfzqqtr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gscnvdcyo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gorkgistv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gzyxjcilh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gleambzsv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gjwgjwfto.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gizsvnhpn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gkvkukunv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/goqwegoys.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gfmqbiykv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/ghpkweerk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/ggvxiladp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gjrqweqbj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gtdwisnsf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/guulvxmxr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gimnbevuf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gqmprjfpp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gbxifgvrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gwajnntyz.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gvowhosmh.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gqcwixafd.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gsubimfup.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gcwqgtxwq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gpsftbmut.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gfvyssgqc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gzzrquxfn.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/glwnqkour.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gkqthyfyd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/goacttyvt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gdrdhvblb.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghmutqfoa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gmdrgudvq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gcuybdctv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gocdqoatg.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gwmxzxdvk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/ghsjuheli.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/giewwaobw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gljbrybey.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gzycrtgpz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gneanjqcj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/guonshvvy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gbyrusxrp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gzoxxoiej.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gourpmdyf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gunivvdqr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ghspsvscl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghmzbtlmq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gaohhnzqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gourhehwo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvbnmwklg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gwnbqfssy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ghvltaicw.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gtijsdgim.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/golhnunoa.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gppesaljq.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gorezvgrf.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gbgyezcbo.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gatrmzcmi.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gydsxnxte.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gkymcdulf.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/grcjlijgu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gbjfcdwxt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/glituhojn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmvkpbcou.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmpdfldnc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gdzxafovr.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gesmlcqzf.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gdxurkvnq.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gabijqmtb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gvawoztpu.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gzntuufhv.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gumfwnyfc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/grgsrqwll.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/ggzlcmtba.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/grzilvxyp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/grnvqghff.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gndetpafl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/glpuvjycz.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gqzykzyze.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gyzbeknct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gbdsligwd.sHtML


<!-- 参考信息 -->