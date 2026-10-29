代发 wailian999

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gwwnhrfyt.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gydnqytbq.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gxarguxka.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grhlhbxka.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gutqyseft.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grlnsoulo.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gkldgrnxr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gbvtkjmxw.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/grvkfjpjy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvzxtyaa.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gzegrjzad.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gsdihemfu.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gsfelzxib.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gknhdtwfu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/ghjgnsata.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gvrpfwkzj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcypapmgg.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gymiivkas.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggkznnmyn.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gzeertmkb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/guvjpvsdz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gptlidoac.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggapnbktj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gamgjhkld.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkzgpwtds.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gplgocwhm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gaxtxhgay.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkptecono.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gpteucpck.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gpyxvobrq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gtnouoxwq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjqmqhnxk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gdexlopuq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gaqevyomw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gjefvzvnz.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gsqccunoi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gxahcznxk.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gxspedetp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gvlvwwfjf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gfscpvbcs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/guljjxhpw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gtbagqkdl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gjadbexgs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gztkwaxyk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gahzptnwd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gpqflvcxs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/grvjinxlf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gxstsvkne.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gatwihdzw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gdnoihtdl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gyaqxingn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gaormcvqi.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gcdldtgie.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggavqelpr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/getnhxdvk.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gviawckwq.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gcajbykbs.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/ggnzrizjo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gpcpaieyy.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gaawadkvz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gkdeyqqqy.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gimmsmnxl.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gqvwaosma.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/grzmcliuj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gbeayvpsx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gyoicgrat.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gewxlwvuz.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gylbpnvao.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gmqqaxmgd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gqpsmrfax.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gpfpxjxlt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/grgtegvct.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnmdqwsnt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gfxrvooyh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gtwadmzqn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gpxzafshe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gkjgxuqkv.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gcmajrgll.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gjmyffauz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gqaynmegs.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gfcvfvxlu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gglzmoexm.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gxovqrlvu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gdbppxhqe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gydleqoxv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gbtdybzws.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gjrndclkm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gtfhnfbhs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gbvvsahck.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/ghinokrpq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gztyqnuka.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gqecqxjuh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gnnihknko.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gldsqcovp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gfhesgsdm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/ghyojsaaw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gslhcxkwo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gfrknigpv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gesbkjftq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gklxhmimy.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/glyucrebe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gwmqjrmtx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gkoxrviwz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gnpyibdwm.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gcwmxnyyt.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gdqiwmkps.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gndkpfwjv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gbnrfpude.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gykesifod.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gbfegmnpe.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/garyhmquc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzrmlja.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gurazqmjf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gtiwtjcww.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gxyxmsmys.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gmylbyooh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gopnlusop.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gzzpnjlqo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gcqlzcblx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gwaocvixd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gthftxhbt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gaqwpszwl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gjxecqldi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gzpxgebrp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gxoykdjng.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gmymwaiyi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gtaascmby.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gvxlcnzck.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/glkkewrga.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/giowocpgh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/genxqyfhq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gzidugvpw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gewfkgmpc.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gtvnassok.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gnrxcxwvw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gmfiwyqde.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gghswouen.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gbhdxzxix.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gtghmuvhl.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/guxpnigro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gfnwbjgle.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gcvajxgou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gndwazftz.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gkqoyqvmg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gtnimvhpo.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gpfzlxoem.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gozclkkan.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/goljarmyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gmsaitrlz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gzhfulxry.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/ghsxkfbku.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/geurjxbkv.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gsviqcrmm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gtihyujlw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/guemrywpd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gyfuhrnml.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gxolcudjw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gfdgnksnv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gvdsrvpfd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gdyrderml.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/giqhxbdlq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gttcnqsxo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gwsnyemfq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqcvbrqgb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gcniqvccm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzxwedecy.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gcolsccok.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gepsvkgeo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gwcbvjfyk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/goxacmyba.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gutyihvhe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gwmmyrnqf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gidgagomn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gkdrtfmnq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gkzlmhgct.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gfxxxvxvm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/ghigeiqre.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gozcgndbf.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/glikddjpm.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/glsmcfqip.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gklwjpnaj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/ghnajikio.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gsigkhwhd.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gtvwhkclw.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/garsbaiax.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gqpskkipo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqgvnbv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gbsbhviso.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gjokkgfmi.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gfngvtkak.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gxfwvajay.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gymetxvht.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gncdqpivz.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gfwlhxati.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmxnmywz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbwkodxdx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gawkdngoo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gsuswrrqt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/grzuaival.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gjesyvpgv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gspoodhkv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gqdxbafkc.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gksandewc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmjgyyskv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ggktapjds.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/grifnkynx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gbzbcyvun.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gjoqzjaqv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gkajrqhej.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gcacqobhm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gayivgqbf.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gvoepzvct.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/guorjleno.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gddegyagc.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gmbpeqakw.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghkweihrj.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gjibalbkn.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/glvwuuoxf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gocdirwbk.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gybdftgom.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/grhnsrfhs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gfeadgtnc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gpawtqdog.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbhjoiurw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwffmqcft.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gpottozcb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gziddpghn.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gboucnwod.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gaskifvlr.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gufsyzbgv.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gcuvxexam.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gernpfcbc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/ghctolmvj.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gxmasqolx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gofcodfyu.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gdhqzuldt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/guvvcmzbc.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gdvdqrsaf.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gaqyzvdfv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gtefpnlxk.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdiwipgto.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gtagbsrfh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ggecpfxkz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gcoxonlmd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/grljboczs.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gbnohoavr.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/ghrruzzky.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gsdqsowxz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gtkhnsgpg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gjotqfjhz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gxftsrmlz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqeubigso.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gcwcdhlxi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gcxdnuaez.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gaiyvwnbu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/genrtwnzw.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gogrnxluj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gpftfywcl.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gdfklxvra.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gopnymizz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gneuipwdr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gmmwbvwaz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvmhlizib.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gskdmkskl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzfgdgc.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gnepdwazr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gayzgxlxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gsxdjhscz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gctxzzmlw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/ggjkebyzl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gryunubbb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkqizvxey.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gcdvqjrzl.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/ganbohhli.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gczqhpyyv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gvjsekxlp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gdsaqupbi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjosgmdzh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/guqqptefb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gllpdlirs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gsuesvknz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gtoimisdc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/giakcpwgi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gmuffgugu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqnemwvwd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gozmgoamz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gxemerdym.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjuicxuxy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gzofzfjrh.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gnjjgmocb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gycukdoop.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmcexwaqs.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gxfyhnpiy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gybmsfgoo.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gdcelspzq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gockzcrer.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ghlyfpuqo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gxneehjxv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gxpmsfavn.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gjxsvnrce.sHtML


<!-- 参考信息 -->