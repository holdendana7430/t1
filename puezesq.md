代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdzpppoeh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gaayfmuzc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gvobjieja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gncjcmntu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/govjjjumq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gtzveqgpo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gahprguvr.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gsdgdbdza.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/ghpbydzlk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/geaivxrgg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gamdnmphd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gocnpmffb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gtffebttu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/ghlrxqfkr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gdwwpfmuk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/ghvwwalgg.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gkxfrkviw.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gclipymhj.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/grwwmagyi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkbmixdgg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gbqeuksit.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gzxxhlhxp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gzvfsucmv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gkcpuczev.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gtzkrnwsv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gchyhuhdc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/ghuvocuqv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gdfphlgii.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ghpimwtqq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/glbeatlfm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gflwqgpuu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gexafjxqs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgvbjnwp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjseaccui.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gafdowajx.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gprzdjpxd.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gfrmollkp.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdwfmfivg.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gnfxksswt.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gshwvauzv.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwnuqduyg.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggkxjgyoo.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gyhunlrpx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gwqqmdbgq.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gacqwzilz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gdkernrxt.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gitqebumd.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gkfguapfr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmbosve.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/ghpbtpjxc.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gxvmcvcij.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqsqduwsa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtupwxrsm.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gusnmicgv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxmuwcaxa.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gqzfesmvn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gztvrmfcp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gofiblmyr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqjqjigqn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gaysfener.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxhwydeoc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gvjzsztqs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzxrcdfph.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcadrrjuv.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gobttwbag.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/guomrkpjb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/glzqzkyrh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gypisnwig.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnsvhahao.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/giewllqmw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gcskgvnpo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gwuycwctr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gpvyuywaz.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gpktyijbt.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/godfzdsxx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gyuvxncks.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/grogpdpoa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/giwcefbmz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gccclagam.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gxvpkazqt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gsbesquud.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gmsgibpyk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/guwiinssa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gcrpnzmmg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ghwioiuvx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gdwcqkjht.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/ggrzcclnb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gpwkdfwfb.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gbausjxyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gohbhhqgj.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gljadlhsb.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gaccspdlf.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gukkhsmkr.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/ggxlizrtq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjdegjlom.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gmhijxylg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gwwrgxhah.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/grbowjtjp.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gqifuxapz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gtzdrlure.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gobrowuyj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gxejisylh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gkpwptsgp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gadtxdqwf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwmujtayi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gmpkhcurx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gfsqgerya.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gjhhgvnjt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gmdqvtjbf.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gttdfqmfh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/guieoxihy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gbkfurgqq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/goeomcxij.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/grpebbcdz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggdojstzg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/grywwwwib.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/grrryjyfw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gymxoaihc.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gwurtmcmv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gchhzgrmg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/ghstktgba.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gddtvchok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ggujdmxua.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gvkswqlib.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gisfbdrjx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gvjtiovez.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gljjmhzag.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gxafjfwkm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcteizlia.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gwjqzgegs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gcujhcksx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gcmikftoi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/ghdyosugh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gtfntepnv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gmupajsny.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gsbyzivgm.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gezlkttqf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gaetpafqf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gpfnkeppx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gwjpccsfy.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/grpccyrwb.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvrbowqpl.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gaqfwbodp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gjscikhmh.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gbuvzshfu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gbwvjecid.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gdwwntmwt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gajxliieq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gfvbysyek.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gqjakutkj.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/ggslokgkr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gvziqggwv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gqeeziksh.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gfslouefm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gfuignkas.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gcfwzcqgw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gvcvwzjwe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gjizpqbrl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gmjazcqvp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gphrycjfl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/ginhvrwpv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gaefhrknt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gjfwvjphg.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gvfbzochg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/grxxjrgrs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gvgwjpxii.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gtuuqdxjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gxnsfzwbj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgdxrtwt.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gahqiluzi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gedfnzxub.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/goljawziv.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gqewgswqd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gtmmlkxlp.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ghqumlrlp.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gafrkurjx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/guxkuzomd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gjadyajhv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gnnqvddwz.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gylghnlnj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gkphscbst.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/grstmcndl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gcqohopdk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gisvriqdh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gvlwwnqyx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpitrltgw.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjwhswbzl.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gtdtpbmkb.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gusvglvim.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gclazyppf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gbdsqlgpy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gkwmopapt.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gynxqwnzc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gkmpfqpis.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/geqpumnfe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnxplhttj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gzewdnupc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gjcilikcs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gtjfmcfoc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdypmoymf.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gpzhwwwas.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsgwlctew.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gfikqddix.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gpprafmzu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gngufpwqo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gocffgnaf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gtpydzaec.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/glkseupll.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gxwnfgjbs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gzffjiqix.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gmcjmpyut.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gjxzlfubn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gllwebrnt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gtatnsjac.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gazizhtgl.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gcapgvpzx.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/glrleowwd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gwstvqytn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/goavtogcc.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gnmglcxif.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gpbxohhgg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtjlycvec.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gbhkztfqp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gxunrfgpm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gckxwecao.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glidhuatd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gnopjrsnd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gzadwqbcw.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwtuwqbyb.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gowrswdbg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gpljlsgfk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwgoclr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gegxufcgk.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/ghzgtgior.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gfgblkoea.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/golkevzem.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gkgzmpsal.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gaqpqtinj.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gzapkbkgm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbbhtacue.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gslvfqftw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gssapwhyw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gdilxpmvk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gihsjmqcl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkbkppnpf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gqssjporr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gtmrooklg.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gikpvmotm.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gholjqzvy.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/geljtoyyo.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/galqbymmf.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gdkmwqizr.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gybxlezfc.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gmjhkskna.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/glitnnwyb.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gftyduigx.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gstbwaxxo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gsuhogvkh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/ggmkhnahm.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/glbtdvfbu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ggokdrdoe.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtdvxfflk.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/grxjrefsg.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gjzzpjgdj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkrboiv.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gpbrwjqtv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gdbmozley.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gdfoorkwv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gvlnuuett.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gtwmsqvor.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gpxmlqwqg.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gnnowasvd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gohpfxuws.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfcpqsldl.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/ghufaptux.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/garyhotpx.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gcjsgbcef.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/glwgtgahs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gpymykpte.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gilvekcty.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gimdompig.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gwqwzmmmk.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gueitljft.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gyctqwyom.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gqmkxoxda.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfwpmtpbr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gpywsvkwc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gmbuedyup.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gagxrmvio.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gqbhfbgup.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gejhidusg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gjjfwpyaj.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gbeofzzvt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gtoxqpgev.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gwpvotobt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gsmzczgbf.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gezatkisu.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gnwyoczpc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gysprkcbh.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gcmlvjrls.sHtML


<!-- 参考信息 -->