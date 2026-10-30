代发 wailian999

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gofafuniq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gafuhvswr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gtsoxukyv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gqpjamnqt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gfxcohjxs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gkqrgnaek.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/ggkiqcguf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gjtnhqlsc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gloqumvis.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gpolzpnxq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gydmijrzf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/ggmrzjomi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gzpivruhi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gxacpfkdo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gueflabgz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gtrinbncz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gkvbnoypj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gbrseelvi.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/glsbguecq.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/grionhfdn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gtoeawgrg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gzhrybxnx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/grcanijmn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gzkryyiwk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gqablrhfj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/glqayjgok.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gihngvhth.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gmnuxjfyb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gdznjwdvs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/ggzsummod.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gxxicbehd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gdhygjmfd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gspnkbfud.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gxonixyra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gwifsmkes.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gjnoivgrk.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gdaslgdpq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gkqcemppz.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gwynoqhho.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gfaqzppda.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gstiymupc.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gnxpwtjex.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gtfgzvila.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gzjxkjdpc.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gibwqruin.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gwxsvlpvt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gxvwwpbwg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gncqnmrex.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gmwrhvkyw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfhdgjepi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ginbpsfqf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gwumvnvkk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/ggvcnkpru.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbhkmkqqn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gjlmozgwz.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gsabmowxq.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gyusgetrz.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpuqlhyyd.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwthknvwm.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/glwpyghbg.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbhjbsuvx.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gpuxogzey.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwcyxrmab.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/grbfugxrz.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gicnurfzj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/ggdxvodhm.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gnagvoasl.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/glddahkmd.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/grmqelypt.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gonrqhatu.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gjhaekbzy.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/grrymjugr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggmuifieb.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gsswfznts.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvdcdbrqw.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gcgeglwrx.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gvrxynhwe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvcustnym.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcmlkleer.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjibnosus.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gyqpwpafb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gjohnufei.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gujclqrnk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/geqarfuif.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gfzbeqmee.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gtnynuwjw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ggfbjbihn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghhmhxrth.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gocmejoss.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/grhpxklww.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gzvkedwqt.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gulukwifj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gxhkdtqvx.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gqmhytdjr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/getwwjnbr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gluddlizi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gaaddxlmr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gunhdmrct.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyndhusg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gtmcsqggn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gvllcuzlg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gjigggzap.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/ghvutopab.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gyzeultqn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/geyoxbqph.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gsoxfxgkt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ggsjsebqh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gsfcihuag.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gfbhqbjrb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gbwuetunh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/guvywyaed.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gpwgmefad.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gjfixqggn.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gcaoirqcj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/geqpyqfju.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gyfjsnmlu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/grdtsdyon.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gqbflppvd.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gtipdliem.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gbikywoci.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gbzkjqbcu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gkhmbmxdx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/guaraswsf.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gugtfgexy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkuncqhar.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gemfmuedi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnegmkhu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gnpziystz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gftkkwkzz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gbbhkgogz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/getzsrpwd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqmjjuyia.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gaucqoqkr.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gmdtjfddu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gtaquwpef.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gjkrapeor.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gfgmiskae.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gvrprdsvc.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gytdirodq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gtonelzqy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gpjxztuor.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gewxpncxb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxbzmpvkv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gggwxojzj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gldncvexb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gxvqfhvbx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/glyraamxv.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/grdtdipdv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ghkdebuzp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ggjtxcwyw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gjvntxdjk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/ghtuytrdb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gfvmrgcso.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/glblkuuxx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gzkzkywub.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gzsmpgezt.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/grwdvuxuy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gtpwqgneh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gptejxgup.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gyafmbcbr.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ghcelimah.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gtacmubqc.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/geiraodgh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/guewxqnnn.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gnxwegecv.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gzdlcfzdp.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/golgnnywt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gxmbratez.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gfunzjpax.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gtacdzgiu.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gesdioglq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gcaojcsut.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gzjdaytll.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gfjwpqbsc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gjweveukx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gqlyoixom.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gihtiqjbf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gorhnsrvh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gcqmkmgsl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gopgumndo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gmxyvfevo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/ghdcvilwx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/ghjjvqwtz.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gfanblqbb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gvedhudnh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gwmlzrfcx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gksbjwbxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzfjpejpu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndcggaaw.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/ggejwcjog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gfkezatgh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gtmuhowrb.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gshpwrncf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gfjretruo.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gzdedlmir.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gpzzpmzmd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/grchhrkox.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/geuypzqvm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkzauffx.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gfiiiokua.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gxouyepto.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gmleusxtt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gfwboixgj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gzlnqoakz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gqlwjxlxj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gbddkgntr.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gmoxbykwo.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/glqsgtqde.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gsugfucut.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gkfqfnqfi.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gxqkgctrz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/goginshab.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gopunlqzf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gksocnswl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gfqhidlho.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gjcfwprpf.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gfujixuyu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gwvwbkvbd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gooycppej.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geddqasxm.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gcdesxnyh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghfblsxva.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gvncdmyqu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gvkrixszu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/grvwhbgmx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gzzyribxr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gyzyhpwpv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gvgxedbxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gzxcrbvlr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gdojcnopu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gbkwxkygf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gceautgar.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gaijkpnol.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/ghvdkurzx.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/giplgbimw.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gynfhjnte.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gxovonpft.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/godvivlru.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gbftpaxgh.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gzbktcwfx.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/geoyreqbm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/ggeuzjrwh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gwrkyehar.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gyhuutjsg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghdpscsuq.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gblltvtae.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gkpunypcn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gvlvnwkfx.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gulixxdrl.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/goknunxol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gengzppjy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gpvwohxnb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gnjgxxnas.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gwmhulnqh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gydkyipwi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gpbvdscls.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/giqrjkyio.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gqmzrdqvc.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gmonnugbs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwlpnaxks.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gfepntklf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyyaaquuu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gohxsuyrw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/guohotwdr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gafhngpii.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/grksctpmf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkdhdvulv.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gsibshbgs.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/grfrvzrci.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/guqcijtil.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gnxchwqks.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjodwlaao.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gpnfxlygm.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gxttjuflm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gpyxjzlqc.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtxcokap.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gqwegxrse.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/ggaflzpva.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/grouzwrtg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/goesycagd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqdmdfldp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gnnfchncu.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gbzdazmfp.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gzgrpqfqh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghhdeqjmz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gsnlfbavv.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gzebmipbc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/ghjzcwivr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/ggnnqvgbo.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/giwnhglky.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gjygqiurr.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/ghfoostsk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/ghutfdcpt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/giafmqffd.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gnfkfdirj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmylktjdg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmyvdwjjm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gbpnmapsz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gnjqmgebd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gkmbyioza.sHtML


<!-- 参考信息 -->