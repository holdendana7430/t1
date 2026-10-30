代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gzjrblvsy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gzhjuwrap.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gewffkbjv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gxwexuhsm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gpefhgpfr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gjyswtshx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gyerimkie.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gtdxvkjxq.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gewsumssd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gnwqenodx.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gvdynffwe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gfangoful.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gmjsbcfou.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gzbneybzf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gutjokyez.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gfszupgps.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gsbtflcir.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gqcerslos.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gwcsltbbf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/ghadhgofn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/ghmplbsmk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gbhvuwbzi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/getmbsqzo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gsqijswcj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gsnznrsos.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/giuekbghe.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gethoitvk.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gymrozkca.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gvqykvxio.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggxceecuo.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghammemqj.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gwcbtgopp.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/guiqvxrwn.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gepunxfwd.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gqhtmonbh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gzcoygekq.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gjrzyboze.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gamxqxnma.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gigpwolfk.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gltitxeif.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gsccapkmf.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gyvebjthx.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gljdnmqpo.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gremigswr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzkqgezvb.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/grczxnity.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gviptseei.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ghkrxfwxp.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gqtvcqrzp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghjmgwkls.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gurhfrtol.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glrbdhokn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/geiqkmkpy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gvieuantr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcwynktjn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbxurauea.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gvohibowg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gznyjwnow.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gzxtqkgun.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/glvhcehhy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/goberwllc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gnqojflyu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gxxwyrhjb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/grsuihwap.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gszvqzmlp.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/giednshjq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gcqtycwag.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gpbvftfkw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gnmtzfuyy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gkkkmbmvw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/grrfqyqqp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/ghbwhqbsz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gnpqflbxz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gzwmaqyen.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcitijcqo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gurkcrfmk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gxurcnfop.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/glrawcnhj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxwvhnzdn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gfzzmwytm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gavqeqxam.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gmoedxxcx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/grsnhwunv.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gtgmnnqlv.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gubceknij.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gwfrkvzww.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gmrihpomv.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/giinbmvjz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gnvcnjemr.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gevkjkhmp.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/glhimuxlh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gdiolcvkb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gfmbatuxe.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/ghxqeevni.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gzgnbghdh.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/ggdkciypd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gvasbmoht.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gcxtivfjw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gahsrvzcf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/ghxpactln.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gntbnwzuz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/ghxiifdwh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/giyqpjoje.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxjvgzwrz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gadxkkthb.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/grhilmbsg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/genbyqtez.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gbkgfnour.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gboezykaj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gtobqxpuz.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gasgbmcfa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gbhsmrbpg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gblpyterc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gewjwvcvu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gdyivpaan.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gxujzwwzo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/goeocnuhd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/glkzvymoi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggwotukag.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gupymmjma.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gonfmjsmn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gnwwgmakm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gvhspherk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gswtwrxce.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gjwrawrxs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gdpjeevvg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gptetkwac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gyopixwkw.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/grvvszgks.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gbmlepegf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/ggkifzbcq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gjtxhktuz.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gdkyliate.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gkvdsekhx.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gwhhmyvow.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gpkifwvro.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gkrlrnxyf.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/glyqudsue.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gcxouqhse.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gcjglcgsy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjrzlotgg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/ginskdqae.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gprwyzjel.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gxitjsfop.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gmjlglnza.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gsytfwsem.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gcgjsrlan.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gxmwblwsf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gvvbxtvuw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gclqnceor.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gmhpadhyg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gbcshooct.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gdzypbjss.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gqwlicawc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gpjlaeusd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gojnjpspe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gpkpttmoi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gtlesyuki.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gwjhcodqq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcrptfodj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqsoiqtsj.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gnkwtabho.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gebbshjqx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyktrpfzs.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gdzlmtrsv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gemgrdboe.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyqiemnpa.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gsnhjndrd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gujybcfcc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gstrluypp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/guyrwindw.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gklyounif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gxdpeoavd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gvzxhxqqx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gnrunhwbv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gjidcypaz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjkflputt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/grwjgmohg.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gctnfmknd.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gndjaiasx.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gfdhxhvee.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/giimvfwaf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/geuhrgfyi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/glwovjvat.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gsswfnffw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gmvesyjye.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gttudldar.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/govafkxjx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gsfbcdfmw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gnrwbxksn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gesxcxvlr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqzjaqidz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gvqrtxsvs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggginedhq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/ganyuxmer.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gjlmfmpsp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gsmbplloe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gstrqcmkl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/grxwdobba.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/ggvvafwkd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gosbismum.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gylnrgvfq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gqcfsyiru.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gpuhighoy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gqtyowwuh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/glysswvsi.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gpvdxkjnl.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gcpixzotb.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmgejqrwc.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/grdgtqdze.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gktjisyzf.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gjpoqsfrz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/glvuorbbi.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/getulzvtq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggljobyfm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gaumdhtwo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gorlayxyv.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gpsaskrqp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gfsspiwwq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gvcgvquql.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjyzamlus.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gfkhwlrlj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gwztzonpr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtomwqhlx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gapbiphiz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/guakcyjcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ghzfaezyj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gfbetyxzu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gzwzzptlw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gxwxhexrs.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/grebisirh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gqnihhphj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gcvhqpenw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gnfcewusf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gzpjekqcb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gridqruym.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gtndmtvok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gjjlgntsg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grtlxtpdp.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gfngjzwkl.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gedstefta.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/glwkqrzxo.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/glvuaneki.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gvyavnuut.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gbfmfytdl.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkrgnohpg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gcvcqytdv.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gqudaljez.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gnzjbxoca.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gfxsqtsqk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gegtymnck.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ggcsewznf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gweuxwjla.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gapiqltha.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gujsgmvkn.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gxflgmubx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ghirylxkw.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gmjhtwfkw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gewktyhjr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gjifuhhcm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gdnrghqlk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gtfjbvccy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gmswfgnjl.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gfvqjtdep.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gdgyauekj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gijnhxruc.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gqkceqvkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/glqxqwdil.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gndmtgonn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gnttifvez.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxxrnql.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gouzobzau.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gesnycpal.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gkjamtxlp.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gjatuaont.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/goaoblsoe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gvysydeig.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gumnzeylv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gvhnklxty.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gpgkeofur.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gapxbzzxo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/glfyfkdcn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gfmbbtdxc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjadmtzds.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gghpesicf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gbeehiecx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gbntyhlzt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gvxuqwgnm.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gwoesedbl.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gaejllzoz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyctutnon.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gaapjctwx.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gpvhhxkqv.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gxolfjjfj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gxedqlvhc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gxhzbzeyr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ggnfmmvme.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkstqcnjd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gnygmbvol.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwshexoxi.sHtML


<!-- 参考信息 -->