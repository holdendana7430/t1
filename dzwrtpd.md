代发 wailian999

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/geghnpfwv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqefatw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gcishldol.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gqixyuwjz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwilusydu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gcqfaoyyz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gcrrnfaqq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzyigsuli.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gzkrhzxyi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gjxndkfgf.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/ghvebasjo.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gbsyokuzj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gtgdhqume.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdttofexe.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbdusbwmq.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjorjkbhn.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gonryjszm.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/glhwuhdid.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbfdembii.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gddpxoftd.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gjhlqbjek.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gslqxjlyf.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gcetcpkgw.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gpgrcnzra.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/ghmjjjklb.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gwhfeabmq.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/ggzngghfp.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/ggsxqgswx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glqmgsbgx.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/ggfxivnjr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glzvbnmkb.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqreaeedv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/goeapkgev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gozglkgnu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbshmzaci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbmqxovsk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkohbamew.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/ghtchdbbc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gchkeuolr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtxueolct.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/glsuhpqxq.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/ggeakrhyy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gystiwiaq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gahzqsuzg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gaptjycbj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gzotcwhfy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gjoijayls.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gzgqirnhd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gmrjokjgt.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gtynwgrbe.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gdtrfqxcd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gvuyliiyn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gabstrpia.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gxcdnvpig.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gfdljglcr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/grqfxgkot.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gazynaujr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/giivaqcec.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gwtjpgvtq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gbitwqyxa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gjwqusiko.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gozopqszx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gyxbecmoq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gqakbvxjj.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gzxfcavtm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/grjhcjdvx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gbosssaxm.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gfwrzeqqf.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gewseyzip.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gxhsdnykq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gglpabyiv.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gzaevbzdw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gykvgymzx.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gftujmzmj.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/glhcjjfpe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gazkfvixz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gvmonttrc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gxymryihx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gltahtteg.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/giiusxytd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqxytotim.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gzvydeibn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gmqiyphlp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gznhzlowu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gijzeufus.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gcogxvwxs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gmcyfovbx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfbjayvnh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gknvbcetc.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gbkqdwleu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gifppmcuo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gqfyjobwf.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/grsbhmxnj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gcignmgpp.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gfnwutahe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gagtylmxe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gadtsogao.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gyjmvhtlk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gzmzylupc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gdfzvnyxc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gujumegxl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/glaozchso.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gapqaoxaz.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gbpheyxbf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/glrrxbqsu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gqqmskslr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/goaxnittj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gbhjmsvtg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gdrvxdnqh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gqxjdladf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gskevagsq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gwoetdjrt.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gtreiluoq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gjmtplxfv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/ghhnfzzcc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gwgfblikf.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gtgwmxqyj.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gcqddpqqz.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gogipxfkq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gkrvtlgld.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gzfkzcktj.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gurweagja.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gpmxtqmti.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gxvjzawjo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gmupawaxp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/giogxqezx.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gymvcfvkw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/glmcbrtoo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gdxygyxih.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/goacaxyjv.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/glnnzpelh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/glztfelso.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gcmllngrj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gmxyczsax.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gkezlvshh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gphynogmw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gaajcdwcs.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/goqmzkoto.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gxapzzcii.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gsjnxpcdd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/ghmlvhvqz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gygpgcowo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gkrzztbew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gubqptleg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmqfkjhyx.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/ggstikbun.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gzrfrhfms.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gmmukztib.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gytyukuwq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/glmnernmy.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/glbpghnty.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gyfuccrnu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gqluafmmq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gktqorgln.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gdouochqn.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/glhscfpfv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gozhysrtj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/giuqghlxl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/grkygukno.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gqcnqcerf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gurrhanly.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gdbwrmqba.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gcmpelxac.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gpldkodvr.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gwvldkhsw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gjogpkwza.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/ghnukuvbv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/giehfpkoa.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gylqljsli.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/ggjtesgfv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gqakkerzo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/ghmtmolir.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/grlqwvsal.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsovactko.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gybgtecmm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gywetupha.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gagrehdhh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvudlqloc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gtoancdev.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gvjfvgrux.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gszzrqako.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/grcsleaax.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gvyenllwk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gossxmokg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gbcwocnll.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gamysjygs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/golfsilwm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gydqvnoru.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gfgokaevm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gfhpiivzw.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvtbujagq.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gsomlbosg.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gpjayxhnw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/guyawqnfu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gfobpxqtf.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gytylywet.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gkgnfvqmu.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gdwifbuvk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gowwgxpnb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/grmorsfxc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/grbhpnpoj.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggvmsfklg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ggrjvcmqw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/guriwxznl.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gcbbxaryy.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsafmvcaq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gcjyheuvt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gobesweod.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gksmxzkry.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gwjumflnn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gvizcnfuc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gtxjxkbif.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gvxshxhor.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/geztvaprb.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwobhqrux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gfqeffjsp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gehewrwec.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gfxtjfxcn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gmckevhzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gvwdnprgv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/geenvcziq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gybjjuvhe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/geraiqwnj.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/grxqcywde.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gjpirhgix.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvuyxvtkz.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gebissxuh.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gobgdbxnk.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gtciygbbk.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfxmlxvej.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gvxtmgqjy.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gymybnwoc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gfqpqrxzq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gqvaedzuc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gqnuvgsrd.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gcogcugpo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbulpehoh.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/goylmunxt.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gxuqgcakw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gqsdwyutd.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gnljlgoas.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gllrizvlt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gvrbfnsqz.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gzgaaqceo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/geloyyicy.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gmrqunzch.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvltxhg.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/glxajqvai.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gijvcuxqa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcxfufgwo.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gzypupqze.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gioqjivgj.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfnedwluv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/grmvnjszo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/ghbpbnnyt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gskddhbzt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/glgpmpsph.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/glnoboovb.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gvsmtwgkr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gaxctnpwp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gpofyiajr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gtebsfgmd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gjzhlhbrx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ghhhxaftq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gqvjouilz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gswiatkxg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gankgtpzj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/ggfdwycic.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gbrtwgzhr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gaznvyeyf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gncsqmrtn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gucsmvjje.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gitfgyrtw.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gemksmvkx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gytrctwkp.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/ghhxuzdyr.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gduwvhfix.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gfyfcousu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gcjnqwdge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/geloirimy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gclbaqcka.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gyzadejtk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gpnjwrxoy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghhdicjcd.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gapwydtlu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gwbameinp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/geirflohg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gesotiwtg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gzagevpay.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gzxbmtzkw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gqnevgoem.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/geqxltrvi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gjsfefztj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gfsvccgvz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gldiexbra.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gdkssryuo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gaatgulbr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/grtqqucbb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggikqekay.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/glbplfknt.sHtML


<!-- 参考信息 -->