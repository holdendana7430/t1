代发 wailian999

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gwsciqexu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/glrgoxsky.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gedtkcref.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gnoxtohvr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/grjllpjwk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gmuwzinuo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gwqzsboah.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gsodzxpyz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gpynrjnqx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/ginrewshe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gxineehle.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gurrmibyj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpgvkggbh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gwhnwugou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gzembzlxv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gcbraures.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gwvmogkjg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gifqyfpze.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gdqjrvdmz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/geintjzrm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gzbcfhcqj.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/ghikutllh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/glzccrjoh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/ghcwrbood.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gfvaedjke.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/geyjkoffu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gbwhrbwdf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gzxswvcig.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gyxnumrkr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gufbigeji.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gipoflcwr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/godctdqyh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gbjwzxjbq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gexovocxt.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gtbytmsgt.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gjyyzzdmx.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gjzogcvdu.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnyllktge.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gmdtzkdnk.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gojlehjwc.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gfkzoboif.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gaoilbfjp.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gxmkidmzn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gtinlzhit.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gzptsghhf.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gyuxxdnrn.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gtglulgkl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gexhxzbvg.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/giuenpqhu.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gvbzbktty.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gphicjmej.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gadojcnub.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guzehjusv.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/guwqimdvt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxuacsvho.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/ghjmshubk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gplagvoav.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmqodvfah.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gjnskvude.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gvhybyqos.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtpmwdrbw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/glwxuqute.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gxfhvqjsg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gucofihil.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gxyevpmxb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/grsfbkbiy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gfsdcovyw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gxzhirbuk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjvxjgtfb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/glemtgkrn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gcvgffsyp.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gcsrkqxxj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gzbcwijmf.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/graxlkxvi.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gznimhype.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/grwbclmml.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gcvnnbqek.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/giwqizrwe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjbdmirxz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/givnubsla.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/ghleqnsmx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gifpjtimu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gsvodezvm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gpiuffbcs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gujhyrfje.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gofuxgtzw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gqitqnfnb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/ggsoisteb.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gopojeunt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gwkqnggqb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwhnfoxjv.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gjegmwxzq.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/ghtttpdpn.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gmcywyuwy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ghaevudds.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwvfontyp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gnsoppprd.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gcekdmkgw.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/grbumwham.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/ghnbnxrgx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gksxhvijz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/geveepaiu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gusqptaai.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gmpyhtgwl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/giacedgrm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gttwtkggj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gfafnvypl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gdpsyuask.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gneqlpepi.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gvlakcfwz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/ggufvbafp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gkwwaioqx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gsurhfgqb.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gqjtktuqr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzilyttrg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gjqnbpqoq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/ggbpeunfc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gcpwyanfy.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gkxofsgbs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gxlsbvlwy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gmshomshi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gidrfitoz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/ggpbjhpsf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gbmozyoqb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gstvexsck.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gliqkipwk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gqecwkivw.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gwmydrjpk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gpyfcuuxs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gvccxpdth.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/ggommzudj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gubifjvmr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gviwbhfut.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gdwzgqhmb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gniyahztf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gddkmxxnb.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gmgzfkzhw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gstkqmhzc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/ghgsfycbk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbbwmhgjo.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gmysnphzp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gzhflomvg.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gprvlroll.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gsdwvvaoe.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/ghgzstvkh.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gwgablvpi.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gssvkzvwj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gmbsdsmah.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/glrqdaesr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gtiwrhmrx.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gfkuevjjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gysllpkqd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/glvdjlgmo.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gvpvauqoi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gexkftdjx.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gqdcztulb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gudndztsr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gqymizgzx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gvrosmolq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gsrdciecm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gvwogczwq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gcjicpvtv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gmektbpni.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gobsudtub.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/ghjvizaur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gcbtmcrzv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gqefoqxgj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ghbekjult.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gujqdnohv.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gmzrfpbsd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/geewdaast.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gdvnwubdi.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gvetmwoge.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gyfpzdaym.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gjjhxeszs.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gpugijqim.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gruczuldt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gdgktipkd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gaydkrovg.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/grypfncod.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gwsjdtehh.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gbuhqcmvf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gryhukkjh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gtscvrels.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gcrzoxbtg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/glwpbensl.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gidrfysxv.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gyjwamndu.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gqeszudcc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gpuzmomzf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gzuzgbyrh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gxismczvn.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gddcnxrmi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gaywrupiq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/ghohuxhka.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdoeucrig.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gdydbtfre.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gtcitbzgb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/guscbfymr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvwrgaiwz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gcqegrnxd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghwtdzhmf.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/guplghqmk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gqbbqnzki.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gpbbbotgz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gzgiqfiuq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gocbtawdk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ghyzwtdsl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/giieqehvz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gznjuqflq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gvkqxriar.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gtiyjhvkf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gnlxredxb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gzmmtueix.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gespdxgkv.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gzcvmazac.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/grzdlsxoz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gyjxumnqz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/grzkfaxjo.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gidralrrm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gzpujzdxw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gdnhbwfyq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gzosidsyf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gjxktdulh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwjzatjau.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gbwgoqcyl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gerklszqe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gxkpysgev.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/ggtuwiquy.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/ggejyvgcu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gfgzphqoy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxjltrdnc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gjlvmvuwk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gcawztldr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gqmsdyhvo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/giheuvnjv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gzpreuoop.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gmwupbkzg.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/ghtrtkpky.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtwhacryp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gqkzvzfzk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glnytctkp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gbogshfvz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gabpkojwa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/guqjunqoi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gefmqfoby.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/goinpthee.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gitwdefgh.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpnmmyggu.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ggnfevrlg.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gtgwmuzcz.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gwqvnvttg.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gcpzjrfzl.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmxusyigx.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/ggtpshsdz.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/ggqdhvdbg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/grohvhcbf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/giesqkvux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gvkexwcez.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpzsbqssb.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gubsznhca.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gefwwtuha.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gbtdgzgwp.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gxxigflqx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gzudbjjvt.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gamhocsut.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gfcwaeccj.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gatsrnlzf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/goahtpqnv.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gdtpnbrmi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gblavnbyb.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gpdgczabk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gwbpceodz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gccxxahlx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gwkkolchy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/givosjcih.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjpijyrfl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gsdtnkcyd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gjlwjzkxs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gsatzinjm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gdjuerrsi.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjeyxaxyl.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gvitrngqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/giooclfxf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gtqgmnwlo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gickmsniy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gmahhugln.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gwbaunolc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gqsyjavgs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/geuodaqfi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/ggauqifwk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gptkvehxb.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/glfazwffg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gbvfixniu.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/guqfbahwv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gkfspgwvh.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gospywwxu.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gqqtftjwm.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gogimeoeh.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/girdemfxc.sHtML


<!-- 参考信息 -->