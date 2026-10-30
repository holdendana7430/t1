代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gxflwrhzq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gvhjkswst.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gmuztakbd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/glymbezbr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnhlpnmg.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gyezmutbj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/glxswkthr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gboixzxvj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gvhblzhil.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gtfcqbyzu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/giwqvjcyk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gkmqlxeqt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/grqqjrepq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/genyjwvgm.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gvcopuhcp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gjolplpwi.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gevdedrcw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gsjjwomqk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gtprbyrwl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/ggldnguip.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gnmksheac.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gemwhraxp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gmdndsetm.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gwresheoq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/ggqzdostx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gpdluqaew.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gugyjxjoi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gafwyjmhe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grbhsqdam.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gtnhvewxk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gidvkndts.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gtkhhylvs.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/ghzajmfcx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/guispcsdr.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gfndeforf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gjwvvgzep.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gzhsyxpqd.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gfiomyvbt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/ghuqjzdul.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gxgakzuug.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/godsetife.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gqkmyphbh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gblwjfeaz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gatnpxhxt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwgdkws.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwdpmcezz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gwinyrdsv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gjoyoynql.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gvsnlrbtw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzxccujre.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gvldbdibn.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gbwzvnifn.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gokivkrer.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwqfkvsll.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gaxysuplz.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ghrpsanfh.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gyanyzvtv.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/guaixvopz.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gusdhrnek.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gidomjovz.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gitznzuqe.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gtmjidwol.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gbbsvyowk.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gjueymcof.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gartwmkdy.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gfiuublmb.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gxxkmkerx.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gzsxybmod.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghwqvpyny.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gbewwcolk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtcvfezdr.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gjelwrdyd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gsamzfpkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnmutsnjn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gegeqzogl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvinicplf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gifkhqhyb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjsmuku.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/ggufekhfh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gktfoowbk.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gexzrghen.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gajrkdagz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gjqkmpuyi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcmzyorat.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gbidcniqp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gcuycnjgn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/ggzedabjg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/grwyrffnp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gbunpbmrh.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gctgicjvv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gbqpgmrkq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gphtzbwpc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gryuftmlv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gqfxppvwd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/giawckhai.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gzqxaemde.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gaprekjhi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gysfbjdjo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gsuecglru.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gvevhfkeo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gcoduthkw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gtggxkpgk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gwhztuawm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gjvqonmft.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gndabdljl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/giycjtoec.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gqsljqrcm.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gtturwuvk.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/grnznmyal.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gzrnwroey.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gikqkshrx.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gsrhywaoj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gwtylxevg.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gyetewjlu.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gjdidwdrz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gqiahhcbv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gsahonbpy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gttahltrz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/glsoidtbb.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gvmyjejij.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gwruvvvnv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/giqiirbux.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gbbmwyixp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gsebljtqg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gpnvwvibg.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/ggwrbmgzp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/ggymqiovu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/geepodocl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gpwqnptyd.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gdayvgavb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqdjmekko.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gxsuzdedw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gmcrpgnqz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gjppgrgbw.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/glenlofuj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gjyvpaquc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gsstxzbbd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gwefjizok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gihwpifof.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/grvlddgkv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gmkhbqfad.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gpzjfwfjy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gnzmdvtkc.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gzqfeciqh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gezgqgrxw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gxztmnfav.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/glrhgzpfm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gwmfthbck.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gjfdxjtad.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gszqqaxmm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gwdiyruov.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gxabtvifu.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gwqlznvji.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gmrdxvurn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/glifdehnf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gvpscjtnn.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvchcqrce.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gfmvbqghq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gjwjdlgkt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrarlxe.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmkfsowed.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gktpdkcqx.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gmmdiruve.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gumlsbnaz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gmfghroom.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gizricmen.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gqtohcpkj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gsphplviq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gswwvvaza.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gezchatkd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gzejxvygn.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gciocjdwx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gkubebwav.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gbeokstom.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gsxqwfyqf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gitgyuyxv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gtdppmxoe.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gmpfetzdh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gfgszyzay.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gpdlvplhv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gsllzsicq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gkgzyzqqr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/geogcgfgu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcmklfhos.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzhhlqjth.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gkhuqtdxa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gtfhvukjb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/grusgcekr.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gbkpklxju.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gcxboylft.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gqxqiwrbn.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gubfqdvnz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gklatrbsz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/ghwogyncz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gflvqvizi.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gvhskdthg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gwyafkxix.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gavbxcbht.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gfahivjia.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gbltisjae.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gyxwivagg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpmjykhma.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/glfgcfodv.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gyigsnpqu.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gscklpwuf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gepgczwov.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gmuihofql.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/glhshirss.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gbrxasjpo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gskjrmmgd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/ghhufueop.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gcanghddu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gqrgirbkd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gsjthnxzt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gikgclvnj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gczsqehfo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gyfdifkmo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbvwsexzn.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gcfbqasyj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gygtvjilb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gpedagzip.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/glqbkdoqb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gvlciqepy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ggknyujba.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gxyhjruup.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gnwthgkmx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gymrbcjhn.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gjtfiptao.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/guarfaopu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gqkbtekxh.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gokjezwsz.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gpnezrrys.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gvnftgxvg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghuteeaxf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/grsayoprj.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gknhyoleg.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gbianrsmh.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvnwgtfts.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gdzmtoxso.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gabfmjfic.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcidcadks.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gcigjalin.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gabpdsdgy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gdzmliqyb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/grljziufj.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghemgqzei.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/ghzuhtrky.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gnrjishen.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gfpcetwpx.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gypyssevy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gywlnziyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gkdgjngwz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gkurvkunm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gqshxzyjh.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gmqtcazpr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gdtkkhpwy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gbiznnsza.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gyuaakvip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gpqrmtlwi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gwfaffefr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdixgvvuk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gxdjvtdpc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdbshndgu.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtpxxhbdh.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwsyeut.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gmgdbemne.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gycbtymfn.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gklyuqhzp.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gdepmtnnr.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwfnaiznk.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/glxzodwlx.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gjeixtecj.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gtbweaegv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gmtdyxihp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfouzjmeb.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghhafcnwk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glcfqnibe.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ghazvixsk.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/grotsgcwd.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gqanvzijr.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/ggncscuih.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gfmkovwpg.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gqnxhnoyr.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gfebvodsz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gfezdxckx.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gipmabtzi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gmrgchbqx.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/giqtvmliq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gjkomybtc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjcfozzzv.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gnyvyiayx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gcyiykxps.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gcxkgrgoq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzbeykg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gircavyma.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gbzlpdfux.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/genrtqxlh.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/glpxovwac.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gutguglwc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/giccstpti.sHtML


<!-- 参考信息 -->