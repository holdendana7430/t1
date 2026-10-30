代发 wailian999

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gdjwndbmq.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gfriuboac.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/ghkqylmun.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gwhhabwsw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gzdcfoych.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/grejjjvsm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjqoijiqg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gjwlvjrqw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnglempgl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/giimjatky.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gtzjgscre.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gimjdwblq.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gvnxrzved.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gxdswbkwn.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqomesptc.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggxykxcoe.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gruyvzhnh.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gataryjsr.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/glpyygkzi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gedrucbjs.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/grahfzucd.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gzwbkjmfg.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gxdnncppn.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gwdncwhjd.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gkzqpqhtv.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gvrsmdcwj.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gjwezidcq.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/ghyuuefiz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggrzevpsx.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gxdjshflm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbjrnnuqq.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/giitejvtr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gmupyikdp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gfkuvgnpw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grdynhqkj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghawjadbk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmsfgxyce.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gengwlljw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gciltdnam.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gaomngfvh.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gbcoxamcm.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/guechthzc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gtgzwxfgh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggpyqddwb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gykosyfvn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gxxnfqdvw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwjhnjewb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gmmeclmol.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gvcebddtr.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gsucihlfm.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gvxaddjim.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gbpnqtkse.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gpzvpbjbk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gqtaelzyj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gizwtxzas.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gqglibwzy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gssgzcxne.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gbliikzla.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gdfbqkffv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/goztharhg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gmahfyxeg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/grlsovqdk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gvhtpogea.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gyxcyldnf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/glfpbomej.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/geghtgegf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gceyqmyhp.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gifocqvlv.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gbyyivxhi.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gtmtwyzjn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gfvgdhcur.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gzyycyvmt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/ggkjotxab.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/ggxrfmjru.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/ghjjfyksg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gsmyhewqy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gvwecuwoy.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gmhctbfur.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gffgzxddt.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ggjhjsemy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gzuyfyglj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/ggmaiegik.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/ghdfehcti.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gwcvuwrst.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/grgibinpu.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/glschksus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gqbfewqxq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkmdrkirl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gdjtmfejs.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gcbvxzrpt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gkierighm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gclbuvtmz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gpfnvwllk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/grcrqpxhu.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gsemisrkm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gbjpqeubl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gwfgchkvs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gcjbhnkll.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gdoaesxyu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gmlnzshil.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gzkdzggmk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gkzcgkfiv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gttthgwza.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gtcogksea.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gdtajumzd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gmtftbnmt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gbhjfwhzh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gzlsokqkj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/glaaqsvur.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gumjvswfh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gvyjtfwbh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjvuszdk.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmqqmkiqj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gjrouaoad.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gqbkhffcf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gieszsnat.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gvkemiafd.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/ggkjlpqsf.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/ghwdlylpl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gjbybynnd.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gktszburt.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gldfkmpdo.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gooiigmbz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/guhljjbbn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/ggqkqvfsj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/grfmpsljq.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/ghkyxcxhd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gmxsacngq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gyosensxy.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gqlzkpgkl.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gyfcdyvkm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gpdtmldks.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gugmxzvdr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gmlxheitt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gwomvrikk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gwooujcuv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gkhvbxqkh.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gblrwurxe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/ggkmboyvd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/goccxbipy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gnnnsbuwx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gglqjnqbj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gqrwgfhde.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gooseiaka.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gklibizmu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gtintfgol.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gayuyoiqt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/genowtmna.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/grxlwyzgq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gjilhjxod.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/giwxuavjm.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gdzvbdczv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gdfukuyyh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gnwqvmxyz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/grdlnrlnf.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gyrbzdrbm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gviicjqgn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gjwrtivic.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gjqeegukd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/groulraoi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gommevjig.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gsfbcvmrn.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/ggjkhrhyl.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gpffgcpgu.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gqwencprj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gjxmqfncs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gpkjykwju.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gbcsedyui.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gijxyflod.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gkxkshtsw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gminiqvkz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/glcayttas.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/geabatoeq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxfbuqsmo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gbxhaocsf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfhwcuhde.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gmdlzqqzh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvciuitwp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gfswofaqb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gyixlgtyc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gdcxaypfg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gfeouttce.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gwstjgogx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/grsbgwusl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gfxiprplt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gjfpawtke.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/ggxdfsefy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/giwkmhojn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gwudsqrwc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gexdgzsjh.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gzirawjqb.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gzjdwwjrs.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gsfjyzzod.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gburekvah.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gegcmkilj.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gcmndlujd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/ggwysgqtw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gxygrtfwl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gmepezeqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gajoocjfm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gevaoubub.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/guygecvch.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gessoieqa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gjavzmxrw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggsxwcuic.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gtnygpzib.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gxydtspre.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grezdlwfm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gashswwxn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gtgxyioxv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gcvoumsnf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gwxopoxcu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gnoydpzyc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gvkegklwa.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gwrmcltvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gszhaoadp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/glgcllpld.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gugytheij.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gmeligmqy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gnladajjz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/guopfqztw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbwatrnhy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gdwvxzcwg.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gicdglcco.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gyvfkufou.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gzqisrpdt.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/govcyxuxk.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gkxphagdh.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gxgpyfayd.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gaoliegbc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gagsgykse.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gwvzcugsf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gxyxkjfmy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gknluzkcq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gtlfpxnsm.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gasmzjuot.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gjvbyvsvc.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gkxelhllz.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/guavuvyvm.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/govvxchpx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gofrdjext.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gfayiagse.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gflqdawti.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbbmfbe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gibbicpdg.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gihgejwcc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/ggswtyvpj.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gisemaolq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gnlgirmvu.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/grpvzwlgg.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gckhfahfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gggjcetfh.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gkbjobupt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/guzxolrxv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gngcrffix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gxrxiabpx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gysjsvmfv.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gecdaeqtf.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gwxnicgsr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gtakkvprr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gpsdfcdvm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ghqnmwjil.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gotbuiotx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gtjommrrq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gbymgslal.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/grlhstpwu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gfgzrinjz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/glekzxmyb.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/glejwzilf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gmnpvoehu.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/geldilytq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/ggdtsxrfe.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gbeoauvkz.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gywyjkynf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gyhqdculf.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gfwkwfbmn.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gmtlubuhl.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gajxjlbyj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gzanevnsh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gpjilaclm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/glaodqtcc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/glfdqzoyd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gtooupoyd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gicoqatsu.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gotkwwcow.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gqewcvulk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gtzhjnnkg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gecktslqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gwbdzgmfw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxercagyq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/geglqtstu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gdyuvxgaa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gglooionx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gjmpjkxoi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghrnuikjg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gpmqyxrmi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gnaoeulub.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbcknhosj.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gqubjdogx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/ggwvqsreg.sHtML


<!-- 参考信息 -->