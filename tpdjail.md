代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gkzzaimxx.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gmkbsosdp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gtgjxuoof.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/goembfscy.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gmwrdjuoq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gbbcdcdys.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/geaxusuao.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gmvwgekqe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gtidiugvz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gygffpatx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gzncamndc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gutdnbnrx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gopuzcrns.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gesxpjaul.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gcsnmbgoy.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/guidetlkk.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gormrzxgk.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmlrylsom.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqecjyynu.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ghjntgaaj.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqvmiwmit.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/graenhgif.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpjkveyej.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gkxqcozqm.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gmlrojmlw.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gxjlyeeyn.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gprutvhri.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gwiodwgdm.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gfkhrdipm.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/ghahswayu.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gdssfweyq.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gilwbqflj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/girxbambh.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gtlzksfxd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geyoqmbwj.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gdpxivcyx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/grykmlflg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grqwxlmhe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzpllbqfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvyzowpws.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqdzwdauy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gvbchonig.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/genhphjdk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmcbzpdtp.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gniovkywo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gurqmmjug.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gpnstgltr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gwrjrpchv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gekigtmht.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gpsqfnhbt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gafcwdqpi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gwredcssd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gmrovruvv.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/geudrqagx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gdznwtdnx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gweymwkho.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gwotatbqx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gbazqampt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gspuiswiw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gkbzoqsqr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gijrjjkwb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gynfhnaxh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gebckuntr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gxoohzlpv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gfoewzvdp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gxtntuqko.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gaftkfaxq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gscftynlb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/guhbkmwsn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/garawkqxg.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gojlrcvxz.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gaxcsmnse.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gnycvjndq.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/guquhivbc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gztmsscpx.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gptepexmf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gcckmeqcg.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gvzadgonq.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gzmiyysrm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gudzoojtq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gefyjkkqe.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gyaiyourg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gsjrbitue.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhhcbatz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gdgtcsmwd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/goxpwmylb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gtgirkccj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gizungksb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gpoypjufw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gtptsafxt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gacthkftd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gmobtjkjq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbraxlp.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gtcqszjue.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gvndfeqph.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/geantvqrj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gcfcwztxn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gwbdlhvri.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/grkbclhms.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gcilkbzcs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gowjgcdwh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ghipmiuig.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gfhktnjec.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/goyfiqgxw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gtwyihhtk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gfsvcipyu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggbtufxie.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gcilycbog.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gaymzgerf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gxkbltywm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gmfiktgpn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/giocqndcw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gruxktxlf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gviazejgq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gcxxfnncp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/goxhluvvn.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/ggrpsibxa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/guczaokgz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gpdmxhgky.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcrtreh.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gyrkxtoeo.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gkauuqqys.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gjmwpbgtl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/grctsyrvf.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gawijdrzx.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gzmklcqaw.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gsragovpw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gpprhmomp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gytkjvgkj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gyjncdetj.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gzczzaknf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gtbxzqghn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gpsqsevqg.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gwgxqymns.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gqpiyoely.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gdvpzskai.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gbcyvyrdy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gvqizggvp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/ghpnzcygl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/ggdyokdjw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/ghmctyiqv.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/grigjeysh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gqyvivrea.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/giqeugdqf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gzcjguqlp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkoilfwa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/goyfvvqjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gcabwufbp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwiozjixv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gvmcmbiqa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gevcbuofs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gxzrbtnyp.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gkaxayxdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gxtrbhikt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwwvkzy.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gadjblhtx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/ggixfqnef.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gczdntmga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gclxheipr.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gkeltdnqz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gswjzkjrk.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gctkmswve.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gfkuuyvlr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gkcqqzlzo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gljpyeezf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gtaiqevwt.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gswqfzdjy.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gytgcadch.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gvvpojiou.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/geqcweaey.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gpatjafqt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gvehycxsz.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/ggargqyyt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gvwjekevi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/geaomdtpp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gkzljbbxs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gjvaokaae.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/glsnhvwef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gzfesfsqz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghcuuasrm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbaqyyh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjgppzgyl.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gfwxurpuu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gljgvezec.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gqlmkyoag.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gdypwnxov.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gtlcrqbhq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gygbevrdt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gqmtfuyng.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gucydnmcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gryzculwy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gfkjryksf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gfrnpxvrp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gcgiqmsdt.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gbpncfsia.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gufvgaqwv.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/grlfyxcpr.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gyncotjrc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gusizaovm.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/giwrlieov.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gfooysenu.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/givldpqyb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gedmpsrme.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gznzyulhf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gzvxkhkgd.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/guizjlecd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gtleawnht.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gwhbqfoso.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpvxjetyv.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/giarqziyp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gtctckwza.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/guyvfqaie.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gknnmfgdn.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gpoaohote.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gvmgmfnoa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gafcsvpci.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gpeeskcnu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gekethpfn.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gtdhvwsmz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxsimceja.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/guueyjkhx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/glwjxswwn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/ghdjkiudh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gjfaerwsq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gddehkvzj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/glkpxsdvf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwagsjjkb.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gxdkwwfvq.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gsgpwyzey.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gdcaxaaft.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gqsopimdg.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gkyptuefw.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gccgdlsnn.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpdtjuiqp.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gahhmvmgl.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gpgdrapjz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/grjsmmvgm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gzanevhqo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ghajejpqk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmkkmvmfy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gpjdfuyxc.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gcwqgmkjn.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gchswfsbt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gwiikmthy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gznfogkbf.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/giakikqox.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gwhgrsdvd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/grusrepmb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gacfllmlq.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gwltqxpsh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/guoedsnir.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/glfrqampo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gszafuwpz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjvjeowrd.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gtxrvjoxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gaicmkqos.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gneiglybr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/ggjeealqt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gibmkbazy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gtaxckarq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtoxqemyz.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gnfvxpekc.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/guykgetny.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gdezsbxfu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmajlbfsk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gjihftgoe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/grpqujgim.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gfabfcxug.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/grtpsagey.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gqwlzgapo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gqxeirrku.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gnqvgsywc.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gbprxmyrl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gwvkiecdp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/ggdeyjjqz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ghjobjelw.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gjvigwybk.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gqssqkoah.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gblpdtkjk.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gmyhktpnp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gifpwpjfb.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gixavvppe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbecrkdjk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gaauhyplf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghdmrgxau.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkqqkzbj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/glnfuxdxe.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/guticdnja.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/grdvkqcdp.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gwwipcuqg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gkfuglrpb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbjsmmewx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/guxfnukks.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ggefbbsxp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkcwnexba.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnkytwogu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/ghygtroli.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gmnsxphht.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gpwvqxwux.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gvzkgtnls.sHtML


<!-- 参考信息 -->