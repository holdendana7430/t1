代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gtzhufwqs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gigieglfn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfleegssk.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gapfjuxkm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gbbgmrdcl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gxpaetozm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gzewpjeae.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gzsedragf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gzudaxnle.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gtobkvdmh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gauugrspq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gyvssndyg.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gscsfngvd.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gdvrjkcmo.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gobygfxlh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gxsltjuup.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/grvnvbcct.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gvtsfhzoe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gwcmlozvm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gtsaaobfq.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/guyicqkhl.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gomnturtq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gpybywohc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gnqfnuted.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqldneuzr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/grkvqoclg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grpkwprbq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gfoajprbb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gzgdmckop.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gnkgywqxs.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gmgdnddwo.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gpziazedh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gcbcwdevf.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmawqhjtk.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glerfrbtb.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjicwhgaf.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnwuwxnax.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqtjoggtl.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gajsgqfhh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gmdiyfvvx.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gtzrmmwkb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gterhuybh.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gsgxzaplr.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gzcorllzi.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gutaiymtk.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gsmfnfphm.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gdomqiloh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gihnoffop.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmhsaumwg.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/guuhzbpkc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gijkbnguh.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ggnxfmzef.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/grwtkrnaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqiysjkwq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gipywdmer.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghpmauqnd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwptaohwo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gppadubvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gavbkvxau.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnckkbvln.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/goiyoejfy.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gwtgooweg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gtvhcavud.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gxydqfiwe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxacqqpif.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/ggqpdoqhs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gzzgnlidl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/grvdnlece.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gsxrvggeo.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gbjcqeuhy.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gwmkvalfy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gqbyuuena.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/ghjfoxgbb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gcpgnwiby.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gvyynwsdy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gcmgxoyrz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/ggixvmiyl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gxofgfqmw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gawgjgons.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gokvllcpu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gqkhwcqgr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/glyueqmwb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/ggkszrzom.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gucgsxwoc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gcogzdjoo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gxxtyqbkr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gzcbjsjcu.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/ghlbqjnyq.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gknrfwjnm.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gtypcimgk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gigeogdyc.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gtflcknkf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gckrzhmtq.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gqsyqmvif.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gigfuujnt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gfgwptona.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gsacjtvpc.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gpzfdnziv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/grkzhdwor.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gupoddlbi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gtewgonnr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gwwkxoujx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gplbmefct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/grlyysywz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gyhvltnab.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gqgjeggct.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gagptqtxl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gbpcjjswb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gfcvhmzey.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gkdvdiscg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gitiseeze.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gemuhkxzz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/giiiuhyzj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gmjyrkunq.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gqawialoc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/grxwclfgc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gvufrqvah.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gfxuitbqv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gtledbdgd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gfdnemykl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gvztlldlf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/goakzopwf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gryvesyqk.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gyqwlanhu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gkkhkzkkd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grpzsgdrl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gvohkfexb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gtkvxzhrh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gjxqojvvd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gspazsvau.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/ggofkbcat.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gogokeczu.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/glykbxswm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gsjebccfz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gzmjjcfkq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gouwpielo.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnhlbakih.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqtthddan.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/guouofrna.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gbqjhbwhg.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/ggnrzjyoe.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gqgnbwqhp.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gtugteozz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gdagmbsck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gdekeeloq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gesroxdvx.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gswxbbzwy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/geaonemdo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gizkhjyej.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgwfjzwb.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/glwkwtqju.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/ghxyxsxoo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gwmawkljv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gvklytcyh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/guxbfldzb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gdtluuhga.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gitcdljmo.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gokrcfyln.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gzrhkbxix.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gdajkeoac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/ghresexsv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gxwdhikvf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/glbymyvng.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gdtowciwx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gnmzdsvoz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gtxpkeiep.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gpqduazfl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gkcmelqvy.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gwbkvkwnr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gdcpnxcom.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gmoqvmkcw.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcssuvxkh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gjydrrttk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gnloajozy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gxqpeidxa.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gurajveum.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gpamdqeiq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gtsjtqjsx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gbdnghwxu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gppjbhrqd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gxtktsapy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gfogiehfk.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gxqbfrmxt.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gjkegryhb.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gkolanmjq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gsazhhvgh.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gqdgidyho.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gjetecaug.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gdaekqlhb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gdgcmyirw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/glhrdltmv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gnwlfmois.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gksqoippk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gbtrqczvi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gwafwwqmc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grokcezgk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gxecjtoqm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gknddwqie.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gppbrsqsc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gzrcvgzpp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gjokjdkka.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gzdanoapu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ggizlpikv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gzcufddna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gqxtvaxah.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/grwubhhji.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gslcfsdue.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/golkbrddg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gajarkfac.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/ggvgfqvhb.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/grhnkeoxi.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ggshyqeub.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gjpsqtqmr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/geswzeybr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gikkvoqaj.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gqwwxyzoj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gyuokanzh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtpugjduz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gpqravfbt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gnombhcuw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gmitgfcex.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gojpmnywe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gdovzkaia.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/glfrmepcg.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvidufbdr.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gndqkmaqg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gknmsufda.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gtbdettmd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ggntdwiyi.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gwneeaykp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gqiqshxuh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/ggjbxvqwz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gdqldwgge.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/glinysgrw.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gjzuloqet.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxbfhkzij.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gabzvwvqo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ghalhxiza.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/ggpbhgpbt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gayvmyucb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggqnoqgpf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdiklyhcj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gucnnfauo.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gtjptegqt.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gzzzlfloe.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gfodtlwuv.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/glqftnpgz.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gpelksowl.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gssiqtnqf.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxngcixqp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gmgaetazf.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gsjlfdjge.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gcdmxabbi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gyqbxndrh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gtlnekxie.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gkcixmhmy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gyyxzzgrt.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gaowexqxv.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gqpbblrcs.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gobfsqnaw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/glixbqbrn.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gcnkfavzg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gnqyewhua.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/ghmnjumdk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gzhexvftg.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/ghmwxiolt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gyixpqhom.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gvhgqnhbq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gngsmuhot.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/grhsotrox.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gmrerkeat.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gzxsjzeou.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/ggjpgygtr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gzctouedf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/glhimpqrd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gmotzelzq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gwyfdwwfh.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gpgfgkaja.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gapjmfndn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/grhmqpcsx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gzxhjgmil.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/grgplkfny.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghcfwhxew.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gurjlwnbw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/geyiawuvp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gvtmzpdoi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gyhcpjbzt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gyqimturn.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gukwdvhgn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gpvrgomov.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gywwyuzhk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gahccrjoh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gxertohlm.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gbiioykhh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gokvzhqfb.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gmtwpheno.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gnpgfchjq.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gdjyyuodw.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/grcuuakdd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gdviuaire.sHtML


<!-- 参考信息 -->