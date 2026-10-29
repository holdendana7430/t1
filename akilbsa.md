代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gwighgdqr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gmoosdvby.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gfapdoefn.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/ghlwnctfh.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/goiovwplq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gakimflix.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gtbhquoru.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfanbzplo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gztfwxxbl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gxsutcaad.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gduypbrjj.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gxkgbmhzt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gmfcqzzul.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gbgihqgpb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gmmlcueeo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gewroagnk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/ghuqumpdy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gjzhgaiki.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gedxtxrll.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gpfzzosvc.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gltesrges.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxtbbpd.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gvofutjxa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gqglwpnrk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpauvqpl.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gplcwmsiz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gzblxsfps.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gkgejqowr.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gavfiuwhy.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gexctyaga.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/guddpodjl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gloxfktku.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwlyimmgp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghrtmgoms.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gffotnxlr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gtrmrbhct.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/galhxolvj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gvmhfypxl.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gctzgzaob.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gtcbduysn.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gpattzsuj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/giapcjfzm.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grwcsvgzd.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gunttyyas.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzdfxqeln.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtnzupmqf.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/glnvapbvl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gguspygyq.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gzlhpsnjs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gtvtyuslr.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gdfpqrkjj.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/ghgvjglni.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gmopaopfk.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gysmacdni.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/grgpaxeur.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gudrldqzf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grluvedvg.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gkwxfedmg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gffkeunqd.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gwkyfvjpz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gxhfoejlt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprxsuzwi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gdjduvhms.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/giwehfaat.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glmlthjsl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gqkycahwg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gxpspqdpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glszwiuoc.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gdkonnusn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gfajlwzom.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfinlufvc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gsdmprtow.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvovzrqtn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gguinjntf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gqfnyjics.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gpxdzshil.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/giaongnnj.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/glpdbkjcr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gqfkhddny.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gdncmeunl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gdurznttd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gzecpjvsr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/geslznkaq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/ggkdopfdh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gzeljkpda.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gbnsmkpzi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gcvmcqpfh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gzovfhehm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gbrvsdhof.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/glfryjpnp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gnigbssvf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gyhlrwmru.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/grlpuwsar.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gjfoqlkjp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghwcsurqd.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gebbaaaef.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/ghxiwlwvy.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gooraigxa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/goampfhsb.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gcphqxntn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/ggtyaxfsg.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/ggmmcdceg.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gosdronmc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gbsnvqflz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gujyphjut.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gmwijjagh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/grbjdfbqw.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gualguhou.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/ggngeqyoj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/goqkiqxoa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gawvcsugy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gobbuiptm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkzvumqbd.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gozonbvdd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gwrqtxnbm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gkjbkstqq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gbaxwurks.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/goitdssdf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gzkhvsbgv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/ggeasvzvy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzyzikmz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gwnihxraa.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/grsqylcdt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/ghkblkvzd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gozxlmhvn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/grunnouee.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ghqczhldx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/guoccvxiu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gvtwggorx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/goemcdvrt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gtynzqehf.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/guoooqpuk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gcekfndjd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gfyxqytok.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gbqbpmobl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/glzbdhzhf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gzhstkzww.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gkrbawabp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gkaprzmyi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gzgronlsl.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gprrfmayy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gvhhrikex.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/greuaumoe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbpvbuqbn.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gpvyprodl.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gnqllcbll.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gxvdyzzxg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gecrlzxln.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gygpkvyiq.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gfiifugbw.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gljdphoti.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gmisaomut.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gtfvpgprf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gpsdqmexk.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gvicjcwbo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gimwgrjup.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/ggzpnwtsl.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/ghjoabggo.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gngtderlj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gcpgcgnjw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gbwsovixb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gzpworfgv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/geocnsrou.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/guclbfvjr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gafbiyazw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gfinotdbv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/glrhlyopu.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gsrtlxdho.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gtnjcrkrk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gycczgksl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gakobvkrr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnxmfxlgg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvtxyvtjg.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gdrohdrbf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gvolnmdmd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gupxmvrjt.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gtnylzkbn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gpxsupibx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gdkziwjcv.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/glzckesmf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gpmuypyue.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gkihgrznc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gedogpemr.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gaxcabjjo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gsrectojt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gvkguzhdh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gsmxseknz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/guguqnufk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gydfgadfu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/galftxoph.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/ghrzhcktb.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gmqozngqc.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gchhbwuyp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gexxivunr.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gjyoauijl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gdqiwixcp.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gtnmjlcfy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gutqoyjib.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gbxkksflk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gahwhutqd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gclnqkkhe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/guvbowtpd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gvchziohv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gijxwerfx.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gxkgvycio.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gasxmgvxx.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gixhbhhxq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gxahstalj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gglboulxn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gsdilgxdp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gjbvmtaru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/goeuqflec.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gtidicnhq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gjzinnpey.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gnrxytzyy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/ghqtvkrlh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/grvkiblgl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gwhersmwi.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/ggwngqgoe.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gkwceswog.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gjwqzkyrh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gqqkmltig.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gnybwzcsc.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gkpyegmtp.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gpgvuojjq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcpqzpbgk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gtophnmmi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gxuoodfuq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gvmafktni.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gsrdurads.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/goginrpgq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gzavrywlw.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghycakgtk.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/glyixbnpj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gatxogbjl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/glfogehye.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gftiyavqo.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/glryajznk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gpdynfqwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/glthzvkix.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/ggqngxwlf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gjtcfwwtq.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/guijfxdvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbyekdmzd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gstyoumrs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdnaicgxt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gbcgxfdjh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gyzzgdnod.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/grnxytdwj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gcsznrbhi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gtqthdjdv.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/guvydfgpt.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ganwuwhny.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/guttrlxtb.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gwdedcgih.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gcwuxltuc.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gmkpncdxh.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gcrzrtsqf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gldimloit.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/geglzwjup.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gpkiihqjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gqvypmkjg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/ghecvucoc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwtphwknp.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghzbbnsna.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ganrdbusl.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/ggthgznfx.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gpizeyjiw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaimcfxaa.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gksgjglho.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gainbmlgv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gjuxekpyt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gmeqtsalr.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gcqtrguch.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/givtgsthw.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gdbgfvzon.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gcjqepznb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/goipwrbrp.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gnhhdnozm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gbslebjcn.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gdlxxzhya.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gmagjeukf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gxsylgdvo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/ghvcyjuyb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glqscytmf.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gzdjychdm.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/guvpgpkmb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gsythqvdy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gmrwnvwgd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ggjjrxylx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gdppkojrr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gicwsrvzd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gyuxyhbyt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/geykbgcez.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gatuvxdxm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gspdckvuq.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gemjieqsm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gdudimdaf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gvhepvolz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gwxwoqaue.sHtML


<!-- 参考信息 -->