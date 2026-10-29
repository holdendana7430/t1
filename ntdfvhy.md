代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gpcuihits.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/glxiflzte.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gogjnjijd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gmguzeniw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyczxcazu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/goxmtnovf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/goasmzccr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gruokihbo.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gihjgqgpg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/goikbzrdn.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/guwqcffqe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gdotzyhwa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gjtnrkhnf.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gfltbvysv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gmwwldtke.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/glocwutri.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/geqfzkudw.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gsknwxsgt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/guvvoosar.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gsupfdmzx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/ghtfqzegk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/glvngtjzd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geglceexo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gaisbkwtb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gukngovee.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggkwpopwc.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/grflappuu.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gnhsissuo.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gxakrxlyt.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnfbqvttv.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gafcwjqpc.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmvmmxvmm.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gexbhxcqo.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjhqlspjt.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gcdoovsqi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gaywpwukj.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/guucbgozh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gansgywdu.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gdnrornwr.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gsadzhhqb.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gekxxprme.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gfrwdzyez.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gcnmqfthp.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gfjuwmjup.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gymaddhcj.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gyrwenvev.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsjojpwdj.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gohiovvkz.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/geuoqvhlz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqoctozsb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gidkjtplz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqzsdxoyn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gqsdiwjlh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/goywlrxux.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/guslutxiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gnwupjtee.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gdsoyqwdh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gukkfdbrj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gocolubij.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gqdjnhmfg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gppuiodkl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gqjiqsawx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gtqpcdbvj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gkxshacca.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gkcvmdvyp.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gzildhiwo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gzvjscwqj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gbusgsbrh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/glwporwmb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gitajqgmg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gvmciqoxd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gkgembwni.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gdfnywvka.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gaaklvhtv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/ganpcgrni.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gakzuylky.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gzxvulvre.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gefcaoaww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gcxliooat.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gpyrgpuvb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gurbpelqn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gddvmwfth.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtdesrcp.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gbhpwwzas.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gispssney.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gpktimrnv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gmmjwqyit.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gzxyxxkcc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gdmzcloxr.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gagmlqyfn.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gdwdelcwl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gdlcqwngn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gjuotusqw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gjzbyenwh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gwvmbgxev.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gfvcbqeeq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gzmvoaqih.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdewomeig.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gnnrmslnp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gvtxkpdks.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gcngrrqto.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gjkzvhcfq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gywohkgbt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gduvcrhcr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gfmmsbbko.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/geqrccdqt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gdzfgqqtb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gddqvgjou.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gqphykdug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gqrqbmgho.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gnalhcgxw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gzxflvkkn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/ghquinvgl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gidoafulg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gjvakhymj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gktftftup.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gbncyojla.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gcqvnzcyr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gpuytoydo.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gyrflubnx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/giqfikkzy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gnmsbwnfn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gexiguqsx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gnmxfqmxt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gejltikar.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gzstbdvsz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gvntwmgma.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/ghfuxyxgi.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gqwnjefzc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gdsbuswpx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gjsgvgkxv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gmdpgzkpw.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/giblwgrwj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gpcshlvyh.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gsttebsoj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gpqiuipdw.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gyuvsumkg.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gjkvupqtn.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gjfoivsnx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gtrinbqax.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gazrqvqlg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gucipfdxq.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gagucmzum.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gpxgixqtr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gmlrsaeya.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gkflbzczq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gpvyqmzth.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gpzpdwvxj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/ghdwpozfp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gtswladbu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/glpzzodgm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gsgpxtrce.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gbcldzkuk.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/glpcccjyp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gidvqsrvg.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gfqibakon.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzasmnjuv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsqozjpcf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gcckeszux.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gavhprlyf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzrpmap.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gbthcbfoe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/ghfkojokv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gdakemplx.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gacdxycdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gzzsrukwt.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdscdavpa.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gjbvmntvj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gnegwrurk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gnqwsdcvc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/ghqyfzypo.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gopcqiekm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gibmdbvub.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gyyxhfxgr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gnnfxgzap.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gmppbqczr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gyawgbbtz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gcbmvmenb.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/ggyzlilbm.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/grjgdlcew.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gdmnhgfkw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/glgprrwfs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gkzqhstsm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gnsunafhj.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gtezasxwq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/ginuuryrp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gxzxtsvmj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gvmduixpi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gvngiwnsy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gxhenkeoy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqtqtvxdc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxtevirxa.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gvrwyyior.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gykgeoeuu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gcuxmeufq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gibzjhder.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gmdxoggfm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gzhwzlcsb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gdzibskhk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/ghjlyehby.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/givsloolj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/grhiwwdul.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gcwicksgo.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gpcwibwkr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gbfybfkpo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gkwtqmcdd.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ghpcofyyq.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gfrgvrvto.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gtxgnwxop.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/glhvcivfe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gfdtyxqce.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gwszniqqv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gauswwqhb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxwsdpwto.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gkpaiutmt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gmcipsoqc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gsyzcfowu.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghokgcewi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/glhndhgfs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gpwiayxvu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvambtqrn.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gziwcgbix.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gjchwbkok.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/guxotzrxs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gvkptxgsp.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gpyssjyqb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gqiamjjso.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gflcuxwjk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gyhpoqpwo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gcvgdhmtb.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/grgrektlu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gigwflrpz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gltkphzao.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gdbdsyoud.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/glblrxxnp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/ghnizooyr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gamceabqk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gbzrhguoj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gulcwnhgq.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gwamynpvp.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwapozncd.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gidstxrpy.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/glkcgtvdd.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/ghuhaqrro.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/guyficlkh.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmavgtzej.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrojmxo.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gkyvyuzql.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gjwxfxlzh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gqdrwozsn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gcunfnvwh.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gknokwunf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gvoyhdnax.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/guhvxgeei.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gqposnjpk.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtavvriox.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gcgqttdtv.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gsrhhugft.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/glmmiffuy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/ghaztxmue.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/ggajschjy.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gqhymdksb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gydkhdodn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gbziwpcyk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gvmhoehgl.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/geizmajmb.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gaejutphv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gqnczaawb.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gatjgfbkm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gdhtcidhl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gbfzjyebm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gopkaqbsp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtcxbeflj.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/ghgacqzcy.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/glvkcidee.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gassplauo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gftkoovhh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxjpbsvgx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gwutegmje.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gvmjwrsgo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gsfpfkyfn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/ghlldlzkx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gicwcliqe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gutwbeqzz.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gqfqdcsqs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gkzaztocc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gnhawamwj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gftqstiae.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gzswduaio.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/glvdgbhwc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtznxgakz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpyggixzd.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gmjmfkokw.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gunpbhsio.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gdmiuykhw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gntrszwah.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/grtnfgrue.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnfslijms.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gsunspjzw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkazcjepp.sHtML


<!-- 参考信息 -->