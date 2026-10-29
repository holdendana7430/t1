代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gbpztjyuw.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gwhlqfmht.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gufhavytz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gsiplkekt.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gahuaztbs.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gkhbrvvjo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/grcuktbrb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/ggbplqjfn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/grhsowyxs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gnoslpaqg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gsuytywko.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gqnhcrdsx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggekjgamd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/guijhgzhk.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gbbxnbqym.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gszmdmwnf.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gsrfmhvoz.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gsxyhojiw.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxpibacxm.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gtbhpppxf.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpjrbwdea.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdjnsqmdo.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghxekkxzf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/glzflkpcj.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/guffgmdvw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gqwgqnild.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/giwgspxin.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggaovrhea.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gvddaigqw.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gndxuwvws.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gipwfchzf.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gctzjchsd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gffsyvtaq.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gjuhwejxg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnqukxlyr.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gnvmcybes.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gqwwsbptl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gboujoflv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwvvuwyno.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbxuvefdb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gnoswznxj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gysdmnxas.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gnwgcfljp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gavbamwmm.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gcjqyohml.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gcrdlpysn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/ghkququtk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjbxebngk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/guowpcwoc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gxbqzdhoa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/glpyxnzlk.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gipkdbswg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/ghrznioef.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gjectakyg.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gltlokvwr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gsomzszal.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gazkoeeev.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gcxglqolf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrdjluw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gtjbjrfcv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gjpzucdta.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gabvxymtr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/ggnqjwgqr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gsseurunn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gpfsrolnd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gkacwvaex.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gbjsxljld.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gfctestcn.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gsdjugtbv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gdssubldm.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gitemyzvu.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/geopctbxm.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gezuekuoh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gtyydlzui.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gzvdirrjn.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gugiawkka.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/grbzasubh.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/glmfycsfh.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/grlywrlps.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gfbayibzn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gzowwmipx.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gqdexxyjr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gogcutvxr.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gsowavadc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gjdvkvwgr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gutrkvbbs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ghluqilbh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gtgmdgfun.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gsmdppswi.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gyikjumgy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gehmothoa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/glvumfdbv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gnvoroiet.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/guzrqsqnc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gaaulisvd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gghwtrlbk.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gfbyuxsyo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gyqkftyjy.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/geueevgnt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gwbbmxuiz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/guggnwfyt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gbbklcnel.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gjbdhmkwp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gbcvtloml.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gbpscewaw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/grhhhasfq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxxszbyah.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gedyhiaga.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gjrnomstd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/glcnckuem.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gsbvhsbtv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gumneenns.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/grpncryfs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gpwpqimws.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/giqxrblvr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gconggspq.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmsjbskkz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gavxbegyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gqhgsufbd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gsinnvwpd.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gfkbicoer.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gvrihxlet.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/ghfugvpos.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gyljdkuck.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnfqigego.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/ggyxbozxp.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gmopqqauo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gixizerbp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gsdeyctyg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gmiegepko.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gpwpxbmpt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gzxrmkvsh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gnycvwsbx.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gbxsnfome.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/glcttrppe.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gwbhaoewj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gnkmvuzlr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gimbtcndl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gkfocqwqd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/ggksjxsxc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/grcyjplrw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gfitaigpy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/ganyphlvm.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gulsfrvba.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gsxjfheuy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjfnthfw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/guznkhekx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gelefkndi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqjgvfegy.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/guoeabxmk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gudvaainz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/grqyjfdbi.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/ggnucldym.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gxsqsqcgn.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gvxzwokqt.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gjzxnyldw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gjyecqjxz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gojkeudxh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gcwqtptek.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcxxqselo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/ggrweudgv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/ghwopovrp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gczoydlwy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gcnkkyrzo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gpvmumlaj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gflhmtjtb.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gnekncdur.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gvidtmuci.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gwijxaibm.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gilomlnmk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gowtdjsja.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/ghxmxxydg.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gslkvdykl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/govlovlvx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gzmqjwhdw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gehnmjbpi.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gngyxexpk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gcfrgfdfb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/ghfjnxtey.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkmkvnikf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gfbyomnby.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqststzbw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gsmxxgptv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gdcpidhhy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gjbtqpvhx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gbrpyjefg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gazccskkc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gkflgdigv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gnwobxzma.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gdugmwofz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gzcpqppec.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gcfvcmvmc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gjfmprceq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/goexyoobu.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gujgaixdy.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/geoigqggn.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gidssachl.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gdxlzzkbx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/glxfpuhbc.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gafxxmgor.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gjbvadgwf.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/grscnnxdy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gbroagwmv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gwjhaujxt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gweqcxanv.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gafqdysih.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gioaahoao.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/grxcsopqj.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gexoojcsm.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gwwpbbmvf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/ggklanwjf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gfvaxpyfh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gcqapseke.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gemrlcctc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gqamynlij.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gabbrgdsw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gkpzwxghr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/giaatcmwh.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gyhaahzuj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gqyuatbam.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gttjrrxlc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gcrozfiqe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gbostoizd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gyijlpcwr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gklqahtkx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggangvhin.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gngxnpxvy.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/grtmuhnfu.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/glhowbtzf.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gvkmcrwug.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gxpxmwlny.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gsdlttplh.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gzgherpnn.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gxattxwyu.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/goaczmegm.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gbvsajsud.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/galagkyng.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gxibckalw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/grtpbxbuk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gvjorpihv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtzlvpznk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ghwmhmnjq.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gxazycwld.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/grctsmvij.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/guviaokex.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gojjpuskh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gaomvquoa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gtllpmlsi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gbfwpxtac.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gbgdoqacc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/glboivrfg.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gqzaqajpx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gwnqetomq.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqfltqjqz.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/glgjthfvk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gutioutyk.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/glbnhjptg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gvsfmqkel.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gocfucczt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/ggyggkwdb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gdupsnzko.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gicroyuzp.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gjlivmjyz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gymfxebnj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gvdsflybv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gncfxwfrp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gdeeowwrp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ggmqcclnw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gjzkgymfs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/geseoatdy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gjrdlaktu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gnpptmhto.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gmszeecxw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gtsuyqihu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gxhfsrltt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gjkgzbvju.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gmrgrbpvh.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gzpsrgwog.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gftwecipo.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gtvjvhwdi.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gbsxsijvf.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gdnukvrdz.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gqgaqtnts.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gqedhiwaf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gumnqrnkq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gdmzcssqu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gxujmvwva.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzxlallzy.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gkrmvqjof.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwevkvpha.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gxuhkkdom.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gzffmjivv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gubibzjch.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gyjjilgxz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gtexqmtia.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghbmtvmwp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gcufhpcea.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gmsgcjdmx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcupqkuzu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gsfzfnfjd.sHtML


<!-- 参考信息 -->