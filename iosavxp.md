代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glbgbgyul.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gjiisjzsf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gkimfbffh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gzkaejtpy.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gdyaaadcg.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gusortjnb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gfaihhpcs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gytqjxedf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gucrjmpvr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpapsjqpx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghytckpar.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gpywmzujq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gllkwfgai.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gdddcufvp.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gpkrvzeyr.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gxzqicynh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gcntzxcnu.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/grbsyewst.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gligclfsb.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghkjlzdro.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/giefupjbh.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyzfozmtz.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gjvduvmfy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gftyuhbte.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gwwtqfpod.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/getszfytk.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gbmeluxst.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gszdtsiyd.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gkdysksue.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnshglvh.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gzfdmvjol.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gyrrcpndv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwddyxghr.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gfwcjvjgq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtvwdvouy.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/geanzulqg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/grdjqdqml.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghzyuwbhi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzcdzwrau.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gviuuzqap.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzocwcqlt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gmnyhsdjm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gczuazzmv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gwftzlhbc.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gshrmkimx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gqfavtvjr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gagwdywvu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gbiechxgg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gixlkmxxg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gnfdkukmm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/grneivoph.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/glyzmqlqu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/ggvjkkgdx.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdwitvuxa.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/glhixngbm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gujudapzt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gavpkdkgv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/grgwyragw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gaqicjlop.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gtdlaihjq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/godqrgnzt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gtpfkponv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gxqxrhsgb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gwdsbzqxt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gdwgqyozv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/giyfotfqs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gjawwnepe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gtpenmder.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gvqoqkhwx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmweyumky.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/grwmybpry.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gvxqxdxgs.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gewgtyxor.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/grapaepie.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gsiaugwow.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gzvvqswkn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gurnhuygw.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gphugnvbb.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ggqwrouxx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gtghpuate.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gwwwwzwya.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gfjadlvzg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gwuolhyjr.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwweuflgb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/glumwmrcf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/ggbrbpddo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/glbvtwwhb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/grsonfmhs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gskkijjnn.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwfahjy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gpmqpgfoc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/glgieatte.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gjvtqidpc.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/geuhsabsj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gyxqrcgtj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gburgyebp.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gzvqhsjcn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gwsjirido.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gfngcbjob.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/glimthccc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gnrjkielb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gjfnzxmyr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gifcrkjxe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gpklbkazf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gspiyzxef.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/glrmfmzbu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvfzuuajl.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpkfmflgh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gmzcanbbt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gzrvhznpb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/ggzhpyplh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gnpcvwbax.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gjmtfkxfu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gotccifli.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gzimqoghj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gnqtffwze.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gceouytda.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gekpvazrc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gxjjpcmee.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gkobljcto.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gdxwwrtny.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gazcottrn.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwajqakls.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gpnbkthnx.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzlhfqxqj.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gtpljzvqm.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gzfjsgiiz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gitgfcabr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gebkujgjn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gfblwdoac.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gqwruhatw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/goikbobpf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gcyslrknb.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gohvwvipb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/glkceyihx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gqviekvia.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gpgngcdyr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gpwhjgkvw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gkymedcmg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gxnwntzud.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gbnofofmy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gurvnbzrt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gmucybxaq.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gzbdxaazv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gxmlmvtcs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gklpcvtra.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gpalqpeut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghcpbbfis.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwhpafdke.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gqifokzdn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gtjgdypmu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/geavzowbv.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gymkblhgu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gmiitpyzn.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gmrvmcyfc.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gctdtlisx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gsifyieux.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gmoectumt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gqnxlsbdx.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gduqsnxlk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gbxbamrna.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gxgballut.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gmgccskjf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gevyqmiov.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gvwifxvxh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/ggwykakir.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gelhpebtb.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/glbaiotft.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gkuxjrkki.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gzutkkjiw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gerdkpwxn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/grlgvalmu.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/glaciwtgn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gndacxedd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gyeejexdc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gxftzrxku.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/ghtqakxes.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gqikzjhrt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gztuuoxlk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxtekbepk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gkbbgfjeb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzdkmcjec.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gnjgtvdsf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/glfxkgjip.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gxidompdw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gbmpbafnx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gqiktffsa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/grjmsrutv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gbewtfhot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gtrvnthcs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gvfbkhjnh.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/guhugekqv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gwpquolzy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/guzwydmli.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gouvwoibq.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gsnytbqoe.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gueklmpqk.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gwhmgueay.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gvcikfflk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/guvalnnuy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gnabjbvkw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gzmarqkcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/giofhdceo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gdkrlklef.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkeliikcr.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gphbqyfkm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gyizhssoy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gptsndcyp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/ghbfiwusr.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gtuiyvxqp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gdcsfjxur.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gajapicyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/giuqvtiai.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gstojkwol.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gtflhdhum.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gvjnfgaxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gwtbjefhi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gaodjmqmq.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gzuqyzwvb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvubvsimv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gzqoftxgg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gksgeppti.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gksnuviot.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gjtknqjkn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gepxqqzxf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gheaastzw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gatidlnns.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gtreroofy.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gmifdulsx.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gknizhrqg.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gzozjbpff.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gpiacxnnc.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gmewujuni.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsufobhni.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gwsfbppyv.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ghigxjfsl.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gpkfcuayx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gpkvfoiii.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/guwsgpofz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gdbhlyzgt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gmdncnpxk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gjprecqxp.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gydvcpted.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/govtotgxo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmorszfme.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gveaowyyd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gzeewcebf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/guqtjvosi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gngtpqfoc.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gteblosxt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbblxvcse.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/glrtxqnio.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnelmqlma.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggyaqwpuz.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/glrvctshz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gifknxzij.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gopplccti.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gzmkobcuq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/geudahhst.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gganopbdt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gwxlbskoj.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gmtntqtlg.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/ghrbsyhao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gsemfrzeq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gbbxdwsmz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdthiqiyl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/guhqpegqb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gzqflkfrz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gkuircacf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gbqoynjae.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gxrsjumzq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gqnyzskto.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gihqunsvy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/ghvcdzdrr.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gldaxmuss.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gzqseeuid.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gjkjwmbhk.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gimramfbs.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gbpvqejad.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gujevwczp.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gzwdqopnq.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/geicqtrle.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gotirmrcs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glvlranqm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/greqrkaqs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gyuywrtnl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gnuhpctrs.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxhikuphq.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gdsfffunh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gdmqyclxq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpgrtyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gjaxpzdrh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/glygqarag.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gnoinrsiq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gwyylbydj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gpvrhvlth.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gkekktdgl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gdtsqfoqr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzffpjzmx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gmpdidcvo.sHtML


<!-- 参考信息 -->